---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationMember();

$requestRequestBody->setVisibleHistoryStartDateTime(new DateTime("0001-01-01T00:00:00Z"));
$requestRequestBody->setRoles( [
"owner",],
$requestRequestBodyAdditionalData = [
		"@odata.type" => "#microsoft.graph.aadUserConversationMember",
		"user@odata.bind" => "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->chatsById("chat-id")->members()->post($requestRequestBody);


```