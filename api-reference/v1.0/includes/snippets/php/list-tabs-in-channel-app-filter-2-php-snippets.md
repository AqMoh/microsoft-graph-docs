---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TabsRequestBuilderGetRequestConfiguration();

$queryParameters = new TabsRequestBuilderGetQueryParameters();
$queryParameters->expand = "teamsApp";
$queryParameters->filter = "teamsApp/id%20eq%20'com.microsoft.teamspace.tab.planner'";

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById("team-id")->channelsById("channel-id")->tabs()->get($requestConfiguration);


```