---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DirectoryObject-idRequestBody();

$requestRequestBodyAdditionalData = [
		"@odata.id" => "https://graph.microsoft.com/beta/directoryObjects/{id}",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->devicesById("device-id")->registeredUsersById("directoryObject-id")->post($requestRequestBody);


```