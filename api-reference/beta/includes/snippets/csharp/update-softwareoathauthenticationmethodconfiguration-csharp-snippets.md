---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new SoftwareOathAuthenticationMethodConfiguration
{
	State = AuthenticationMethodState.Disabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
	.Request()
	.UpdateAsync(authenticationMethodConfiguration);

```