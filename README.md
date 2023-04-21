# Microsoft //build '23 Demo

This repo was used as the basis for a //build '23 demo. It shows and is based on a set of new capabilities which are:
  * [App Spaces](https://www.bing.com/search?q=Azure+App+Spaces)
  * [Azure Developer CLI](https://azure.github.io/awesome-azd/about)
  * [Azure Container Container Apps Add-Ons](https://github.com/microsoft/azd-aca-templates/tree/main/springboard)


### Prerequisites 
Some of the above features are in preview. As a result please ensure your subscription is enabled to access these capabilities via:

```
az feature register --name SpringboardApps --namespace Microsoft.App
az feature register --name PrereleaseApiVersionAllowed --namespace Microsoft.App
```

Also make sure you have [AZD installed](https://github.com/Azure/azure-dev#installupgrade-azure-developer-cli) via `brew`, `bash` or `choco`.


### One More Thing
Once everything is in place you should be able simply run:

```
azd login
azd up
```

Your can observe progress either via console output or by visiting App Spaces on the portal.