---
title: "How to: Set Up the Envestnet Yodlee Bank Feeds Service"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: "dynamics-nav-2017"
---

# How to: Set Up the Envestnet Yodlee Bank Feeds Service
You can import electronic bank statements from your bank to quickly fill in the **Payment Reconciliation Journal** window so you can apply payments and reconcile the bank account. For more information, see [Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Note**: The Envestnet Yodlee Bank Feeds service, or anther provider's bank feed service, may not be available in your system. Contact your Microsoft partner if you want to use a bank feed service to import bank statements.

When you have enabled the bank feed service, you must link the involved bank account to the online bank account that the feed will come from. You link bank accounts to online bank accounts in the following different scenarios:

- A bank account does not exist in Dynamics NAV for your online bank account. Therefore, you create the bank account by linking from the online bank account.
- A bank account exists in Dynamics NAV, which you want to link to an online bank account.
- A linked bank account must be unlinked because you want to stop using the bank feed service for the account.
- Online bank accounts have changed and you want to update the information on bank accounts in Dynamics NAV.

When the bank feed service is enabled, you can set a bank account up to automatically import new bank statements into the **Payment Reconciliation Journal** window every two hour. Transactions for payments that have already been posted as applied and/or reconciled in the **Payment Reconciliation Journal** window will not be imported. For more information, see the “To enable automatic import of bank statements” section.

**Note**: If you use the Set Up Company assisted setup, then some of the steps in the following procedures will be performed automatically when you get to the company bank account setup. For more information, see [Welcome to Dynamics NAV](across-get-started.md).

## To enable the bank feed service
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.
2. Open the bank account that you will use for the bank feed service.
3. In the **Bank Account** window, in the **Bank Statement Import Format** field, select YODLEEBANKFEED.  

The bank feed service will be enabled when you link a bank account to its related online bank account. See the next procedure.  

## To create a new linked bank account
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.
2. Select the relevant bank account, and then choose the **Create New Linked Bank Account**. The **Bank Account Linking** window opens after a few moments.

    **Note**: This window shows the actual web page of the Envestnet Yodlee Bank Feeds service. Terminology and functionality in the window may not match instructions provided in this topic.  
3. In the **Online Bank Account Linking** window, in the **Link Account** pane, use the Search function to find the bank where you have one or more online bank accounts.
4. Choose the bank name. The **Log In** pane opens.
5. Enter the username and password that you use to log on to the online bank, and then choose the **Next** button.  
6. The bank feed service prepares to link the first online bank account at the specified bank to a new bank account in Dynamics NAV.

    **Note**: If you have more than one online bank account at the bank, you must create additional bank accounts in Dynamics NAV for those additional online bank accounts. See steps 8 through 10.

    When the process has completed successfully, the bank name will appear in the **My Accounts** pane on the **Linked** tab. The number in brackets indicates how many online bank accounts were linked.
7. Choose the **OK** button.

    If only one online bank account is linked, the **Bank Account Card** window for a new bank account opens, prefilled with the name of the online bank account. In this case, the bank account linking task is completed. All that remains is to set up the bank account. For more information, see [How to: Set Up Bank Accounts](bank-how-setup-bank-accounts.md).

    If more than one online bank accounts were linked, the **Bank Account Linking** window opens listing the additional online bank accounts that are not linked to bank accounts in Dynamics NAV yet. In that case, follow the next step.  
8. In the **Bank Account Linking** window, select the line for an online bank account, and then choose the **Link to New Bank Account** action.

    The **Bank Account Card** window for a new bank account opens, prefilled with the name of the online bank account.

    If a bank account already exists in Dynamics NAV that you want to link the additional online bank account to, follow the next step.  
9. In the **Bank Account Linking** window, select the line for an online bank account, and then choose the **Link to Existing Bank Account** action.
10. In the **Bank Account List** window, select the bank account that you want to link to, and then choose the **OK** button.

## To link a bank account to an online bank account
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.
2. Select the line for a bank account that is not linked to an online bank account, and then choose the **Link to Online Bank Account** action. The **Online Bank Account Linking** window opens with the name of the bank prefilled in the **Link Account** pane.
3. Choose the bank name. The **Log In** pane opens.
4. Enter the username and password that you use to log on to the online bank, and then choose the **Next** button.

    The bank feed service prepares to link your bank account in Dynamics NAV to the related online bank account.

    When the process has completed successfully, the bank name will appear in the **My Accounts** pane on the **Linked** tab. If the bank has more than one bank account, only the bank account that you selected in step 2 is linked.
5. Choose the **OK** button.

In the **Bank Account List** window, the **Linked** check box is selected.

## To unlink a bank account
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.  
2. Select the line for a linked bank account that you want to unlink from its related online bank account, and the choose the **Unlink Online Bank Account** action.

**Note**: If you choose **Yes** on the confirmation dialog, the link to the online bank account is removed, and the log-in details are cleared. To link the bank account to the online bank account again, you must log on to the bank again. For more information, see the “To link a bank account to an online bank account“ section.

## To update bank account linking
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.
2. Select the relevant bank account, and then choose the **Update Bank Account Linking** action.

If issues exist for any of the linked bank accounts in the **Bank Account List** window, the **Bank Account Linking** window opens specifying which bank accounts have issues. Issues can best be resolved by unlinking the online bank account and then re-creating the link. For more information, see the “To link a bank account to an online bank account“ section.

## To enable automatic import of bank statements
1. In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.
2. Select the line for a linked bank account, and then choose the **Automatic Bank Statement Import Setup** action.
3. In the **Automatic Bank Statement Import Setup** window, in the **Number of Days Included** field, specify how far back in time to get new bank transactions for.

    **Note**: It is recommended that you set this value to 7 days or more.
4. Select the **Enabled** check box.  
Every hour, the **Payment Reconciliation Journal** window will now be filled with any new payments that are made on the online bank account.

**Note**: Transactions for payments that have already been posted as applied and/or reconciled in the **Payment Reconciliation Journal** window will not be imported.

## See Also  
[Set Up Banking](bank-setup-banking.md)  
[Manage Bank Accounts](bank-manage-bank-accounts.md)  
[Apply Payments Automatically and Reconcile Bank Accounts](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Customizing Dynamics NAV Using Extensions ](ui-extensions.md)
