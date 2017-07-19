---
title: "Manage Payables"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# Manage Payables
A central task in managing accounts payable is to pay your vendors. You can use functions to automatically fill in the **Payment Journal** window with payments lines for due purchase invoices. To quickly perform the involved bank transactions, you can export multiple payment journal lines to a file, which you then upload to your bank for processing. You can also make payments by check, including to transmit checks as electronic payments.

Another typical task is to apply outgoing payments to their related vendor ledger entries and thereby close the related purchase invoices or purchase credit memos as paid. You can perform this work in the **Payment Reconciliation Journal** window by importing a bank statement file to quickly register the payments in Dynamics NAV. An automatic application function applies the payments to their related open vendor or customer ledger entries based on a data matches between payment text and entry information. You can use various functionality to review and change automatic applications before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. This means that the bank account is automatically reconciled when all payments are applied.

Alternatively, you can apply outgoing payments manually in the **Payment Journal** window or from the related vendor ledger entries.

The following table describes a sequence of tasks within accounts payable, with links to the topics that describe them.

|To |See |
|---|----|
|Generate due vendor payments prioritized according to payment discounts and overdue penalties. Optionally, export the payments to a bank file when posting.|[Make Payments](payables-make-payments.md)|
|Apply vendor payments automatically to unpaid purchase invoices by importing a bank statement file.|[Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Apply vendor payments to unpaid purchase invoices manually.|[How to: Apply Vendor Payments Manually](payables-how-apply-purchase-transactions-manually.md)|

## See Also
[Manage Purchasing](purchasing-manage-purchasing.md)  
[Manage Receivables](receivables-manage-receivables.md)  
[Work With Dynamics NAV](ui-work-product.md)  
[Across Business Areas](ui-across-business-areas.md)
