---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeCard();


$clockInEvent = new TimeCardEvent();
$requestRequestBody->setClockInEvent($clockInEvent);
$clockInEvent->setDateTime(new DateTime("2019-03-18T00:00:00.000Z"));
$clockInEvent->setAtApprovedLocation(True);

$notes = new ItemBody();
$clockInEvent->setNotes($notes);
$notes->setContent('Started late due to traffic in CA 237');
$notes->setContentType('text');



$notes = new ItemBody();
$requestRequestBody->setNotes($notes);
$notes->setContent('8 To 5 Inventory management');
$notes->setContentType('text');

$breaksArray = [];

$breaks1 = new TimeCardBreak();$breaks1->setBreakId('string');

$notes = new ItemBody();
$breaks1->setNotes($notes);
$notes->setContent('Lunch break');
$notes->setContentType('text');


$start = new TimeCardEvent();
$breaks1->setStart($start);
$start->setDateTime(new DateTime("2019-03-18T02:00:00.000Z"));
$start->setAtApprovedLocation(True);

$notes = new ItemBody();
$start->setNotes($notes);
$notes->setContent('Reduced break to make up for lost time');
$notes->setContentType('text');



$breaksArray []= $breaks1;
$requestRequestBody->setBreaks($breaksArray);
$requestRequestBodyAdditionalData = [
"onBehalfOfUserId" => 'a3601044-a1b5-438e-b742-f78d01d68a67',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->timeCards()->post($requestRequestBody);


```