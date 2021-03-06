# AzureStaticWebAppWithBicep
Azure Static Web App with Bicep


## Demo
Site is running at https://nice-stone-071af0403.azurestaticapps.net/


### Notes
I've also added a [staticwebapp.config.json](https://docs.microsoft.com/en-us/azure/static-web-apps/configuration) with a `navigationFallback` like this:
``` json
{
    "navigationFallback": {
        "rewrite": "/"
    }
}
```

Which makes sure that when you access an invalid/non-existing URL, you don't see the default 404 page from Azure like this:
![Azure 404](/resources/azure-404.png)

But the 404 page from the blog:
![Blog 404](/resources/blog-404.png)


### References
- https://blog.johnnyreilly.com/2021/08/15/bicep-azure-static-web-apps-azure-devops
- https://blog.johnnyreilly.com/2021/12/05/azure-static-web-app-deploy-previews-with-azure-devops
- https://medium.com/bb-tutorials-and-thoughts/two-ways-to-deploy-react-static-web-apps-service-on-azure-4e4ee7aac852
