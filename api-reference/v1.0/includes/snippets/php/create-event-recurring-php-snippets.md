---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();

$requestRequestBody->setSubject('Let's go for lunch');

$body = new ItemBody();
$requestRequestBody->setBody($body);
$body->setContentType('HTML');
$body->setContent('Does noon time work for you?');


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);
$start->setDateTime('2017-09-04T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);
$end->setDateTime('2017-09-04T14:00:00');
$end->setTimeZone('Pacific Standard Time');


$recurrence = new PatternedRecurrence();
$requestRequestBody->setRecurrence($recurrence);

$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);
$pattern->setType('weekly');
$pattern->setInterval(1);
$daysOfWeekArray = [];
'Monday',$daysOfWeekArray []= $daysOfWeek1;
$pattern->setDaysOfWeek($daysOfWeekArray);


$range = new RecurrenceRange();
$recurrence->setRange($range);
$range->setType('endDate');
$range->setStartDate('2017-09-04');
$range->setEndDate('2017-12-31');



$location = new Location();
$requestRequestBody->setLocation($location);
$location->setDisplayName('Harry's Bar');

$attendeesArray = [];

$attendees1 = new Attendee();$attendees1AdditionalData = [
"type" => 'required',
];
$attendees1->setAdditionalData($attendees1AdditionalData);

$attendeesArray []= $attendees1;
$requestRequestBody->setAttendees($attendeesArray);
$requestRequestBody->setAllowNewTimeProposals(True);
$result =  $graphClient->me()->events()->post($requestRequestBody);


```