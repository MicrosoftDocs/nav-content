---
title: "How to: Use Resources for Jobs"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# How to: Use Resources for Jobs
You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs. For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).

You can also post the usage of a resource in a resource journal. Entries posted in a resource journal have no effect on the general ledger.

## To assign resources to jobs
You assign resources to jobs by creating job planning lines for the job. For more information, see [How to: Create Jobs](projects-how-create-jobs.md).

## To record resource usage for a job

1. In the top right corner, choose the **Search for Page or Report** icon, enter **Job Journals**, and then choose the related link.
2. Open a relevant job journal batch, and then fill in the fields as necessary. Choose a field to read a short description of the field or link to more information.
3. When the journal is complete, choose the **Post** action.

## To adjust resource prices  
If you want to change costs or prices for a large number of resources, you can use a batch job.  

1. In the top right corner, choose the **Search for Page or Report** icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.
2. Fill in the fields on a line as necessary, and then choose the **OK** button.

**Note**: This batch job does not create or adjust alternate costs or prices for resources. It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job. The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.

## To get resource price change suggestions based on existing alternate prices  
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.

## To get resource price change suggestions based on standard prices  
If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.  

1. In the top right corner, choose the **Search for Page or Report** icon, enter **Resource Price Changes**, and then choose the related link.
2. Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.  
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.

## To get resource price change suggestions based on alternate prices  
If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.

1. In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.  
2. Fill in the fields as necessary.
3. Choose the **OK** button.  
4. When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.

## See Also
[Manage Projects](projects-manage-projects.md)  
[Finance](Finance.md)  
[Manage Purchasing](purchasing-manage-purchasing.md)         
[Manage Sales](sales-manage-sales.md)     
[Work With Dynamics NAV](ui-work-product.md)  
