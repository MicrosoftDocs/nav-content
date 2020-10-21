---
title: "Using Dynamics NAV as your Business Inbox in Outlook"
description: Dynamics NAV has deep integration with Microsoft 365 enabling you to manage all your business interactions and mail with customers and vendors directly in Outlook.
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.search.keywords: SMTP, mail, Microsoft 365
ms.prod: "dynamics-nav-2018"
---

# Using Dynamics NAV as your Business Inbox in Outlook
Dynamics NAV introduces the ability to manage business interactions with your customers and vendors, directly in Microsoft Outlook. With the Dynamics NAV Outlook Add-in, you can see financial data related to customers and vendors, as well as create and send financial documents, such as quotes and invoices.  

Some companies using Microsoft 365 restrict users' permissions to deploy add-ins. So you must make sure that you have a Microsoft 365 subscription that includes email and allows you to deploy add-ins. You can sign up for a 1-month free trial of Microsoft 365 [here](https://products.office.com/try).  

## Get the add-in
In Dynamics NAV, one of the assisted setup guides is **Set Up Office Add-Ins**. The guide helps you  set up a connection between your Microsoft 365 account and Dynamics NAV. The Dynamics NAV add-in is then automatically added to your Outlook.  

The new add-in is added to the Outlook ribbon, and in Outlook Web Access, you can see it in the add-in ribbon, immediately above the body of the email message.  

## Using the add-in
When you get a message from a customer, directly in Outlook, you can open the Dynamics NAV add-in, which recognizes the customer, and opens the customer card for his company. From this dashboard, you can see overview information for the customer, as well as drill down for more detail on specific documents. You can also dig into the sales history for the customer.
In the add-in, you can create a sales quote and send it back to this customer without leaving Outlook. All of the information that you need to send the sales quote is available in your business inbox in Outlook.  
Once you have the data entered, you can post the quote. You can then send it by email. Dynamics NAV generates a .PDF file with the sales quote and attaches it to the email message that you draft in the add-in.  

Similar experience applies to messages from your vendors and purchase documents.  

Sometimes you want to see more fields that you can see in the add-in, such as when you want to fill in lines in an invoice. To give you a bit more space to work with, you can pop out the add-in to a separate window. It's still part of Outlook, but you have more space. As you enter data for the document in the pop-out view, the changes are automatically saved. When you are done entering data for the document, you can close the page. Choosing the add-in frame in Outlook automatically refreshes the document with the changes you made in the pop-out view.  

## Quick document lookup
The Dynamics NAV Document Links add-in gives you quick access to documents mentioned in email messages. The add-in is available for an email message if a document number is recognized in the body of the message. Opening the add-in provides quick access to the document.  

For example, if you receive an email message that mentions the text *S-QUO100*, Dynamics NAV identifies that as a sales quote, and so you can open this document in Outlook. In Outlook, choose the **Document Links** button immediately above the body of the email message. In the Outlook Web App, choose the *S-QUO1001* text in the body of the email message.  

In the Document Links add-in, you can modify and take actions with the document, just like you can in Dynamics NAV.

## See Also
[Welcome to Dynamics NAV](across-get-started.md)  
[Finance](finance.md)  
[Manage Sales](sales-manage-sales.md)  
[Manage Purchasing](purchasing-manage-purchasing.md)  
