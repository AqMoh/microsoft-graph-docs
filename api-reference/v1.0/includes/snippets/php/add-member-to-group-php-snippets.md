---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new $refRequestBody();

$requestRequestBodyAdditionalData = [
		"@odata.id" => "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groupsById("group-id")->members()->$ref()->post($requestRequestBody);


```