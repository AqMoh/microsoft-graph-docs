---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendActivityNotificationRequestBody();


$topic = new TeamworkActivityTopic();
$requestRequestBody->setTopic($topic);
$topic->setSource("entityUrl");
$topic->setValue("https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2");

$requestRequestBody->setActivityType("taskCreated");

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);
$previewText->setContent("New Task Created");


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);
$recipientAdditionalData = [
"@odata.type" => "microsoft.graph.chatMembersNotificationRecipient",
"chatId" => "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2",
];
$recipient->setAdditionalData($recipientAdditionalData);

$templateParametersArray = [];

$templateParameters1 = new KeyValuePair();$templateParameters1->setName("taskId");
$templateParameters1->setValue("Task 12322");

$templateParametersArray []= $templateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
 $graphClient->chatsById("chat-id")->sendActivityNotification()->post($requestRequestBody);


```