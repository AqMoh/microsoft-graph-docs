---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new $refRequestBody();

$requestRequestBodyAdditionalData = [
	"@odata.id" => 'https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->applicationsById('application-id')->tokenIssuancePolicies()->$ref()->post($requestRequestBody);


```