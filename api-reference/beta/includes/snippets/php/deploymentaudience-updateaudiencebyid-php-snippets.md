---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdateAudienceByIdRequestBody();

$requestRequestBody->setMemberEntityType('String');
$requestRequestBody->setAddMembers( [
'String',],
$requestRequestBody->setRemoveMembers( [
'String',],
$requestRequestBody->setAddExclusions( [
'String',],
$requestRequestBody->setRemoveExclusions( [
'String',],
 $graphClient->admin()->windows()->updates()->deploymentsById('deployment-id')->audience()->updateAudienceById()->post($requestRequestBody);


```