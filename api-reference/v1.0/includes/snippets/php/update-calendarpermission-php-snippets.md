---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CalendarPermission();

$requestRequestBody->setRole("write");
 $graphClient->usersById("user-id")->calendar()->calendarPermissionsById("calendarPermission-id")->patch($requestRequestBody);


```