---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ClaimsMappingPolicy();

$requestRequestBody->setDisplayName('UpdateClaimsPolicy');
 $graphClient->policies()->claimsMappingPoliciesById('claimsMappingPolicy-id')->patch($requestRequestBody);


```