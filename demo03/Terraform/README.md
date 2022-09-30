# Terraform Infrastructure

Crear credenciales de Azure

az ad sp create-for-rbac --skip-assignment

{
  "appId": "aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa",
  "displayName": "azure-cli-2019-04-11-00-46-05",
  "name": "http://azure-cli-2019-04-11-00-46-05",
  "password": "aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa",
  "tenant": "aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa"
}

terraform init

terraform plan

terraform apply

# Get Kube Config
az aks get-credentials --resource-group $(terraform output -raw resource_group_name) --name $(terraform output -raw kubernetes_cluster_name)