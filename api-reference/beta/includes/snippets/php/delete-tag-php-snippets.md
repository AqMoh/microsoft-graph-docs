---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TagRequestBuilderDeleteRequestConfiguration();

$queryParameters = new TagRequestBuilderDeleteQueryParameters();
$queryParameters->forcedelete = true;

$requestConfiguration->queryParameters = $queryParameters;


 $graphClient->compliance()->ediscovery()->casesById('case-id')->tagsById('tag-id')->delete($requestConfiguration);


```