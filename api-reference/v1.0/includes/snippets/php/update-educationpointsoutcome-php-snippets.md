---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationOutcome();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.educationPointsOutcome',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
 $graphClient->education()->classesById('educationClass-id')->assignmentsById('educationAssignment-id')->submissionsById('educationSubmission-id')->outcomesById('educationOutcome-id')->patch($requestRequestBody);


```