---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();



$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType('html');
$body->setContent('<div><div><at id="0">GraphTesting</at>&nbsp;Hello team</div></div>');

$mentionsArray = [];

$mentions1 = new ChatMessageMention();

$mentions1->setId(0);
$mentions1->setMentionText('GraphTesting');

$mentioned = new ChatMessageMentionedIdentitySet();
$mentions1->setMentioned($mentioned);



$conversation = new TeamworkConversationIdentity();
$mentioned->setConversation($conversation);


$conversation->setId('68a3e365-f7d9-4a56-b499-24332a9cc572');
$conversation->setDisplayName('GraphTesting');
$conversation->setConversationIdentityType('team');



$mentionsArray []= $mentions1;
$requestRequestBody->setMentions($mentionsArray);
$reactionsArray = [];
$requestRequestBody->setReactions($reactionsArray);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestRequestBody);


```