---
title: "How to: Make predictive cash flow forecasts"
author: bholtorf
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2017"
---

# How to: Make predictive cash flow forecasts
Cash flow forecasts help you ensure that your company has enough cash available to meet its financial obligations, and are useful for identifying adjustments. For example, if you have a cash surplus you might pay off some debts, and you'll appreciate an early warning if times look tight. 

Cortana Intelligence uses the Azure Machine Learning service to make reliable, predictive forecasts. For example, forecasts from Cortana Intelligence can help you predict, and avoid, cash deficits. The service combines historical information with current postings for payables and receivables, including postings with due dates that are in the future. These include:
* Purchase orders
* Sales orders
* Posted sales and purchase invoices
* Credit memos

## Before you start  
There are a few things to do before you can use Cortana Intelligence for cash flow forecasts: 
* If you aren't already using cash flow forecasts, you will need to set up:
	* One or more setups in **Cash Flow Setups**. 
	* Accounts for payables, receivables, sales orders, and purchase orders. Cortana Intelligence uses the postings in these accounts.
	* One or more cash flow forecasts in **Cash Flow Forecast**. Be sure to include purchase orders, sales orders, receivables, and payables as sources.  
	For more information, search for _cash flow forecasts_ in the Help system. 
* Know the API URL and API key for the predictive web service to use.  
    You can use Azure Machine Learning or another service, if you have one. Alternatively, a public model named _Forecasting model for Microsoft Dynamics NAV_ is available online in the Cortana Intelligence Gallery. To use the model, follow these steps:

	1. In a browser, go to the [Cortana Intelligence Gallery](https://go.microsoft.com/fwlink/?linkid=828352)
	2. Search for _Forecasting Model for Microsoft Dynamics NAV_, and then open the model in Azure Machine Learning Studio.
	3. Use your Microsoft account to sign up for a workspace, and then copy the model.
	4. Run the model, and publish it as a web service.
	5. Make a note of the API URL and API key. You will use these credentials when you set up Cortana Intelligence in Microsoft Dynamics NAV.  

* Consider how often to calculate the forecast. The Azure Machine Learning service has limitations regarding use. For example, if you have a lot of items, it might be better to calculate less frequently. 
* Be assigned to the Accountant role center. 

## Set up Cortana Intelligence
You can use an assisted setup guide to set up cash flow forecasts. The guide helps you specify things like how often to update the forecast, the accounts to base it on, information about when you pay taxes, and whether to use Cortana Intelligence.  

If you are already using cash flow forecasts and just want to turn on Cortana Intelligence, you can also use a manual process. When you sign in, a notification displays in a blue bar at the top of the workspace. To set up Cortana Intelligence right away, choose **Yes please**. The message displays only once. If you close it, use the manual process to set up Cortana Intelligence.  

**Tip:** Consider the length of the periods that the service will use in its calculations. The more data you provide, the more accurate the predictions will be. Also, watch out for large variances in periods. They will also impact predictions. If Cortana Intelligence does not find enough data, or the data varies a lot, the service will not make a prediction. 

To use the assisted setup guide:
1. In the Accountant role center, under the **Cash Flow Forecast** chart, choose the **Open Assisted Setup** action.
2. Fill in the fields as necessary in each step of the guide.

To use a manual process:
1. Search for **Cash Flow Setup**, and then choose the related link.
2. Expand the **Cortana Intelligence** FastTab, and then fill in the fields as necessary.

## Turn on Cortana Intelligence for cash flow forecasts
1. Search for **Cash Flow Forecasts**, and then choose the related link.
2. Choose the **Cash Flow Worksheet** action.
3. On the **Cash Flow Worksheet** page, choose the **Suggest Worksheet Lines** action.  
4. Under **Source Types to Include**, choose the **Cortana Intelligence Forecast** check box.

## Investigate a cash flow forecast
To take a good look at the data behind the forecast, including the variance, choose the **Cortana Intelligence** column. The first row in the table displays the variance. The other rows are arranged by source document.  

For example, you can see how the forecast:    
* Handles confirmed sales and purchases 
* Subtracts payables and adds receivables
* Skips duplicate sales orders and purchase orders

## See Also  
[Work With Dynamics NAV](ui-work-product.md)
