---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AuthenticationMethodConfiguration();

$requestRequestBody->setId('Sms');
$requestRequestBody->setState('enabled');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.smsAuthenticationMethodConfiguration',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->policies()->authenticationMethodsPolicy()->authenticationMethodConfigurationsById('authenticationMethodConfiguration-id')->patch($requestRequestBody);


```