# Cloud Platform Solutions

## General comments regarding the labs in this course ##

* To stay within the contraints of the free trial, make sure that you reserve 1-2 hours of dedicated study time per lab and **follow all instructions exactly as stated**. This will ensure that the resources are provisioned and deprovisioned quickly to prevent exceeding your free trial. **Instructions for deprovisioning your resources are included at the end of every lab**.

* Availability of Azure regions and resources in these regions depends to some extents on the type of subscription you are using. To identify Azure regions available in your subscription, refer to https://azure.microsoft.com/en-us/regions/offers/. To identify resources available in these regions, refer to https://azure.microsoft.com/en-us/global-infrastructure/services/. These restrictions might result in failures during template validation or template deployment, in particular when provisioning Azure VMs. If this happens, review error messages and retry deployment with a different VM size or a different region.

* When launching Azure Cloud Shell for the first time, you will likely be prompted to create an Azure file share to persist Cloud Shell files. If so, you can typically accept the defaults, which will result in creation of a storage account in an automatically generated resource group. Note that this might happen again if you delete that storage account.

* Before you perform a template based deployments, you might need to register providers that handle provisioning of resource types referenced in the template. This is a one-time operation (per subscription) required when using Azure Resource Manager templates to deploy resources managed by these resource providers (if these resource providers have not been yet registered). You can perform registration from the subscription's Resource Providers blade in the Azure portal or by using Cloud Shell to run:

PowerShell:
```Powershell
Register-AzResourceProvider
```
or Azure CLI:
```sh
az provider
```
