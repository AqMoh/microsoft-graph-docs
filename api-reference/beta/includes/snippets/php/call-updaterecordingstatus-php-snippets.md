---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdateRecordingStatusRequestBody();

$requestRequestBody->setClientContext("clientContext-value");
$requestRequestBody->setStatus("notRecording | recording | failed");
$result =  $graphClient->communications()->callsById("call-id")->updateRecordingStatus()->post($requestRequestBody);


```