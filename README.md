#  Azure Resource Deployment – HOS06 Template

This repository contains an ARM template to deploy a Windows virtual machine with networking resources in Azure. It is designed for students and developers working on the HOS06 lab assignment.

---

##  Resources Deployed

- Virtual Network (`studentVNet`)
- Subnet (`studentSubnet`)
- Public IP (`studentPublicIP`)
- Network Interface (`studentVM-nic`)
- Windows Virtual Machine (`studentVM`)

---

##  One-Click Deployment

Click the button below to deploy the template directly from GitHub using the Azure portal:

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsukhmani%2F-CY628Temp%2Fmain%2Fazuredeploy.json)

---

## Manual Deployment via Azure CLI

```bash
az deployment group create \
  --resource-group sukhmani \
  --template-file azuredeploy.json \
  --parameters adminUsername='azureuser' adminPassword='YourSecureP@ssword123'
