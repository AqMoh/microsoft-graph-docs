---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CreateLinkRequestBody();

$requestRequestBody->setType('embed');
$result =  $graphClient->sitesById('site-id')->listsById('list-id')->itemsById('listItem-id')->createLink()->post($requestRequestBody);


```