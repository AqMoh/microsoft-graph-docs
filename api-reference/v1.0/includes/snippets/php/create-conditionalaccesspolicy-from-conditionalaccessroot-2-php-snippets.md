---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConditionalAccessPolicy();

$requestRequestBody->setDisplayName('Block access to EXO non-trusted regions.');
$requestRequestBody->setState('enabled');

$conditions = new ConditionalAccessConditionSet();
$requestRequestBody->setConditions($conditions);
$clientAppTypesArray = [];
'all',$clientAppTypesArray []= $clientAppTypes1;
$conditions->setClientAppTypes($clientAppTypesArray);

$applications = new ConditionalAccessApplications();
$conditions->setApplications($applications);
$applications->setIncludeApplications( [
'00000002-0000-0ff1-ce00-000000000000',],


$users = new ConditionalAccessUsers();
$conditions->setUsers($users);
$users->setIncludeGroups( [
'ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba',],


$locations = new ConditionalAccessLocations();
$conditions->setLocations($locations);
$locations->setIncludeLocations( [
'198ad66e-87b3-4157-85a3-8a7b51794ee9',],



$grantControls = new ConditionalAccessGrantControls();
$requestRequestBody->setGrantControls($grantControls);
$grantControls->setOperator('OR');
$builtInControlsArray = [];
'block',$builtInControlsArray []= $builtInControls1;
$grantControls->setBuiltInControls($builtInControlsArray);

$result =  $graphClient->identity()->conditionalAccess()->policies()->post($requestRequestBody);


```