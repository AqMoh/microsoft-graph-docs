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
$body->setContent('Does late morning work for you?');


$start = new DateTimeTimeZone();
$requestRequestBody->setStart($start);
$start->setDateTime('2019-06-16T12:00:00');
$start->setTimeZone('Pacific Standard Time');


$end = new DateTimeTimeZone();
$requestRequestBody->setEnd($end);
$end->setDateTime('2019-06-16T14:00:00');
$end->setTimeZone('Pacific Standard Time');


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
$result =  $graphClient->groupsById('group-id')->events()->post($requestRequestBody);


```