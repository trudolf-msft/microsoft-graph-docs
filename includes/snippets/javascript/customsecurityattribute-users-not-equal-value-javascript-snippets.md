---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
	.version('beta')
	.header('ConsistencyLevel','eventual')
	.filter('customSecurityAttributes/Marketing/AppCountry ne \'Canada\'')
	.select('id,displayName,customSecurityAttributes')
	.get();

```