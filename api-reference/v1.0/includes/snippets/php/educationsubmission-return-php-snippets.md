---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$result =  $graphClient->education()->classesById("educationClass-id")->assignmentsById("educationAssignment-id")->submissionsById("educationSubmission-id")->return()->post();


```