# Prepare your Azure subscription for lab environment

> **Please note: These labs require that you have an account with Azure and an Internet connection. If you do not have an existing subscription, sign up for a free trial by clicking [this link](https://azure.microsoft.com/en-us/free) and following the posted instructions.**

>

**The lab instructions listed within [this link](https://github.com/CoIT-WGU/D084-Lab-Resources/tree/master/Instructions/Labs) should be opened with a browser, and indicates when you will need to reference each file to successfully complete each exercise.**

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

1. Download the lab files by clicking [this link](https://github.com/BGarza-CoIT/D084-Lab-Resources/archive/master.zip) and extract the contents. **Note the location you save this directory as you will need it later.**

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

1. Click the **Open in Explorer** blade.

1. Click **Open Azure Storage Explorer**.

1. In the **Explorer** pane, navigate to *\<Your subscription\>\\Storage Accounts\\\<Your storage account name\>*.

1. Click **Upload**.

1. Click **Upload folder...**.

1. Navigate to **D084-Lab-Resources-master\Allfiles** in your File Explorer. 

1. Select **LabFiles**, then click **Upload** you documented from step 1.


*	Now you should be able to see all of your necessary lab files stored within your Azure File Share to reference as you progress through the labs.
