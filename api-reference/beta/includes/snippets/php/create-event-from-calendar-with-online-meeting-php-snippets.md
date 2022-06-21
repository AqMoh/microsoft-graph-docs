---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();


$requestRequestBody->setSubject('Let\'s go for lunch');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType('HTML');
$body->setContent('Does next month work for you?');


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);


$start->setDateTime('2019-03-10T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);


$end->setDateTime('2019-03-10T14:00:00');
$end->setTimeZone('Pacific Standard Time');


$location = new Location();
$requestRequestBody->setLocation($location);


$location->setDisplayName('Harry\'s Bar');

$attendeesArray = [];

$attendees1 = new Attendee();

$attendees1AdditionalData = [
"type" => 'required',
];
$attendees1->setAdditionalData($attendees1AdditionalData);

$attendeesArray []= $attendees1;
$requestRequestBody->setAttendees($attendeesArray);
$requestRequestBody->setIsOnlineMeeting(True);
$requestRequestBody->setOnlineMeetingProvider('teamsForBusiness');
$result =  $graphClient->me()->calendarsById('calendar-id')->events()->post($requestRequestBody);


```