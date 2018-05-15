# VM-Series in an Availability Set Template

This ARM template deploys a VM-Series next generation firewall VM in an availability set of a Azure resource group. It lets you select your:
- Username and Password, or SSH key
- Resource Group and Storage Account inside it
- VNET and subnets to use
- Azure VM size and login for VM-Series (BYOL edition) with 3 NIC's that map to above subnets
- Specify PAN-OS version and VM-Series model: BYOL, hourly pay-as-you-go (PAYG)Bundle 1 or Bundle 2
- Specify the Azure Availability Set (required parameter)


This template is meant to let you do customized deployments of VM-Series instead of deploying from the Azure Marketplace. You can deploy using the "Deploy to Azure" button below or download the template and customize it to your needs. You can also fork the templates into your own GitHub repository.

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fwvanbesien%2FPaloAlto%2Fmaster%2FPaloAlto%2Fazuredeploy.json)



# Support Policy 
This template is released under an as-is, best effort, support policy. It should be seen as community supported and Palo Alto Networks will contribute our expertise as and when possible. We do not provide technical support or help in using or troubleshooting the components of the project through our normal support options such as Palo Alto Networks support teams, or ASC (Authorized Support Centers) partners and backline support options. The underlying product used (the VM-Series firewall) by the scripts or templates are still supported, but the support is only for the product functionality and not for help in deploying or using the template or script itself. Unless explicitly tagged, all projects or work posted in our GitHub repository (at https://github.com/PaloAltoNetworks) or sites other than our official Downloads page on https://support.paloaltonetworks.com are provided under the best effort policy.
