---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ApplicationsRequestBuilderGetQueryParameters{
	Filter: "startswith(displayName,%20'a')",
	Count: true,
	Top: 1,
	Orderby: "displayName",
}
headers := map[string]string{
	"ConsistencyLevel": "eventual"
}
options := &msgraphsdk.ApplicationsRequestBuilderGetOptions{
	Q: requestParameters,
	H: headers,
}
result, err := graphClient.Applications().Get(options)


```