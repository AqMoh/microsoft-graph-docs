---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendMailRequestBody();


$message = new Message();
$requestRequestBody->setMessage($message);
$message->setSubject('Meet for lunch?');

$body = new ItemBody();
$message->setBody($body);
$body->setContentType('Text');
$body->setContent('The new cafeteria is open.');

$toRecipientsArray = [];

$toRecipients1 = new Recipient();
$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);
$emailAddress->setAddress('fannyd@contoso.onmicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$message->setToRecipients($toRecipientsArray);
$ccRecipientsArray = [];

$ccRecipients1 = new Recipient();
$emailAddress = new EmailAddress();
$ccRecipients1->setEmailAddress($emailAddress);
$emailAddress->setAddress('danas@contoso.onmicrosoft.com');


$ccRecipientsArray []= $ccRecipients1;
$message->setCcRecipients($ccRecipientsArray);

$requestRequestBody->setSaveToSentItems('false');
 $graphClient->me()->sendMail()->post($requestRequestBody);


```