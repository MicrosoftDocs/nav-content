---
title: "How to: Post Year-End Closing Entry"
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: "dynamics-nav-2017"
---
# How to: Post Year-End Closing Entry
As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts. After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.

## To post the year end closing entry
1. In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.
2. In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.
3. Review the entries.
4. To post the journal, choose the **Post** action.

**Note**: If an error is detected, an error message is displayed. If the posting is successful, the posted entries are removed from the journal. After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.

## See Also
[Close Books](year-close-books.md)  
[Close Income Statement](year-close-income-statement.md)  
[How to: Close Accounting Periods](year-close-account-periods.md)  