# Azure Web Apps 

- reference: https://docs.microsoft.com/en-us/azure/app-service/quickstart-nodejs?tabs=linux&pivots=development-environment-vscode 

*** The reference above is using VS Code for deployment. 
*** below is for using Azure CLI. 

- reference for CLI: https://docs.microsoft.com/en-us/cli/azure/install-azure-cli-macos

- Get started with azure-cli, in short az. 
https://docs.microsoft.com/en-us/cli/azure/get-started-with-azure-cli

- Command Line with azure-cli for Web App.
https://docs.microsoft.com/en-us/cli/azure/webapp?view=azure-cli-latest

- update deployment by using local zip. 
https://docs.microsoft.com/en-us/azure/app-service/tutorial-nodejs-mongodb-app?tabs=azure-cli%2Cterminal-bash%2Cazure-cli-deploy%2Cdeploy-instructions-azcli%2Cdeploy-zip-linux-mac%2Cdeploy-instructions--zip-azcli

```
zip -r web-app.zip . -x '.??*'

az webapp deploy \
    --name first-azure-app-trial \
    --resource-group appsvc_linux_centralus \
    --src-path ./web-app.zip
```

Here are tips 
https://microsoft.github.io/AzureTipsAndTricks/blog/tip19.html

## More, needs to know 

- Resource group 
- Service Plan 
- Intergrating with Github 