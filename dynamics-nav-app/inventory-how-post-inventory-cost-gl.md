---
title: "How to: Post Inventory Costs to the General Ledger"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
---

# How to: Post Inventory Costs to the General Ledger   
When you post inventory transactions, such as sales shipments, purchase invoices, or inventory adjustments, the changed quantities and costs are recorded in the item ledger entries and the value entries, respectively. To reflect this change of inventory value in your financial books, you must post inventory costs to the related inventory accounts in the general ledger.

You can post inventory costs to the general ledger in two ways:

- Automatically, so that inventory costs are posted to the general ledger every time you post an inventory transaction.
- Manually, so that inventory costs are only posted to the general ledger when you run a batch job.


## To post inventory costs automatically
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Inventory Setup**, and then choose the related link.
2. In the **Inventory Setup** window, select the **Automatic Cost Posting** check box.

For each inventory transaction that you post, the appropriate values are posted to the inventory account, adjustment account, and COGS account in the general ledger.

Even if you use automatic cost posting, it is still necessary to periodically run the Adjust Cost - Item Entries batch job to ensure that the costs of goods are forwarded to the appropriate outbound transactions, such as sales or transfers. This is especially important in situations where you sell goods before invoicing the purchase of those goods.

If an error occurs in the dimension setup while posting the inventory cost to the general ledger, the posting will end with an error.

## To post inventory costs manually
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Post Inventory Cost to G/L**, and then choose the related link.
2. Post inventory costs to the general ledger manually by running the batch job. When you run this batch job, general ledger entries are created on the basis of value entries. You can post the entries so that they are summarized per posting group.

**Note**: When you run this batch job, you may encounter errors having to do with missing setup or incompatible dimension setup. If the batch job encounters errors in the dimension setup, it overrides these errors and uses the dimensions of the value entry. For any other errors, the batch job skips posting the value entries and lists them at the end of the report in a section titled “Skipped Entries.” To post these entries, you must fix the errors.

To see a list of errors before running the posting batch job, you can run the **Post Invt. Cost to G/L - Test** report. The test report lists all the errors encountered during a test posting. You can then fix the errors, and run the inventory cost posting batch job without skipping any entries.

If you would like to simply get an overview of what values could be posted to the general ledger without actually performing the posting, you can run the Post Inventory Cost to G/L batch job without actually posting the values to the general ledger. You do this by clearing the check mark from the Post field on the request page. This way, when you run the batch job, the report is produced showing the values that are ready to be posted to the general ledger, but they are not posted.

## See Also
[Dynamics 365 Business Central](https://docs.microsoft.com/dynamics365/business-central/)  
[Manage Inventory](inventory-manage-inventory.md)    
[How to: Adjust Item Costs](inventory-how-adjust-item-costs.md)  
[Manage Sales](sales-manage-sales.md)  
[Manage Purchasing](purchasing-manage-purchasing.md)
