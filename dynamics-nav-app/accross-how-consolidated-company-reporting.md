---
title: Consolidate Data from Multiple Companies 
description: Get an summary view of the financial health accross your businesses.
documentationcenter: ''
author: bholtorf

ms.prod: "dynamics-nav-2018"
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: consolidation, subsidiaries, consolidate 
ms.date: 07/14/2017
ms.author: bholtorf

---

# How To: Work with the Consolidated Trial Balance Report
If you have more than one company in [!INCLUDE[d365fin](includes/d365fin_md.md)], the Consolidated Trial Balance Report on the Accountant Role Center can give you an overview of the financial health of your overall business.  

The report combines general ledger (G/L) entries from each of your companies in a new company that you create to contain the consolidated data. This company is typically referred to as the "consolidated company." The consolidated company is just a container for the consolidated data, and does not have any live business data. The companies that you include in the consolidated company become **Business Units** in the report.

You can consolidate:  

* Across companies that have different charts of accounts.  
* Companies that use different fiscal years and different currencies.  
* Either the full amount or a percentage of a company's financial information
* Using different currency exchange rates in individual G/L accounts 

Depending on the complexity of your businesses, there are two ways to set up the report:

* If you don't need advanced settings, such as including a company that you only own part of, you can use the **Company Consolidation** assisted setup guide to quickly set up a consolidation. The guide helps you through the basic steps.
* If you do need more advanced settings, you can set up the consolidated company and business units yourself.

## To do a simple consolidation setup 
If your consolidation is straightforward, for example because you wholly-own the business units to consolidate, the **Company Consolidation** assisted setup guide will help you through the following steps:
  
* Choose whether to create a new consolidated company, or whether to consolidate the data in a company that you have already created for the consolidation. The company should not contain transactions.
* Preview the results. [!INCLUDE[d365fin](includes/d365fin_md.md)] verifies that the master data and transactions can be successfully transferred to the consolidated company.

To use the assisted setup guide, follow these steps:

1. On the **Accountant** Role Center, choose the **Assisted Setup** action.
2. Choose **Set up consolidation reporting**, and then complete each step in the assisted setup guide.

## To do an advanced consolidation setup
If you need more advanced settings for your consolidation, you can set up consolidation manually. For example, if you have companies that you own only partially, or you have companies that you don’t want to include in the consolidation. You set up the consolidated company in the say way that you set up other companies. For more information, see [Getting Ready for Doing Business](ui-get-ready-business.md).  

[!INCLUDE[d365fin](includes/d365fin_md.md)] lets you set up a list of companies to consolidate, verify the accounting data before you consolidate it, import files, and generate consolidation reports.  

1. Sign in to the consolidated company.
2. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Units**, and then choose the related link.  
3. Choose **New**, and then fill in the required fields.  

If your business unit uses a foreign currency, you must specify the exchange rate to use in the consolidation. You must also enter consolidation information about the business unit's general ledger accounts. These processes are described in the following sections.

### To prepare general ledger accounts for consolidation 
If the chart of accounts in the business unit differs from the consolidated company, you must prepare general ledger accounts for consolidation. You can specify the accounts to post debits and credits to, and the method to use to translate currencies in the consolidated company. For example, this is useful if you frequently run the report.

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.  
2. Open the card for the account, and then fill in the fields on the **Consolidation** FastTab.

### To specify exchange rates for consolidations
If a business unit uses a different currency than the consolidated company, you must specify exchange rate methods for each account before you consolidate. For each account, the content of the **Consol. Translation Method** field determines the exchange rate. On each business unit card, in the **Currency Exchange Rate Table** field, you specify whether consolidation will use exchange rates from the business unit or the consolidated company. If you use exchange rates from the consolidated company, you can change the exchange rates for a business unit. For business units, if the **Currency Exchange Rate Table** field on the business unit card contains **Local**, you can change the exchange rate from the business unit card. The exchange rates are copied from the **Currency Exchange Rate** table, but you can change them before consolidating. 

The following table describes the exchange rate methods you can use for accounts.

|Exchange rate | Typical use |
|---|---|
|Average Rate (Manual) | You manually calculate the average rate for the period to consolidate. Calculate the average either as an arithmetic average or as a best estimate, and specify the result for each business unit. Used for income statement accounts.| 
|Closing Rate | Used for balance sheet accounts.|
|Last Closing Rate | The rate that was valid in the foreign exchange market on the date for which the balance sheet or income statement is being prepared. You enter this rate for each business unit. Used for balance sheet accounts.|
|Historical Rate | The exchange rate that was valid when the transaction occurred.|
|Composite Rate | The current period amounts are translated at the average rate and added to the previously recorded balance in the consolidated company. This method is typically used for retained earnings accounts because they include amounts from different periods and are therefore a composite of amounts translated with different exchange rates.|
|Equity Rate | This is similar to **Composite**. Differences are posted to separate general ledger accounts.|   

To specify exchange rates for business units, follow these steps:

1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Units**, and then choose the related link.  
2. On the **Business Unit List** page, choose the business unit, and then choose the **Average Rate (Manual)** action.   
3. On the **Change Exchange Rate** page, the contents of the **Relational Exch. Rate** field have been copied from the **Currency Exchange Rate** table, but you can modify them. Close the page.  
4. On the **Navigate** tab, in the **Exch. Rates** group, choose **Closing Rate**.  
5. In the **Relational Exch. Rate Amount** field, enter the exchange rate. 

<!-- ### To include or exclude dimensions

COMMENTING THIS OUT BECAUSE i CANNOT REPRODUCE THE SETTINGS. tHERE IS NO CONSOLIDATION CODE FIELD ON DIMENSIONS OR DIMENSIOIN VALUES.

You can consolidate dimension information and general ledger accounts, as follows:

* To exclude dimension information in the consolidation, leave the **Consolidation Code** field blank, and do not choose dimensions in the **Copy Dimensions** fields in any consolidation functions or reports described later in this topic.
* To include dimension information in the consolidation, leave the **Consolidation Code** field blank. However, the consolidation will only work if the dimension values in the business unit are the same as the consolidated company.
* To consolidate the dimension value code in the business unit with a different dimension value code in the consolidated company, fill in the **Consolidation Code**. -->

### To exclude a company from consolidation
If you do not want to include a business unit in the consolidation, you can exclude it. To do that, go to the business unit card, and clear the **Consolidate** check box.

### To include a partially-owned company in consolidation
If you own only part of a company, you can include a percentage of each transaction that corresponds to the percentage of the company you own. For example, if you own 70% of the company, consolidation will include $70 of an invoice for $100. To specify the percentage of the company you own, go to the business unit card, and enter the percentage in the **Consolidation %** field.  

### To test the data before you consolidate
You can test your data before you transfer it to the consolidated company. [!INCLUDE[d365fin](includes/d365fin_md.md)] looks for differences in the information in the business units and the consolidated company. For example, whether account numbers or dimension codes are different. You must correct errors before you can run the report. You can test the database or, if you are importing data from an XML file, you can test the file.   
  
1. Open the consolidated company.  
2. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Business Units**, and then choose the related link.  
3. Do one of the following:  
  
    * To test a file, choose the **Test File** action, enter the name of the file to test, and then choose **Print**.  
    * To test the database, choose **Test Database**.  

## To run the consolidation
After you have tested the data, you can transfer it to the consolidated company.  
  
1. Sign in to the consolidated company.  
2. On the **Accountant Role Center**, choose the **Run Consolidation** action.  
3. Fill in the required fields.  
4. In the **Where** field, choose **Company Name**, and then choose the consolidated company in the **is** field.  

## To export data from Dynamics NAV and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]
If data for a business unit is in another database, you must export the data to a file before you can include it in the consolidation. Each company must be exported separately. For this purpose, use the **Export Consolidation** batch job.  
  
After you run the batch job, all entries in general ledger accounts are processed. For every combination of selected dimensions and date, the contents of the entries' **Amount** fields are totaled and exported. The next combination of selected dimensions and date with the same account number is processed, then the combinations in the next account number are processed, and so on.  

The exported entries contain the following fields: **Account No.**, **Posting Date**, and **Amount**. If dimensions information was also exported, dimension codes and dimension values are also included.  

1. For each exported line, if the total of the **Amount** fields is a debit, the account number that is set up in the business unit's **Consol. Debit Acc.** field is exported to the line. If the total is a credit, the corresponding number in the **Consol. Credit Acc.** field is exported to the line.  
2. The date used for each exported line is either the period's ending date or, if the transfer occurs each day, the exact date of the calculation.  
3. The dimension value exported for the entry will be the consolidated company dimension value that is set up in the **Consolidation Code** field for that dimension value. If no consolidated company dimension value has been entered in the **Consolidated Code** field for that dimension value, the dimension value itself will be exported to the line.   
4. The XML files also contain the currency exchange rates in the consolidation period. These rates are included in a separate section at the beginning of the file.

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Exporting Your Business Data to Excel](about-export-data.md)
