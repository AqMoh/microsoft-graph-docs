---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleEligibilityScheduleRequest();

$requestRequestBody->setAction("AdminRemove");
$requestRequestBody->setJustification("Assign User Admin eligibility to IT Helpdesk (User) group");
$requestRequestBody->setRoleDefinitionId("fdd7a751-b60b-444a-984c-02652fe8fa1c");
$requestRequestBody->setDirectoryScopeId("/");
$requestRequestBody->setPrincipalId("07706ff1-46c7-4847-ae33-3003830675a1");

$scheduleInfo = new RequestSchedule();
$requestRequestBody->setScheduleInfo($scheduleInfo);
$scheduleInfo->setStartDateTime(new DateTime("2021-07-26T18:08:06.2081758Z"));

$expiration = new ExpirationPattern();
$scheduleInfo->setExpiration($expiration);
$expiration->setEndDateTime(new DateTime("2022-06-30T00:00:00Z"));
$expiration->setType("AfterDateTime");


$result =  $graphClient->roleManagement()->directory()->roleEligibilityScheduleRequests()->post($requestRequestBody);


```