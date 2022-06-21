---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReplyRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('samanthab@contoso.onmicrosoft.com');
$emailAddress->setName('Samantha Booth');


$toRecipientsArray []= $toRecipients1;

$toRecipients2 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients2->setEmailAddress($emailAddress);


$emailAddress->setAddress('randiw@contoso.onmicrosoft.com');
$emailAddress->setName('Randi Welch');


$toRecipientsArray []= $toRecipients2;
$message->setToRecipients($toRecipientsArray);

$requestRequestBody->setComment('Samantha, Randi, would you name the group please?');
 $graphClient->me()->messagesById('message-id')->reply()->post($requestRequestBody);


```