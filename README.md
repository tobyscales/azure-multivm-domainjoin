# Blank Template

![Azure Public Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/PublicLastTestDate.svg)
![Azure Public Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/PublicDeployment.svg)

![Azure US Gov Last Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/FairfaxLastTestDate.svg)
![Azure US Gov Last Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/FairfaxDeployment.svg)

![Best Practice Check](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/BestPracticeResult.svg)
![Cred Scan Check](https://azurequickstartsservice.blob.core.windows.net/badges/100-blank-template/CredScanResult.svg)

This is an empty template and parameters file with the schema reference and top-level properties defined.



| Parameter Name    | What it does   | Default |
| --- | --- | --- |
| location | Azure Region for deployment | Defaults to location of Resource Group |
| virtualMachineName | VM root name. Will automatically be suffixed. | Defaults to vm- plus the name of the resource group. |
| vmSize | Azure VM size | Standard_D2s_v3 |
| adminUsername | Local Admin username | localadmin |
| numberOfInstances | How many VMs to deploy | 2 |
| startNumberingAt | Start numbering VMs from here | 1 |
| suffixLength | Number of digits to append to vmname (NOTE: VM names must be less than 15 characters) | 2 |
| OS | OS Platform for the VM | Windows |
| customImageName | Name of custom image. Leave blank for generic platform images | blank |
| authenticationType | Type of authentication to use on the Virtual Machine | password |
| adminPasswordOrKey | Local Admin password for the VMs | password1! |
| joinDomain | The FQDN of the AD domain to join. Set to 'no' to disable | no |
| ouPath | The OU for the domain computer account. | OU=testOU; DC=domain; DC=Domain; DC=com |
| domainUsername | Username of the account used to join the domain | domainadmin |
| domainPassword | Password of the account used to join the domain | domainpassword1! |
| virtualNetworkName | Vnet name. | Defaults to vn- plus the name of the resource group. |
| addressSpace | CIDR block for the vnet and subnet. | 10.10.10.0/24 |


[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)]("https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftescales%2Fazure-multivm-domainjoin%2Fmaster%2Fazuredeploy.json")  
[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)]("http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Ftescales%2Fazure-multivm-domainjoin%2Fmaster%2Fazuredeploy.json")

----
services: `arm`

----

`Tags: vms, domainjoin, template, arm, extension`


