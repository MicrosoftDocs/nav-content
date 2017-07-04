---
title: "Manage Receivables"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# Manage Receivables#
A central task in managing receivables is to apply incoming payments to their related customer or vendor ledger entries and thereby close the related sales invoices or purchase credit memos as paid. When all payments are applied, you can reconcile the bank account.  

You can perform this task in the **Payment Reconciliation Journal** window by importing a bank statement file or feed to quickly register the payments in Dynamics NAV. An automatic application function applies the payments to their related open customer or vendor ledger entries based on data matches between payment text and entry information. You can review and change automatic applications before you post the journal. You can choose to close any open bank account ledger entries related to the applied ledger entries when you post the journal. This means that the bank account is automatically reconciled when all payments are applied.

**Note**: You can reconcile bank accounts as a separate task in the **Bank Acc. Reconciliation** window, which also supports check ledger entries. For more information, see [How to: Reconcile Bank Accounts Separately](bank-how-reconcile-bank-accounts-separately.md).

Alternatively, you can apply payments in the **Payment Registration** window by manually checking payments received as cash, check, or bank transaction against a generated list of unpaid sales documents. Note that this functionality is only available for sales documents.

As another manual reconciliation of payments you can post each receipt to the relevant general ledger, customer, or other account by entering a payment line in the **Cash Receipt Journal** window. In that case, you can either apply the receipt or refund to one or more open entries before you post the cash receipt journal, or you can apply from the created customer ledger entries.

Another task in managing receivables is to collect outstanding balances, including to manage finance-setup charges and issue reminders.

The following table describes a sequence of tasks, with links to the topics that describe them.

|To |See |
|---|----|
|Apply payments to open customer or vendor ledger entries based on an imported bank statement file or feed, and reconcile the bank account when all payments are applied.|[Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Apply payments to open customer ledger entries based on manual entry in a list of unpaid sales documents. | [How to: Reconcile Customer Payments Manually From a List of Unpaid Sales Documents](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Post cash receipts or refunds for customers in the cash receipt journal and apply to customer ledger entries, either from the journal or from posted ledger entries. | [How to: Reconcile Customer Payments Manually](receivables-how-apply-sales-transactions-manually.md) |
|Remind customers of overdue amounts, calculate interest and finance-setup charges, and manage accounts receivable. | [How to: Collect Outstanding Balances](receivables-collect-outstanding-balances.md) |

## See Also
[Manage Sales](sales-manage-sales.md)  
[Manage Payables](payables-manage-payables.md)  
[Work With Dynamics NAV](ui-work-product.md)  
[Across Business Areas](ui-across-business-areas.md)
