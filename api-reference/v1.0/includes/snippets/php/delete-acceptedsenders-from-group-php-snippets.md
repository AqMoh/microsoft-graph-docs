---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RefRequestBuilderDeleteRequestConfiguration();

$queryParameters = new RefRequestBuilderDeleteQueryParameters();
$queryParameters->id = 'https://graph.microsoft.com/v1.0/users/%7Buser-id%7D';

$requestConfiguration->queryParameters = $queryParameters;


 $graphClient->groupsById('group-id')->acceptedSenders()->$ref()->delete($requestConfiguration);


```