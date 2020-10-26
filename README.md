# Cloud Platform Solutions

> **Please note: These labs require that you have an account with Azure and an Internet connection. If you do not have an existing subscription, sign up for a free trial by clicking [this link](https://azure.microsoft.com/en-us/free) and following the posted instructions.**

> **To successfully complete the labs for this course, you will need to first download the lab files by clicking [this link](https://github.com/BGarza-CoIT/D084-Lab-Resources/archive/master.zip) and extract the contents.  The lab instructions listed within [this link](https://github.com/CoIT-WGU/D084-Lab-Resources/tree/master/Instructions/Labs) should be opened with a browser, and indicates when you will need to reference each file to successfully complete each exercise.**

<br />

This repository will include the following labs:

-  Azure AD Identity Protection
-  Azure Network Watcher
-  Configure Azure DNS
-  Deploy and Manage Virtual Machines
-  Governance and Compliance
-  Implement ASR Between Regions
-  Implement Directory Synchronization
-  Implementing File Sync
-  Implement and Manage Storage
-  Load Balancer and Traffic Manager
-  Role-Based Access Control
-  Self-Service Password Reset
-  VNet Peering and Service Chaining


## Lab Preparation

#### Task 0: 

1. Log into your [Azure portal](https://www.portal.azure.com) and click **Create a new resource**.

1. Within the **New** blade, search Azure Marketplace for **storage account**, and select **Storage accounts**.

1. Click **Create**.

1. From the **Create storage account** blade, create an account with the following:

    - Subscription: the name of the subscription you are using in this lab
  
    - Resource Group: Click **Create new** and set the name of the resource group to: **azlabfiles-RG**, and click **OK**.
  
    - Storage account name: **azlabfiles&lt;lastname&gt;&lt;MM&gt;&lt;DD&gt;**.
    
        * lastname = your last name | MM = two-digit month | DD = two-digit date.  For example, John Smith creating a storage account on October 26 would be **azlabfilessmith1026**.
  
1. Leave everything else as default. Click **Review + create**.
  
1. Click **Create** once the validation completes.

1. Once you receive a notification that your deployment is complete, click **Go to resource**.

1. Click the **Data transfer** blade.

1. Click **\+Container**.

1. In the **New container** pane that opens on the right side, type **az-labfile-cn**. Then click **Create**.

1. Click on **az-labfile-fs** and within the blade, click **Upload**.


*	We are publishing the lab instructions and lab files on GitHub to afford us the opportunity to scale, version, and stay up-to-date. We hope this will help keep the content current as the Azure platform changes.

*	Within each repository there are lab guides in the Markdown format in the Instructions folder. If appropriate, there are also additional files that are needed to complete the lab within the Allfiles\Labfiles folder. Not every course has corresponding lab files.

**General comments regarding the labs in this course**

* Throughout, and after completing each module, we ask you deprovision all resources created as you progress. This will help mitigate the risk of exceeding the default CPU quota limits and minimize usage charges.

* Availability of Azure regions and resources in these regions depends to some extents on the type of subscription you are using. To identify Azure regions available in your subscription, refer to https://azure.microsoft.com/en-us/regions/offers/. To identify resources available in these regions, refer to https://azure.microsoft.com/en-us/global-infrastructure/services/. These restrictions might result in failures during template validation or template deployment, in particular when provisioning Azure VMs. If this happens, review error messages and retry deployment with a different VM size or a different region.

* When launching Azure Cloud Shell for the first time, you will likely be prompted to create an Azure file share to persist Cloud Shell files. If so, you can typically accept the defaults, which will result in creation of a storage account in an automatically generated resource group. Note that this might happen again if you delete that storage account.

* Before you perform a template based deployments, you might need to register providers that handle provisioning of resource types referenced in the template. This is a one-time operation (per subscription) required when using Azure Resource Manager templates to deploy resources managed by these resource providers (if these resource providers have not been yet registered). You can perform registration from the subscription's Resource Providers blade in the Azure portal or by using Cloud Shell to run Register-AzResourceProvider PowerShell cmdlet or az provider Azure CLI command.
