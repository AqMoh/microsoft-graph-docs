---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new B2cIdentityUserFlow();

$requestRequestBody->setIsLanguageCustomizationEnabled(True);
$requestRequestBody->setDefaultLanguageTag("en");
 $graphClient->identity()->b2cUserFlowsById("b2cIdentityUserFlow-id")->patch($requestRequestBody);


```