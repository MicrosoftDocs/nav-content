---
    title: How to Print Remittance Advice
    description: You can help your vendors perform reconciliations by printing remittance advice before you post a payment journal, and after you post a payment.
    documentationcenter: ''
    author: bholtorf

    ms.prod: "dynamics-nav-2017"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 10/26/2017
    ms.author: bholtorf

---

#How to: Print Remittance Advice
You can print remittance advice before posting a payment journal and after posting a payment. This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.

##To print remittance advice
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.  
2. In the **Payment Journal** window, select the payment for which remittance advice must be printed.  
3. Choose the **Print Remittance Advice** action.  
4. In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.  
  
    >[!Note]
    > You can filter using the vendor's external document number to match payments with invoices.

5. On the **Vendor** FastTab, choose the appropriate filters.  
6. Choose **Print** to print the report, or choose **Preview** to view it now.  

## Using Remittance Advice Reports
The following table describes the reports that you can use with remittance advice:

|Report|Description|
|----|----|
|Remittance Advice - Journal Report|This report indicates which documents are included in the payment. For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number. For vendors, you can enter the vendor numbers to include in the report. |
|Remittance Advice - Entries Report| This report indicates which documents are included in the payment. You define the report contents by setting filters. You can set additional fields on the tab by choosing the **Field** field. For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include. |

> [!Note]
> The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances. For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).

##See Also  
[Welcome to Dynamics NAV](across-get-started.md)