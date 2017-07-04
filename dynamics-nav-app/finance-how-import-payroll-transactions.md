---
title: "How to: Import Payroll Transactions"
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# How to: Import Payroll Transactions
To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger. To do this, you first import a csv. file that you receive from the payroll provider into the **General Journal** window. Then you map the external accounts in the payroll file to the relevant G/L accounts. Lastly, you post the payroll transactions according to the account mapping.

## To import a payroll file
1. In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.
2. In the relevant general journal batch, choose the **Import Payroll Transactions** action.
3. In the **Import** window, select the relevant payroll file, and then choose the **OK** button. The file must be in CSV format. 
4. Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.

    The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.
4. Edit or post the journal lines as for any other general ledger transactions. For more information, see [How to: Work With General Journals](ui-work-general-journals.md).   

## See Also
[Finance](finance-setup.md)  
[How to: Work With General Journals](ui-work-general-journals.md)  
