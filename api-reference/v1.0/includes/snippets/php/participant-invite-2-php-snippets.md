---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new InviteRequestBody();

$participantsArray = [];

$participants1 = new InvitationParticipantInfo();$participants1AdditionalData = [
			"@odata.type" => "#microsoft.graph.invitationParticipantInfo",
	];
$participants1->setAdditionalData($participants1AdditionalData);

$participantsArray []= $participants1;
$requestRequestBody->setParticipants($participantsArray);
$requestRequestBody->setClientContext("f2fa86af-3c51-4bc2-8fc0-475452d9764f");
$result =  $graphClient->communications()->callsById("call-id")->participants()->invite()->post($requestRequestBody);


```