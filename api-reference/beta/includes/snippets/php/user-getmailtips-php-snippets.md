---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GetMailTipsRequestBody();

$requestRequestBody->setEmailAddresses( [
'danas@contoso.onmicrosoft.com','fannyd@contoso.onmicrosoft.com',],
$requestRequestBody->setMailTipsOptions('automaticReplies, mailboxFullStatus');
$result =  $graphClient->me()->getMailTips()->post($requestRequestBody);


```