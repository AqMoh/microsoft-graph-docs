---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LinkedResource();


$requestRequestBody->setWebUrl('http://microsoft.com');
$requestRequestBody->setApplicationName('Microsoft');
$requestRequestBody->setDisplayName('Microsoft');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.linkedResource',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->me()->todo()->listsById('todoTaskList-id')->tasksById('todoTask-id')->linkedResourcesById('linkedResource-id')->patch($requestRequestBody);


```