Testing deployments of GitHub Worflows and Azure templates for AHW Tech services

Using personal MSDN Subscription and a secret for actions in Azure
    Service Principal name: yourusername-githubactionazure

Pre-requisites:

 1.  Create resource group, VNET and subnet in your MSDN subscription
 2.  GitHub Desktop
 3.  Visual Studio Code
 4.  GitHub Secret for Actions in Azure
        Create Azure SPN and paste details into GitHub action secret:
                az ad sp create-for-rbac --name "yourusername-githubactionazure" --role contributor --scopes /subscriptions/yoursubscriptionid/resourceGroups/yourresourcegroupname --sdk-auth

FirstSteps:

1. Create a private GitHub repo and clone locally
2. Copy contents from sharepoint folder to local clone
3. Edit parameter files with new resource names
4. Create Azure SPN and set it up as a a secret for actions
5. Commit and push

Resources created:

1. Azure storage account for application A
2. Azure SQL server with DB for application B
3. Azure Windows VM for application C

 




 
