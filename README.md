# AzureStaticWebAppWithBicep
Azure Static Web App with Bicep

## Demo
Site is running at https://nice-stone-071af0403.azurestaticapps.net/

### Notes
I've also added a `staticwebapp.config.json` with a `navigationFallback` like this:
``` json
{
    "navigationFallback": {
        "rewrite": "/index.html"
    }
}
```

Which makes sure that you don't see the default 404 page from Azure like this:
![Azure 404](/resources/azure-404.png)

But the 404 page from the blog:
![Blog 404](/resources/blog-404.png)

### Based on 
- https://blog.johnnyreilly.com/2021/08/15/bicep-azure-static-web-apps-azure-devops
- https://blog.johnnyreilly.com/2021/12/05/azure-static-web-app-deploy-previews-with-azure-devops