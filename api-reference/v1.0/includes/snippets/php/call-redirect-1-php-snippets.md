---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RedirectRequestBody();

$targetsArray = [];

$targets1 = new InvitationParticipantInfo();$targets1AdditionalData = [
			"@odata.type" => "#microsoft.graph.invitationParticipantInfo",
	];
$targets1->setAdditionalData($targets1AdditionalData);

$targetsArray []= $targets1;
$requestRequestBody->setTargets($targetsArray);
$requestRequestBody->setCallbackUri("https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039");
 $graphClient->communications()->callsById("call-id")->redirect()->post($requestRequestBody);


```