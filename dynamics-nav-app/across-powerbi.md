---
title: "Using the Dynamics NAV Content Pack for Power BI"
author: edupont04
ms.custom: na
ms.date: 08/10/2018
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: "dynamics-nav-2018"
ms.author: edupont
---

# Using the Dynamics NAV Content Pack for Power BI
Getting insights into your Dynamics NAV data is easy with Power BI and the Dynamics NAV content pack. Power BI retrieves your data and then builds an out-of-the-box dashboard and reports based on that data.  

The content pack is preconfigured to work with sales data and financial data from the demonstration company that you get when you sign up for the Dynamics NAV preview.  

- Choose any visual on the dashboard to bring up one of seven underlying reports.  
- Filter the report or add fields that you want to monitor.  
- Pin this customized view to the dashboard to continue tracking.  
The dashboard and underlying reports refresh daily. You can control the refresh schedule and modify the frequency on the dataset.  

## Accessing Dynamics NAV in Power BI
To see your Dynamics NAV data in Power BI, you must have the following:  

- Access to Dynamics NAV. For more information, see [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714).  
- Access to Power BI. For more information, see [Power BI](https://powerbi.microsoft.com).

On the Power BI site, you can find additional information about [adding the Dynamics NAV content pack to Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

To access the Dynamics NAV content pack in Power BI, in the connection window, you must specify the following information:


|           Field           |                                                             Description                                                             |
|---------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
|    **OData Feed URL**     | The OData URL so Power BI can access data from your company, such as <https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US>'). |
| **Authentication method** |                                                          Choose **Basic**.                                                          |
|       **User name**       |                  The email account that you used to sign up for Dynamics NAV, such as <em>me@mybusiness.com</em>.                   |
|       **Password**        |                              This is the web service access key for your user account in Dynamics NAV.                              |

This means that you must get two pieces of information from Dynamics NAV: The OData URL and the web service access key for your user account.  
**Getting the URL**  
When you add Dynamics NAV to Power BI, you must specify a URL so Power BI can access data from your company. In the connection window, the URL is referred to as the **OData Feed URL**, and it must have the following format:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
In this example, *mybusiness* is the name of your Dynamics NAV service, and *CRONUS US* is the name of the demonstration company with *%20* representing the space in the name.   
To get the URL, in Dynamics NAV, search for and open the **Web Services** window. This window lists the web services that are currently available, and you can copy the link from the **OData URL** field for one of the default OData web services.  
**Getting the web service access key**  
In order to use data from Dynamics NAV, in Power BI, in the **Connect to Dynamics NAV** window, you must specify your user name, which is your email account, and a password. The password is the web service access key that is set up for your user account in Dynamics NAV.  
To get a web service access key, in Dynamics NAV, search for the **Users** window, and then open the card for your user account. On the **Web Service Access** FastTab, copy the contents of the **Web Service Access Key** field. If the field is blank, in the ribbon, choose **Change Web Service Access Key**, choose the **Key Never Expires** field, and then choose the OK button. You can then copy the key.  

## Getting Data from Dynamics NAV
The Dynamics NAV dashboard shows the most typical reports that you will want to use to track your business. The data is extracted from your Dynamics NAV company using web services to read live data. In Dynamics NAV, the **Web Services** window lists the web services that have been set up for you, including the following that are consumed by the content pack in Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Note**: If you change the name of any of these web services, the data will not show up in Power BI.  
If you want to add use other data in Power BI, you must find the tables in Dynamics NAV, expose them as web services, and then add them to the content pack. This is an advanced scenario, and we recommend that you start with the data that is already available in Power BI.  

## Troubleshooting
The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance-setup solution. However, if something goes wrong, this section provides a workaround for the most typical issues.  

**"Parameter validation failed, please make sure all parameters are valid"**  
If you see this error after you enter your Dynamics NAV URL, make sure the following requirements are satisfied:  

- The URL follows exactly this pattern:

    <https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US>')  
- Delete any text after the company name in parenthesis  
- Make sure there are no trailing forward slash at the end of the URL.  
- Make sure that it is a secure connection as indicated by the URL starting with *https*.  


**"Login failed"**  
If you get a "login failed" error when you log in to the dashboard, using your Dynamics NAV credentials, then this can be caused by one of the following issues:

* The account you are using does not have permissions to read the Dynamics NAV data from your account.

    Verify your user account in Dynamics NAV, and make sure that you have used the right web service access key as the password, and then try again.  
* The Dynamics NAV  instance that you are trying to connect to does not have a valid SSL certificate. In this case you'll see a more detailed error message ("unable to establish trusted SSL relationship").

    **Note**: Self-signed certificates are not supported.  


**"Oops"**  
If you see an "Oops" error dialog after you pass the authentication dialog, this is most frequently caused by a problem connecting to the data for the content pack.

* Verify that the URL follows the pattern that was specified earlier:

    <https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US>')  
* A common mistake is to specify the full URL for a specific web service:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* Or you might have forgotten to specify the company name:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## See Also
[Welcome to Dynamics NAV](across-get-started.md)  
