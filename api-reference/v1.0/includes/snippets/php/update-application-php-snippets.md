---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Application();

$requestRequestBody->setDisplayName("New display name");
 $graphClient->applicationsById("application-id")->patch($requestRequestBody);


```