---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ActivityBasedTimeoutPolicy();

$requestRequestBody->setDefinition( [
'definition-value',],
$requestRequestBody->setDisplayName('displayName-value');
$requestRequestBody->setIsOrganizationDefault(True);
$result =  $graphClient->policies()->activityBasedTimeoutPolicies()->post($requestRequestBody);


```