---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PermissionGrantConditionSet();

$requestRequestBody->setPermissionType('delegated');
$requestRequestBody->setClientApplicationsFromVerifiedPublisherOnly(True);
$result =  $graphClient->policies()->permissionGrantPoliciesById('permissionGrantPolicy-id')->includes()->post($requestRequestBody);


```