---
    title: How to Set Up Approval Users 
    description: Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes. In the Approval User Setup window, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.
    
    documentationcenter: ''
    author: SorenGP

    ms.prod: "dynamics-nav-2018"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 07/01/2017
    ms.author: edupont

---
# How to: Set Up Approval Users
Before you can create workflows that involve approval steps, you must set up the workflow users who are involved in approval processes. In the **Approval User Setup** window, you also set amount limits for specific types of requests and define substitute approvers to whom approval requests are delegated when the original approver is absent.  

> [!NOTE]  
>  Approval users, both approval requesters and approvers, must first be set up as workflow users in the **Workflow User Group** window. For more information, see [How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md).  

 When you have set up approval users, you can use the setup to create workflow responses for approval workflows. For more information, see step 9 in [How to: Create Workflows](across-how-to-create-workflows.md).  

> [!NOTE]  
>  To define that an approval request is not approved until multiple approvers in an approval chain have approved it, set up approvers in a hierarchy. For approver type **Approver**, set approvers up in the **Approval User Setup** window. For approver type, **Workflow User Group**, set approvers up in the **Workflow User Groups** window and define the hierarchy by assigning incremental numbers to each approver in the **Sequence No.** field. For more information, see this topic and [How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md).  
>   
>  To define that an approval request is not approved until multiple equal approvers have approved it, regardless of a hirarchy, set up a flat workflow user group. For approver type, **Workflow User Group**, set up approvers in the **Workflow User Groups** window and assign the same number to each approver in the **Sequence No.** field. For more information, see [How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md).  

## To set up an approval user  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Approval User Setup**, and then choose the related link.  
2. Create a new line in the **Approval User Setup** window, and then fill the fields as described in the following table.  

    |Field|Description|  
    |---------------------------------|---------------------------------------|  
    |**User ID**|Select the user ID of the user who is involved in the approval process.|  
    |**Salespers./Purch. Code**|Specify the salesperson or purchaser code that applies to the user in the **Salespers./Purch. Code** field.<br /><br /> You typically fill the **Salespers./Purch. Code** field if the salesperson or purchaser who is responsible for the customer or vendor is also the person who must approve the sales or purchase request in question.|  
    |**Approver ID**|Select the user ID of the user who must approve requests made by the user in the **User ID** field.|  
    |**Sales Amount Approval Limit**|Specify the maximum sales amount in LCY that the user in the **User ID** field can approve.|  
    |**Unlimited Sales Approval**|Specify that the user in the **User ID** field can approve all sales requests regardless of their amount.<br /><br /> If you select this check box, then you cannot fill the **Sales Amount Approval Limit** field.|  
    |**Purchase Amount Approval Limit**|Specify the maximum purchase amount in LCY that the user in the **User ID** field can approve.|  
    |**Unlimited Purchase Approval**|Specify that the user in the **User ID** field can approve all purchase requests regardless of their amount.<br /><br /> If you select this check box, then you cannot fill the **Sales Amount Approval Limit** field.|  
    |**Request Amount Approval Limit**|Specify the maximum amount in LCY that the user in the **User ID** field can approve for purchase quotes.<br /><br /> To use this field, you must select the **Approver Chain** option in the **Approver Limit Type** field in the **Workflow Response** window.|  
    |**Unlimited Request Approval**|Specify that the user in the **User ID** field can approve all purchase quotes regardless of their amount.<br /><br /> If you select this check box, then you cannot fill the **Request Amount Approval Limit** field.|  
    |**Substitute**|Select the user ID of the user who must approve requests made by the user in the **User ID** field if the user in the **Approver ID** is not available. **Note:**  The substitute can either be the user in the **Substitute** field, the direct approver, or the approval administrator, in that order of priority. For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).|  
    |**Email**|Specify the email address of the user in the **User ID** field.|  
    |**Approval Administrator**|Specify the user who has rights to unblock approval workflows, for example, by delegating approval requests to new substitute approvers and deleting overdue approval requests.|  

    > [!NOTE]  
    >  The behavior of **Approver Limit Type** field only applies to application areas where limits can be defined, namely sales and purchase approvals. Any other type of approval where limits do not apply will always behave as described for the **Direct Approver** option.  

3. To test the approval user setup, choose the **Approval User Setup Test** action.  
4. Repeat steps 2 and 3 for every user who you want to set up as an approval user.  

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md)   
[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)   
[How to: Create Workflows](across-how-to-create-workflows.md)   
[Setting Up Workflows](across-set-up-workflows.md)   
[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Workflow](across-workflow.md)   
