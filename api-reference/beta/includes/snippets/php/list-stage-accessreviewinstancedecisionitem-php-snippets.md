---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$result =  $graphClient->identityGovernance()->accessReviews()->definitionsById("accessReviewScheduleDefinition-id")->instancesById("accessReviewInstance-id")->stagesById("accessReviewStage-id")->decisions()->get();


```