# Cloud Platform Solutions

> **Please note: These labs require that you have an account with Azure and an Internet connection. If you do not have an existing subscription, sign up for a free trial by clicking [this link](https://azure.microsoft.com/en-us/free) and following the posted instructions.**

> **To successfully complete the labs for this course, you will need to first download the lab files by clicking [this link](https://github.com/BGarza-CoIT/D084-Lab-Resources/archive/master.zip).  The lab instructions should be opened with a browser, and indicates when you will need to reference each file to successfully complete each exercise.**

<br />
This repository will include the following labs:

-  Azure Event Grid and Azure Logic Apps
-  Azure AD Identity Protection
-  Azure Network Watcher
-  Configure Azure DNS
-  Deploy and Manage Virtual Machines
-  Governance and Compliance
-  Implement and Manage Azure Web Apps
-  Implement ASR Between Regions
-  Implement Directory Synchronization
-  Implementing File Sync
-  Implement and Manage Storage
-  Load Balancer and Traffic Manager
-  Migrate On-premises Hyper-V VMs to Azure
-  Role-Based Access Control
-  Self-Service Password Reset
-  Virtual Machines and Scale Sets
-  VNet Peering and Service Chaining

Note that the following labs will not be part of the AZ-103 course:

-  Azure Event Grid and Azure Logic Apps
-  Implement and Manage Azure Web Apps
-  Migrate On-premises Hyper-V VMs to Azure
-  Privileged Identity Management

**What are we doing?**

*	We are publishing the lab instructions and lab files on GitHub to afford us the opportunity to scale, version, and stay up-to-date. We hope this will help keep the content current as the Azure platform changes.

*	Within each repository there are lab guides in the Markdown format in the Instructions folder. If appropriate, there are also additional files that are needed to complete the lab within the Allfiles\Labfiles folder. Not every course has corresponding lab files.

**How are we doing?**

*	If as you are progressing through these courses, you identify areas for improvement, please use the Issues tab to provide feedback. We will periodically create new files to incorporate the changes.

**General comments regarding the labs in this course**

* Although not required, it is a good idea to deprovision any existing resources when you have completed each lab. This will help mitigate the risk of exceeding the default CPU quota limits and minimize usage charges.

* Availability of Azure regions and resources in these regions depends to some extents on the type of subscription you are using. To identify Azure regions available in your subscription, refer to https://azure.microsoft.com/en-us/regions/offers/. To identify resources available in these regions, refer to https://azure.microsoft.com/en-us/global-infrastructure/services/. These restrictions might result in failures during template validation or template deployment, in particular when provisioning Azure VMs. If this happens, review error messages and retry deployment with a different VM size or a different region.

* When launching Azure Cloud Shell for the first time, you will likely be prompted to create an Azure file share to persist Cloud Shell files. If so, you can typically accept the defaults, which will result in creation of a storage account in an automatically generated resource group. Note that this might happen again if you delete that storage account.

* Before you perform a template based deployments, you might need to register providers that handle provisioning of resource types referenced in the template. This is a one-time operation (per subscription) required when using Azure Resource Manager templates to deploy resources managed by these resource providers (if these resource providers have not been yet registered). You can perform registration from the subscription's Resource Providers blade in the Azure portal or by using Cloud Shell to run Register-AzResourceProvider PowerShell cmdlet or az provider Azure CLI command.
