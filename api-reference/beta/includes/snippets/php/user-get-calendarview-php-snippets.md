---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CalendarViewRequestBuilderGetRequestConfiguration();

$queryParameters = new CalendarViewRequestBuilderGetQueryParameters();
$queryParameters->startDateTime = "2020-01-01T19:00:00-08:00";
$queryParameters->endDateTime = "2020-01-02T19:00:00-08:00";

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->calendarView()->get($requestConfiguration);


```