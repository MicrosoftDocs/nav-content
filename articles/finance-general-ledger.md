---
title: "The General Ledger and the Chart of Accounts"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: "dynamics-nav-2017"
---

# The General Ledger and the Chart of Accounts
The general ledger stores your financial data, and the chart of accounts shows the accounts that all general ledger entries are posted to. Dynamics NAV includes a standard chart of accounts that is ready to support your business.

## General Ledger Setup and General Posting Setup
At the core of your business processes is the general ledger and the configuration of how data is posted to the general ledger.
In the **General Ledger Setup** window, you specify how to handle certain accounting issues in your company. This includes invoice rounding details, address formats, and whether you want to use an additional reporting currency, for example.
Similarly, in the **General Posting Setup** window, you specify how you want to set up combinations of general business and general product posting groups. You fill in a line for each combination of business posting group and product posting group.  

## The Chart of Accounts
The chart of accounts shows all accounts. From here, you can open various reports that show your general ledger entries and balances, and you can close the income statement. For each account, you can open the G/L account card and add or change settings. You can also see a list of posting groups that post to that account.  

Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.  

## Account Categories
With account categories, you can map general ledger accounts to categories as a personalization of the structure of your financial statements.  

The **G/L Account Categories** window shows your existing main categories and subcategories and the G/L accounts that you have assigned each category. You can create new subcategories and assign those categories to existing accounts.  

You can group the account categories by indenting individual subcategories. This makes it easy for you to get an overview, because each grouping shows a total balance. For example, you can create subcategories for different types of assets and then create category groups for fixed assets versus current assets, for example. You create a category group by indenting other subcategories under a line in the **G/L Account Categories** window.  

For each subcategory, you can specify if accounts of this category must be included in specific types of financial reports. The account categories help define the layout of your financial statements. For example, the default balance statement has a single entry for cash under assets. If you want the balance statement to have subentries for petty cash and your checking account, then you can add two new subcategories, specify the additional report definition Cash Accounts for each of them, and indent them under the Cash subcategory. Then, when you have generated account schedules based on your changes, your next balance statement will show a total balance for cash and two lines with balances for petty cash and the checking account.     

##See Also
[Finance](finance-setup.md)  
[Set Up or Change the Chart of Accounts](finance-setup-setup-chart-accounts.md)  
[Account Schedules](finance-setup-account-schedule.md)  
