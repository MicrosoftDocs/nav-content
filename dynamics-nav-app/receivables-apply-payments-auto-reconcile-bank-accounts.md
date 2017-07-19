---
title: "Apply Payments Automatically and Reconcile Bank Accounts"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# Apply Payments Automatically and Reconcile Bank Accounts
You must regularly reconcile your bank, receivables, and payables accounts in Dynamics NAV by applying payments recorded in the bank to their related unpaid invoices and credit memos or other open entries in Dynamics NAV.

You can perform this task in the **Payment Reconciliation Journal** window by importing a bank statement file or feed to quickly register the payments in Dynamics NAV. An automatic application function applies the payments to their related open customer or vendor ledger entries based on data matches between payment text and entry information. You can review and change automatic applications before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. This means that the bank account is automatically reconciled when all payments are applied.

To enable import of bank statements as a bank feed, you must first set up and enable the Envestnet Yodlee Bank Feed service, and then link your bank accounts to the related online bank accounts. For more information, see [How to: Set Up the Envestnet Yodlee Bank Feeds Service](bank-how-setup-bank-statement-service.md).

**Note**: The Envestnet Yodlee Bank Feeds service, or anther provider's bank feed service, may not be available in your system. Contact your Microsoft partner if you want to use a bank feed service to import bank statements.

Alternatively, you can use the bank data conversion service to have a bank statement file in any format converted to a data stream that you can import into Dynamics NAV. For more information, see [How to: Set Up the Bank Data Conversion Service](bank-how-setup-bank-data-conversion-service.md).

The following table describes a sequence of tasks, with links to the topics that describe them.

|To |See |
|---|----|
|Apply payments to open customer or vendor ledger entries by importing a bank statement, and reconcile the bank account when all payments are applied. | [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md) |
|Manually apply payments by viewing detailed information about matched data and suggestions for candidate open entries to apply payments to. | [How to: Review or Apply Payments After Automatic Application](receivables-how-review-apply-payments-auto-application.md)
|Resolve payments that cannot be applied automatically to their related open ledger entries, for example because the amounts differ or because a related ledger entry does not exist. | [How to: Reconcile Payments That Cannot be Applied Automatically](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Link text on payments to specific customer, vendor, or general ledger accounts to always post recurring cash receipts or expenses to those accounts when no documents exist to apply to.| [How to: Map Text on Recurring Payments to Accounts for Automatic Reconciliation](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## See Also
[Manage Receivables](receivables-manage-receivables.md)  
[Manage Sales](sales-manage-sales.md)
