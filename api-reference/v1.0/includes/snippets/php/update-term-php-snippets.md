---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Term();


$labelsArray = [];

$labels1 = new LocalizedLabel();

$labels1->setName('changedLabel');
$labels1->setLanguageTag('en-US');
$labels1->setIsDefault(True);

$labelsArray []= $labels1;
$requestRequestBody->setLabels($labelsArray);
 $graphClient->sitesById('site-id')->termStore()->setsById('set-id')->termsById('term-id')->patch($requestRequestBody);


```