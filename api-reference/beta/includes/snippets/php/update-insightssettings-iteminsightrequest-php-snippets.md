---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InsightsSettings();

$requestRequestBody->setDisabledForGroup("edbfe4fb-ec70-4300-928f-dbb2ae86c981");
 $graphClient->organizationById("organization-id")->settings()->itemInsights()->patch($requestRequestBody);


```