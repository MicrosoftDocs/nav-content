---
title: "Set Up Dimensions"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
---

# Set Up Dimensions
You must define which dimensions and dimension values you want to use in your company. You should also define which dimensions you wish to use as global and shortcut dimensions. You should consider carefully which dimensions will be most effective as global and shortcut dimensions for your company.  
You set up all of the different dimensions that you want to track in the **Dimensions** window. The Dimensions window contains one line for each dimension, such as *Project*, *Department*, *Area*, and *Salesperson*.  

For each dimension, you must also set up the dimension values, such as all of the departments in your company. Dimension values can be set up in a hierarchical structure similar to the chart of accounts, so that data can be broken down into various levels of granularity, and subsets of dimension values can be totaled.  

You can specify two global dimensions that will automatically be available everywhere, for example on reports and batch jobs. You can also specify six additional shortcut dimensions that will be available as a field on journal and document lines. The remaining dimensions can be used by accessing a separate window that displays dimensions for the line.  

You can define as many dimensions as you need in your company, and you can define an unlimited number of dimension values for each dimension. All dimensions defined by you can be used on entries in journals and documents, as well as in dimensions-related reports and batch jobs.  

## Set Up Default Dimensions for Customers, Vendors, and Other Accounts
You can set up a default dimension for a specific individual account. This code is then copied to the journal or document when the account number field is filled in on the line. However, you may delete or change the code if appropriate. You can also make a dimension required, so that it is not possible to post an entry with a specific type of account unless the account has a dimension value assigned to it.  

Furthermore, you can set up a default dimension for each type of account so that this code is copied to the journal or document when the account type is filled in on the line. However, you can always change the code on the document if relevant.  

Finally, you can also make a dimension required, so that it is not possible to post an entry with a specific type of account unless the account has a dimension value assigned to it.

## See Also
[Working with Dimensions](finance-dimensions.md)  
[Set Up Core Financial Processes](finance-setup-finance.md)
