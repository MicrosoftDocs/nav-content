---
title: "Dimensions"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: "dynamics-nav-2017"
---

#Dimensions
Dimensions are data that you add to entries to categorize them for analysis. For example, you can have dimensions that indicate which project or department an entry originates from.
Then you can use dimensions instead of setting up separate general ledger accounts for each department and project. This allows you to have rich analysis information in your data without having to use a complicated chart of accounts.
You can define an unlimited number of dimensions with an unlimited number of dimension values.  

For example, you set up a dimension called *Department*, and you use this dimension and a dimension value when you post sales documents. Then, you can later get business intelligence data on which items have been sold by which departments, for example.
The more dimensions you set up and use, the more detailed reports you can base your business decisions on. For example, a single sales entry can include multiple dimension information about which account the item sale has been posted to, where the item was sold, who sold it, and what kind of customer made the purchase.  

## Using dimensions
In a document such as a sales order, you can add dimension information for both an individual document line and the document itself. For example, in the **Sales Order** window, you can enter dimension values for the first two shortcut dimensions directly on the document, and you can add further dimension information if you choose the **Dimensions** button.  
In you work in a journal instead, you can also add dimension information to an entry in the same way, if you have set up shortcut dimensions as fields directly on journal lines.  
You can set up default dimensions for accounts or account types, so that dimensions and dimension values are filled in automatically.  

## Dimension sets
A dimension set is a unique combination of dimension values. It is stored as dimension set entries in the database. Each dimension set entry represents a single dimension value. The dimension set is identified by a common dimension set ID that is assigned to each dimension set entry that belongs to the dimension set.  

When you create a new journal line, document header, or document line, you can specify a combination of dimension values. Instead of explicitly storing each dimension value in the database, a dimension set ID is assigned to the journal line, document header, or document line to specify the dimension set.  

## See Also
[Finance](finance-setup.md)  
[Set Up Dimensions](finance-setup-setup-dimensions.md)  
