# -CY628Temp
# Azure ARM Template Deployment via GitHub Actions

This repo deploys a simple Ubuntu VM using an ARM template and GitHub Actions.

## 📁 Files

- `azuredeploy.json`: ARM template
- `parameters.json`: Deployment parameters
- `.github/workflows/deploy.yml`: GitHub Actions workflow

## 🚀 Deployment

### Manual (Azure CLI)

```bash
az deployment group create \
  --resource-group your-resource-group-name \
  --template-file azuredeploy.json \
  --parameters @parameters.json
