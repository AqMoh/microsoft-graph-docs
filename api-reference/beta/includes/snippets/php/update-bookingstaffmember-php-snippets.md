---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BookingStaffMember();

$workingHoursArray = [];

$workingHours1 = new BookingWorkHours();$workingHours1->setDay('monday');
$timeSlotsArray = [];
$workingHours1->setTimeSlots($timeSlotsArray);
$workingHours1AdditionalData = [
		"@odata.type" => '#microsoft.graph.bookingWorkHours',
		"day@odata.type" => '#microsoft.graph.dayOfWeek',
		"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
	];
$workingHours1->setAdditionalData($workingHours1AdditionalData);

$workingHoursArray []= $workingHours1;

$workingHours2 = new BookingWorkHours();$workingHours2->setDay('tuesday');
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
		"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
	];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours2->setTimeSlots($timeSlotsArray);
$workingHours2AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours2->setAdditionalData($workingHours2AdditionalData);

$workingHoursArray []= $workingHours2;

$workingHours3 = new BookingWorkHours();$workingHours3->setDay('wednesday');
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours3->setTimeSlots($timeSlotsArray);
$workingHours3AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours3->setAdditionalData($workingHours3AdditionalData);

$workingHoursArray []= $workingHours3;

$workingHours4 = new BookingWorkHours();$workingHours4->setDay('thursday');
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours4->setTimeSlots($timeSlotsArray);
$workingHours4AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours4->setAdditionalData($workingHours4AdditionalData);

$workingHoursArray []= $workingHours4;

$workingHours5 = new BookingWorkHours();$workingHours5->setDay('friday');
$timeSlotsArray = [];

$timeSlots1 = new BookingWorkTimeSlot();$timeSlots1->setEnd('17:00:00.0000000');
$timeSlots1->setStart('08:00:00.0000000');
$timeSlots1AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkTimeSlot',
];
$timeSlots1->setAdditionalData($timeSlots1AdditionalData);

$timeSlotsArray []= $timeSlots1;
$workingHours5->setTimeSlots($timeSlotsArray);
$workingHours5AdditionalData = [
"@odata.type" => '#microsoft.graph.bookingWorkHours',
"day@odata.type" => '#microsoft.graph.dayOfWeek',
"timeSlots@odata.type" => '#Collection(microsoft.graph.bookingWorkTimeSlot)',
];
$workingHours5->setAdditionalData($workingHours5AdditionalData);

$workingHoursArray []= $workingHours5;
$requestRequestBody->setWorkingHours($workingHoursArray);
 $graphClient->bookingBusinessesById('bookingBusiness-id')->staffMembersById('bookingStaffMember-id')->patch($requestRequestBody);


```