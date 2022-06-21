---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UsersRequestBuilderGetRequestConfiguration();

$queryParameters = new UsersRequestBuilderGetQueryParameters();
$queryParameters->filter = "startswith(displayName,'Eric')";
$queryParameters->select = "displayName,signInActivity";

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->users()->get($requestConfiguration);


```