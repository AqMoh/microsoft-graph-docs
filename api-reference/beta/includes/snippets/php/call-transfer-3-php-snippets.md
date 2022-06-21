---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TransferRequestBody();


$transferTarget = new InvitationParticipantInfo();
$requestRequestBody->setTransferTarget($transferTarget);
$transferTarget->setEndpointType('default');

$identity = new IdentitySet();
$transferTarget->setIdentity($identity);
$identityAdditionalData = [
];
$identity->setAdditionalData($identityAdditionalData);

$transferTargetAdditionalData = [
"languageId" => 'languageId-value',
"region" => 'region-value',
];
$transferTarget->setAdditionalData($transferTargetAdditionalData);

 $graphClient->communications()->callsById('call-id')->transfer()->post($requestRequestBody);


```