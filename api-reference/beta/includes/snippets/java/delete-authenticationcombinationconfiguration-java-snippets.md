---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().conditionalAccess().authenticationStrength().policies("0e371351-6419-4c8a-8047-61eef0212ffb").combinationConfigurations("6cbbcfd0-5054-4a59-a10e-2d21fe09305d")
	.buildRequest()
	.delete();

```