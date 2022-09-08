---
title: Create Incoming Documents From Documents
description: You can create records of incoming documents, such as e-invoices, and manage OCR tasks, eCommerce, and document exchange.

documentationcenter: ''
author: SorenGP

ms.prod: "dynamics-nav-2018"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: edupont

---
# How to: Create Incoming Document Records Directly from Documents and Entries
You can store external business documents in [!INCLUDE[d365fin](includes/d365fin_md.md)] by attaching the document files to the related incoming document records. If the document, such as a purchase invoice, did not start its existence as an incoming document record, you can still create and connect an incoming document record to it later. You can also attach incoming document files to posted purchase and sales documents and to vendor, customer, and general ledger entries by using the **Incoming Document Files** FactBox in, for example, the **Posted Purchase Invoices** and **Vendor Ledger Entries** windows.

From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files. For more information, see [How to: Find Posted Documents without Incoming Document Records](across-how-find-posted-documents-without-income-document-records.md).

The following procedures show how to attach a file to an existing purchase invoice that was not created from an incoming document record and how to attach a file to a vendor ledger entry. Attaching a file to posted purchase or sales documents works in a similar way.

## To create and connect an incoming document record from a purchase invoice
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.
2. Select the line for a purchase invoice that you want to attach a file to, and then choose the **Create Incoming Document from File** action.
3. Alternatively, select the line for a purchase invoice that you want to attach a file to, and then choose the **Attach File** action.
4. In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.

## To create and connect an incoming document record from a vendor ledger entry
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Ledger Entries**, and then choose the related link.
2. Select a line for a vendor ledger entry that you want to attach a file to, and then choose the **Create Incoming Document from File** action.
3. Alternatively, select a line for a vendor ledger entry that you want to attach a file to, and then choose the **Attach File** action.
4. In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.

## To remove a connection from an incoming document record to a posted document
You can remove file attachments from non-posted documents at any time by deleting the related incoming document record. If the document is posted, then you must first remove the connection from the incoming document record.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.
2. Select the line for an incoming document record connected to a posted document that you want to remove, and then choose the **Remove Reference to Record** action.

The connection to the posted document is removed. You can now proceed to connect another incoming document record to the posted document as described in this topic.

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[Process Incoming Documents](across-process-income-documents.md)  
[Incoming Documents](across-income-documents.md)  
[Purchasing](purchasing-manage-purchasing.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
