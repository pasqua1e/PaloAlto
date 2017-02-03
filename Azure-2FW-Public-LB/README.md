# Azure-2-Firewalls-Public-Load-Balancer

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fdjspears%2FPaloAlto%2Fmaster%2FAzure-2FW-Public-LB%2FazureDeploy.json)

[<img src="https://camo.githubusercontent.com/536ab4f9bc823c2e0ce72fb610aafda57d8c6c12/687474703a2f2f61726d76697a2e696f2f76697375616c697a65627574746f6e2e706e67" data-canonical-src="http://armviz.io/visualizebutton.png" style="max-width:100%;">](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fdjspears%2FPaloAlto%2Fmaster%2FAzure-2FW-Public-LB%2FazureDeploy.json)

- This is a template was created to support the deployment of a Public Azure Load Balancer in front of 2 Palo Alto Networks Firewalls.  It supports the following features:
- The 2 firewalls deploys with 4 interfaces.  1 MGMT and 3 data plane. 
- Static IP addresses are assigned to the interfaces based on the input in the starting ip address fields.
- This template deloys into existing VNETs and storage accounts within the same region.  As a result, the storage account and VNET must be created before deploying this template.
        The following Storage Account types are supported:
                    Standard_LRS
                    Standard_GRS
                    Standard_RAGRS
                    Premium_LRS
        The following VMs are supported:
                    Standard_D3
                    Standard_D4
                    Standard_D3_v2
                    Standard_D4_v2
                    Standard_A4
                    Standard_DS3_v2
                    Standard_DS4_v2
        NOTE: Make sure the VMs are supported in the specific Storage Account Type and Azure Region.