---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new $valueRequestBody();

$requestRequestBodyAdditionalData = [
	"LocalizedStrings" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->languagesById('userFlowLanguageConfiguration-id')->overridesPagesById('userFlowLanguagePage-id')->$value()->put($requestRequestBody);


```