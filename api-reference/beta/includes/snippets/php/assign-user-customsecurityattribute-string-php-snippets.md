---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();


$customSecurityAttributes = new CustomSecurityAttributeValue();
$requestRequestBody->setCustomSecurityAttributes($customSecurityAttributes);
$customSecurityAttributesAdditionalData = [
];
$customSecurityAttributes->setAdditionalData($customSecurityAttributesAdditionalData);

 $graphClient->usersById('user-id')->patch($requestRequestBody);


```