To ensure the templates are up to date or suitable for your environment, please consult with a CompuNet Engineer before deploying.

* * *

# LB Sandwich - 2 Palo Alto VM's
Deploys 2 PA VM's in a 'Load Balancer Sandwich'. Bootstraps a working PA configuration allowing external access through the LB and PA's to a (manually built) internal server. Update the PA address objects with the correct IP's for the manually deployed web server.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fgenlb.json)
* * *

# PA Bootstrap Creator
This can be used with the above LB Sandwich deployment template. Use this first, create your bootstrap with your specific IP Address in mind and note the folder your new bootstrap exists in.
[Launch Bootstrap Creator](https://cnet-pa-tools.azurewebsites.net/bs_maker)


# 1 Palo Alto VM, Basic
Deploys 1 PA VM, building a new vNet with Route-Tables for Management/Public/Private networks.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fcnet-pa1.json)
* * *

# 1 Palo Alto VM, with Bootstrap
Deploys 1 PA VM, building a new vNet with Route-Tables for Management/Public/Private networks. Bootstrap enabled.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fcnet-pa1-bootstrap.json)
* * *

# 1 Palo Alto VM, into Existing vNet
Deploys 1 PA VM, into an existing vNet, this is not recommended for production.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fcnet-pa1-existing-vnet.json)
* * *

# 2 Palo Alto VM's, LB Sandwich - POC 
**(deprecated, replacement coming soon)**

Deploys 2 PA VM's in a 'Load Balancer Sandwich'. Build's sample subnets and bootstraps a working PA configuration allowing access to a (manually built) web server in the Web subnet. Update the PA address objects with the correct IP's for the manually deployed web server.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fpoc-lbsand-deploy.json)
* * *

# Basic vNet & VM
Deploys 1 or more virtual network with Linux VM, building up to 10 (vNetCount). Can be updated to support higher count very easily, just ask.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fvmvnet.json)
* * *

# Basic vNet, VM, & Gateway
Deploys 1 or more virtual network, Linux VM, and vNet Gateway, building up to 10 (vNetCount). Can be updated to support higher count very easily, just ask.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Fvmvnet-gw.json)
* * *

# Linux VM, Existing vNet
Deploys a Linux VM in existing vNet...cleaner than using the marketplace.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fcnetpalopublic.blob.core.windows.net%2Farm-public%2Flinuxvm.json)
* * *

* * *
