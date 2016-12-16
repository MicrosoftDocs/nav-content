---
title: "How to: Invoice Sales"
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: "dynamics-nav-2017"
---

# How to: Invoice Sales

You create a sales invoice or sales order to record your agreement with a customer to sell certain products on certain delivery and payment terms.

**Note**: You must use sales orders if your sales process requires that you can ship parts of an order quantity, for example, because the full quantity is not available at once. If you sell items by delivering directly from your vendor to your customer, as a drop shipment, then you must also use sales orders. For more information, see [How to: Make Drop Shipments](sales-how-drop-shipment.md). In all other aspects, sales orders work the same way as sales invoices. For more information, see [How to: Sell Products](sales-how-sell-products.md).

You can negotiate with the customer by first creating a sales quote, which you can convert to a sales invoice when you agree on the sale. For more information, see [How to: Make Offers](sales-how-make-offers.md).

After the customer has confirmed the agreement, for example after a quote process, you post the sales invoice to create the related quantity and value entries in your system. When you post the sales invoice, you can also email the document as a PDF attachment. You can have the email body prefilled with a summary of the invoice and payment information, such as a link to PayPal. For more information, see [How to: Send Documents by Email](ui-how-send-documents-email.md).

In business environments where the customer must pay before products are delivered, such as in retail, you must wait for the receipt of payment before you deliver the products. In most cases, you process incoming payments some weeks after delivery by applying the payments to their related posted, unpaid sales invoices. For more information, see [How to: Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).

If the posted sales invoice is paid, then you must create a sales credit memo to reverse the sale. For more information, see [How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md).

Products can be both inventory items and services. For more information, see [How to: Register New Products](inventory-how-register-new-products.md). The sales invoice process is the same for both product types.

**Note**: In Dynamics NAV, a product is referred to with the term “item”.

You can fill customer fields on the sales invoice in two ways depending on whether the customer is already registered.

## To create a sales invoice
1. On the Home page,  choose the **Sales Invoice** action.  
3. In the **Customer** field, enter the name of an existing customer.

    Other fields in the **Sales Invoice** window are now filled with the standard information of the selected customer. If the customer is not registered, then follow these steps:
4. In the **Customer** field, enter the name of the new customer.
5. In the dialog box about registering the new customer, choose the **Yes** button.
6. In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.
7. A new customer card opens, prefilled with the information on the selected customer template. The **Name** field is prefilled with the new customer’s name that you entered on the sales invoice.
8. Proceed to fill in the remaining fields on the customer card. For more information, see [How to: Register New Customers](sales-how-register-new-customers.md).  
9. When you have completed the customer card, choose the **OK** button to return to the **Sales Invoice** window.

    Several fields on the sales invoice are now filled with information that you specified on the new customer card.
10. Fill in the remaining fields in the **Sales Invoice** window as necessary. Choose a field to read a short description of the field or link to more information.

    You are now ready to fill the sales invoice lines with inventory items or services that you want to sell to the customer.

    If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the invoice by choosing the **Get Recurring Sales Lines** action.
11. On the **Lines** FastTab, in the **Item** field, enter the number of an inventory item or service.  
12. In the **Quantity** field, enter the number of items to be sold.

    **Note**: For items of type Service, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.

    The **Line Amount** field is updated to show the value in the **Unit Price** field multiplied by the value in the **Quantity** field.

    The price and line amounts are shown with or without sales tax depending on what you selected in the **Prices Including Tax** field on the customer card.
13. In the **Line Discount %** field, enter a percentage if you want to grant the customer a discount on the product. The value in the **Line Amount** field is updated accordingly.

    If you have set up special item prices on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, then the price and amount on the quote line are automatically updated if the agreed price criteria are met. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).
14. To add a comment about the quote line that the customer can see on the printed sales quote, write a text in the **Description** field on an empty line.  
15. Repeat steps 10 through 13 for every item that you want to offer to the customer.

    The totals under the lines are automatically calculated as you create or modify lines.
16. In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.

    If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field. For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).
17. When the sales invoice lines are completed, choose the **Post and Send** action.

The **Post and Send Confirmation** dialog box opens showing the preferred sending method for the customer. You can change the sending method by choosing the lookup button for the **Send Document to** field. For more information, see [How to: Set Up Document Sending Profiles](sales-how-setup-document-send-profiles.md).

The related item and customer ledger entries are now created in your system, and the sales invoice is output as a PDF document. The sales invoice is removed from the list of sales invoices and replaced with a new document in the list of posted sales invoices.

## See Also  
[Manage Sales](sales-manage-sales.md)  
[Set Up Sales](sales-setup-sales.md)  
[Inventory](inventory-manage-inventory.md)    
[How to: Send Documents by Email](ui-how-send-documents-email.md)  
[Work with Dynamics NAV](ui-work-product.md)
