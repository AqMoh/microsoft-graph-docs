---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrivilegedApproval();


$requestRequestBody->setApprovalState('approvalState-value');
$requestRequestBody->setApproverReason('approverReason-value');
 $graphClient->privilegedApprovalById('privilegedApproval-id')->patch($requestRequestBody);


```