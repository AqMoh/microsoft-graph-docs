---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TenantTag();

$requestRequestBody->setDisplayName('Onboarding');
$requestRequestBody->setDescription('Tenants that we are currently onboarding');
 $graphClient->tenantRelationships()->managedTenants()->tenantTagsById('tenantTag-id')->patch($requestRequestBody);


```