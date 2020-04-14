
# 1 Palo Alto VM, Basic
Deploys 1 PA VM, building a new vNet with Route-Tables/etc.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalotraining.blob.core.windows.net%2Farm-public%2Fcnet-pa1.json)


# 1 Palo Alto VM, Basic, Existing vNet
Deploys 1 PA VM, into an existing vNet, this is not recommended.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalotraining.blob.core.windows.net%2Farm-public%2Fcnet-pa1-existing.json)


# 2 Palo Alto VM's, LB Sandwich
Deploys 2 PA VM's in a 'Load Balancer Sandwich'.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalotraining.blob.core.windows.net%2Farm-public%2Fgpa-deploy.json)


# Basic vNet & VM
Deploys a new virtual network and linux VM, building as many as needed (vNetCount)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalotraining.blob.core.windows.net%2Farm-public%2Fvmvnet.json)


# Basic vNet, VM, & Gateway
Deploys a new virtual network, linux VM, and vNet Gateway, building as many as needed (vNetCount)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalotraining.blob.core.windows.net%2Farm-public%2Fvmvnet-gw.json)

---

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


#### To Deploy via CloudShell:
1. Upload FILENAME.json and FILENAME.parameters.json

1. Create Resource Group
    + New-AzResourceGroup -Location WestUS2 -Name PA-ResourceGroup-Name
1. cd ~
1. Deploy
    + New-AzResourceGroupDeployment -ResourceGroupName PA-ResourceGroup-Name -TemplateFile .\FILENAME.json -TemplateParameterFile .\FILENAME.parameters.json
