---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();


$body = new ItemBody();
$requestRequestBody->setBody($body);
$body->setContentType("html");
$body->setContent("<div><div><at id="0">General</at>&nbsp;Hello there!</div></div>");

$mentionsArray = [];

$mentions1 = new ChatMessageMention();$mentions1->setId(0);
$mentions1->setMentionText("General");

$mentioned = new ChatMessageMentionedIdentitySet();
$mentions1->setMentioned($mentioned);

$conversation = new TeamworkConversationIdentity();
$mentioned->setConversation($conversation);
$conversation->setId("19:0b50940236084d258c97b21bd01917b0@thread.skype");
$conversation->setDisplayName("General");
$conversation->setConversationIdentityType("channel");



$mentionsArray []= $mentions1;
$requestRequestBody->setMentions($mentionsArray);
$result =  $graphClient->teamsById("team-id")->channelsById("channel-id")->messages()->post($requestRequestBody);


```