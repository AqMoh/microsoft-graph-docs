---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TiIndicator();


$requestRequestBody->setDescription('description-updated');
 $graphClient->security()->tiIndicatorsById('tiIndicator-id')->patch($requestRequestBody);


```