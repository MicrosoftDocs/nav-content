---
    title: How to Archive Sales and Purchase Documents | Microsoft Docs
    description: You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to restore the document that it was archived from.

    documentationcenter: ''
    author: SorenGP

    ms.prod: "dynamics-nav-2018"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 11/21/2018
    ms.author: edupont

---
# How to: Archive Documents
You can archive sales and purchase orders, quotes, return orders, and blanket orders, and you can use the archived document to restore the document that it was archived from.

## To set up automatic document archiving  
You can set up automatic archiving of sales and purchase orders, quotes, blanket orders, and return orders, before you delete documents.

The following procedure describes how to set up automatic archiving of sales documents. The steps are similar for purchase documents.
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.
2. In the **Sales & Receivables Setup** window, fill in the fields as follows.

|Field|Description|
|-----|-----------|
|**Archiving Sales Quotes**|**Never** to never archive sales quotes when they are deleted. **Question** to prompt the user to choose whether to archive sales quotes when they are deleted. **Always** to archive sales quotes automatically when they are deleted.|
|**Archiving Blanket Sales Orders**|Select to archive blanket sales orders automatically each time they are deleted.|
|**Arch. Orders and Ret. Orders**|Select to automatically archive sales orders each time they are deleted.|

## To archive a sales order
The following procedure describes how to archive a sales order. The steps are similar for all orders, blanket orders, return orders, and quotes.

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.  
2.  Open a sales order that you want to archive.  
3.  Choose the **Archive Document** action.

The sales order is archived. You can view it in the **Archived Sales orders** window. From here, you can also use it to restore the sales order that it was archived from.

## To restore a sales order from the archive
The following procedure describes how to restore a sales order. The steps are similar for all orders, blanket orders, return orders, and quotes.

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Archived Sales Orders**, and then choose the related link.
2.  Select the archived sales order that you want to restore, and then choose the **Restore** action.  

The sales order is restored to the earlier state.

NOTE: An archived version of a sales quote / sales order cannot be restored after deleting an original document.

## To delete archived sales orders
The following procedure describes how to delete archived sales orders when the original sales order has been deleted. The steps are similar for other archived sales and purchase documents.

1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Archived Sales Order Versions**, and then choose the related link.  
2.  In the **Delete Archived Sales Order Versions** window, select the appropriate filters.  
3.  Choose the **OK** button.

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[How to: Track Document Lines](across-how-to-track-document-lines.md)  
[Sales](sales-manage-sales.md)  
[General Business Functionality](ui-across-business-areas.md)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
