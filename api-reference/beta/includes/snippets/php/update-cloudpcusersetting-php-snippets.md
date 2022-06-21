---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CloudPcUserSetting();

$requestRequestBody->setDisplayName("Example");
$requestRequestBody->setSelfServiceEnabled(True);

$restorePointSetting = new CloudPcRestorePointSetting();
$requestRequestBody->setRestorePointSetting($restorePointSetting);
$restorePointSetting->setFrequencyInHours(16);
$restorePointSetting->setUserRestoreEnabled(True);

$requestRequestBody->setLocalAdminEnabled(False);
$requestRequestBodyAdditionalData = [
	"@odata.type" => "#microsoft.graph.cloudPcUserSetting",
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->deviceManagement()->virtualEndpoint()->userSettingsById("cloudPcUserSetting-id")->patch($requestRequestBody);


```