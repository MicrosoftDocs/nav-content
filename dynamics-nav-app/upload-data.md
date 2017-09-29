---
title: Import Your Legacy Business Data into Dynamics NAV
description: You can migrate data for customers, vendors, and inventory, for example, from Excel, QuickBooks, or Dynamics GP, into Dynamics NAV.
author: edupont04
ms.custom: na
ms.date: 09/25/2017
ms.author: edupont
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.search.keywords: QuickBooks, transfer, import, migrate, initialize, implement
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# Import Data from Other Finance Systems
In Dynamics NAV, you can choose to create an empty company so that you can upload data from other finance-setup systems to use in your new Dynamics NAV. Depending on the finance-setup solution that your business uses today, you can transfer information about customers, vendors, inventory, and bank accounts.
In the Business Owner Role Center, you can access an assisted setup guide that helps you transfer the business data from an Excel file or from other formats. The type of files you can upload depends on the extensions that are available. For example, you can upload data from QuickBooks because Dynamics NAV includes an extension that handles the conversion from QuickBooks. If you want to upload data from other finance-setup solutions, you must either check if an extension is available for that solution or import from Excel.  
Dynamics NAV includes templates for customers, vendors, and inventory items that you can choose to apply when you upload your data.  

## Importing Data from Configuration Packages
[!INCLUDE[navnow](includes/navnow_md.md)] includes a configuration package that you can export to Excel and set up your data there. Then, you can import the data from Excel again. The package consists of 27 tables, including master data such as customers, vendors, items, and accounts, other basic setup tables such as shipping methods, and transactions tables such as sales header and lines.  

> [!NOTE]  
>   Working with configuration packages is advanced functionality, and we recommend that you contact your administrator. For more information, see [Importing Data from Legacy Accounting Software using a Configuration Package](across-import-data-configuration-packages.md).

## See Also
[Finance](Finance.md)  
[Customizing Dynamics NAV Using Extensions](ui-extensions.md)   
[Set Up Your Dynamics NAV](setup.md)
