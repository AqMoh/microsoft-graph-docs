---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Alert();


$requestRequestBody->setAssignedTo('String');
$requestRequestBody->setClosedDateTime(new DateTime("String (timestamp)"));
$requestRequestBody->setComments( [
'String',],
$requestRequestBody->setFeedback('@odata.type: microsoft.graph.alertFeedback');
$requestRequestBody->setStatus('@odata.type: microsoft.graph.alertStatus');
$requestRequestBody->setTags( [
'String',],

$vendorInformation = new SecurityVendorInformation();
$requestRequestBody->setVendorInformation($vendorInformation);


$vendorInformation->setProvider('String');
$vendorInformation->setVendor('String');

 $graphClient->security()->alertsById('alert-id')->patch($requestRequestBody);


```