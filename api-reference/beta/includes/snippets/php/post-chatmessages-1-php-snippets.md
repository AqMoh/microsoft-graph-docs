---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();


$body = new ItemBody();
$requestRequestBody->setBody($body);
$body->setContent("Hello world");

$result =  $graphClient->chatsById("chat-id")->messages()->post($requestRequestBody);


```