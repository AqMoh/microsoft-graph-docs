---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Store();

$requestRequestBody->setDefaultLanguageTag('en-US');
 $graphClient->sitesById('site-id')->termStore()->patch($requestRequestBody);


```