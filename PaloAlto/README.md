# VM-Series in an Availability Set Template

This ARM template deploys a VM-Series next generation firewall VM in an availability set of a Azure resource group. It lets you select your:
- Username and Password, or SSH key
- Resource Group and Storage Account inside it
- Azure VM size and login for VM-Series (BYOL edition) with 3 NIC's that map to above subnets
- Specify PAN-OS version and VM-Series model: BYOL, hourly pay-as-you-go (PAYG)Bundle 1 or Bundle 2
- Specify the Azure Availability Set (required parameter)


This template is meant to let you do customized deployments of VM-Series instead of deploying from the Azure Marketplace. You can deploy using the "Deploy to Azure" button below or download the template and customize it to your needs. You can also fork the templates into your own GitHub repository.

[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fwvanbesien%2FPaloAlto%2FMD%2FPaloAlto%2Fazuredeploy.json)



**Check the status of your deployment:**

- CLI: `azure vm show  -g YourResourceGroupName  -n YourDeploymentLabel`
- Azure Portal: Your Resource Group > Deployment or Alert Logs


If you are creating customized ARM templates you can use the following information to deploy VM-Series:

- Publisher name: paloaltonetworks
- Offer: vmseries1
- SKU: byol or bundle1 or bundle2
- Version: 8.0.0, 7.1.1 or latest (recommended)

