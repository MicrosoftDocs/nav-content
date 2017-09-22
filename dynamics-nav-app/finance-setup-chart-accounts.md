---
title: "Set Up or Change the Chart of Accounts"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# Set Up or Change the Chart of Accounts
The chart of accounts shows the ledger accounts that store your financial data. Dynamics NAV includes a standard chart of accounts that is ready to support your business.
However, you can change the default accounts, and you can add new accounts.  

## Adding or Changing Accounts
From the chart of accounts, you can open each G/L account and add or change settings.

**Note**: You can delete a general ledger account. However, before you delete it, the following must be true:  
- The balance on the account must be zero.  
- The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.  
- If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.  

Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.  

##See Also  
[The General Ledger and the Chart of Accounts](finance-general-ledger.md)  
[Manage Bank Accounts](bank-manage-bank-accounts.md)  
[Dimensions](finance-setup-dimensions.md)  
[How to: Work With GIFI Codes in Canada](ca-finance-work-GiFI-codes.md)
