---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MeetingRegistrationQuestion();


$requestRequestBody->setAnswerInputType('radioButton');
$requestRequestBody->setAnswerOptions( [
'Software Engineer','Software Development Manager','Product Manager','Data scientist','Other',],
 $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->registration()->customQuestionsById('meetingRegistrationQuestion-id')->patch($requestRequestBody);


```