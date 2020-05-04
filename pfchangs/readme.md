To ensure the templates are up to date or suitable for your environment, please consult with a CompuNet Engineer before deploying.

* * *
![image info](endor.png)

# Project Endor - Phase 1

## P.F. Chang's UAT / Prod ARM Deployment
Deploys 1 PA VM, building a new vNet with Route-Tables for Management/Public/Private networks. Bootstrap enabled.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fcnet-pa1-lb.json)
* * *


* * *

#### To Deploy via PowerShell:

1. Login
    + Connect-AzAccount

1. View subscriptions
    + Get-AzSubscription

1. Set subscription
    + Set-AzContext -SubscriptionId <ID>

1. Create Resource Group
    + New-AzResourceGroup -Location WestUS2 -Name PA-ResourceGroup-Name

1. Deploy
    + New-AzResourceGroupDeployment -ResourceGroupName PA-ResourceGroup-Name -TemplateFile .\FILENAME.json -TemplateParameterFile .\FILENAME.parameters.json

* * *

#### To Deploy via CloudShell:
1. Upload FILENAME.json and FILENAME.parameters.json

1. Create Resource Group
    + New-AzResourceGroup -Location WestUS2 -Name PA-ResourceGroup-Name
1. cd ~
1. Deploy
    + New-AzResourceGroupDeployment -ResourceGroupName PA-ResourceGroup-Name -TemplateFile .\FILENAME.json -TemplateParameterFile .\FILENAME.parameters.json
