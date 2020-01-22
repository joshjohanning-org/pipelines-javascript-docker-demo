
# Getting Started

```bash
# Create a resource group
az group create --name js-docker-pipelines-demo-rg --location eastus

# Create a container registry
az acr create --resource-group js-docker-pipelines-demo-rg --name jsdockerpipelinesdemoacr --sku Basic

# Create a Kubernetes cluster
az aks create \
    --resource-group js-docker-pipelines-demo-rg \
    --name jsdockerpipelinesdemoaks \
    --node-count 1 \
    --enable-addons monitoring \
    --generate-ssh-keys
```
