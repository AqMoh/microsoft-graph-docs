---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new $refRequestBody();

$requestRequestBodyAdditionalData = [
		"@odata.id" => "https://graph.microsoft.com/beta/education/users/14011",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->education()->classesById("educationClass-id")->teachers()->$ref()->post($requestRequestBody);


```