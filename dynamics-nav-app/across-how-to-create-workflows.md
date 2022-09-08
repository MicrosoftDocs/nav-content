---
    title: How to Create Workflows 
    description: You can create workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.
    
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
# How to: Create Workflows
You can create workflows that connect business-process tasks performed by different users. System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks. Requesting and granting approval to create new records are typical workflow steps.  

In the **Workflow** window, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event moderated by event conditions and a workflow response with response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.  

When you create workflows, you can copy the steps from existing workflows or from workflow templates. Workflow templates represent non-editable workflows that exist in the generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)]. The code for workflow templates that are added by Microsoft are prefixed with “MS-“, such as in “MS-PIW”. For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).  

If your business scenario requires workflow events or responses that are not supported, a Microsoft partner must implement them by customizing the application code.  
  
> [!NOTE]  
>  All notifications about workflow steps are sent through a job queue. Make sure that the job queue in your installation is set up to handle workflow notifications, and that the **Start Automatically From NAS** check box is selected. For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).  

## To create a workflow  
1. Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.  
2. Choose the **New** action. The **Workflow** window opens.  
3. In the **Code** field, enter a maximum of 20 characters to identify the workflow.  
4. To create the workflow from a workflow template, in the **Workflows** window, choose the **Create Workflow from Template** action. For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).  
5. In the **Description** field, describe the workflow.  
6. In the **Category** field, specify which category the workflow belongs to.  
7. In the **When Event** field, specify the event that must occur to start the workflow step.  

    When you choose the field, the **Workflow Events** window opens where you select from all the workflow events that exist.  
8. In the **Condition** field, specify one or more conditions that must be met before the event in the **When Event** field can occur.  

    When you choose the field, the **Event Conditions** window opens where you choose from a list of filter fields that are relevant as conditions for the event in question. You can add new filter fields that you want to use as event conditions. You set event condition filters just as you set filters on report request pages.  

    If the workflow event is the change of a specific field on a record, then the **Event Conditions** window opens with options to select the field and the type of change.  

    1.  To specify a field change for the event, in the **Event Conditions** window, in the **Field** field, select the field that changes.  
    2.  In the **Operator** field, select either **Decreased**, **Increased**, or **Changed**.  
9. In the **Then Response** field, specify the response that will follow when the workflow event occurs.  

     When you choose the field, the **Workflow Responses** window opens where you select from all workflow responses that exist and set response options for the selected response.  
10. On the **Options for the Selected Response** FastTab, specify options for the workflow response, by selecting values in the different fields that appear, as follows:  

    1.  To specify options for a workflow response that involves sending a notification, fill the fields as described in the following table.  

        |Field|Description|  
        |----------------------------------|---------------------------------------|  
        |**Recipient User ID**|Specify the user who the notification must be sent to. Note: This option is only available for workflow responses with a placeholder for a specific user. For workflow responses without placeholders for users, the notification recipient is typically defined by the approval user setup.|  
        |**Link Target Page**|Specify another page in [!INCLUDE[d365fin](includes/d365fin_md.md)] that the link in the notification opens instead of the default page.|  
        |**Custom Link**|Specify the URL of a link that is added to the notification in addition to the link to page in [!INCLUDE[d365fin](includes/d365fin_md.md)].|  
    2.  To specify options for a workflow response that involves creating an approval request, fill the fields as described in the following table.  

        |Field|Description|  
        |----------------------------------|---------------------------------------|  
        |**Due Date Formula**|Specify in how many days the approval request must be resolved from the date when it was sent.|  
        |**Delegate After**|Specify if and when an approval request will automatically be delegated to the relevant substitute. You can select to automatically delegate one, two, or five days after the date when the approval was requested.|  
        |**Approver Type**|Specify who the approver is, according to the setup of approval users and workflow users.<br /><br /> The following options exist:<br /><br /> -   **Salesperson/Purchaser** specifies that the user who is set up in the **Salespers./Purch. Code** field in the **Approval User Setup** window determines the approver. Approval request entries are then created according to the value in the **Approver Limit Type** field.<br />     For more information, see [How to: Set Up Approval Users](across-how-to-set-up-workflow-users.md).|  
        |**Show Confirmation Message**|Specify if a confirmation message is shown to users after they request an approval.|  
        |**Approver Limit Type**|Specify how approvers’ approval limits affect when approval request entries are created for them. A qualified approver is an approver whose approval limit is above the value on the request being made.<br /><br /> The following options exist:<br /><br /> 1.  **Approver Chain** specifies that approval request entries are created for all the requester’s approvers up to and including the first qualified approver.<br />2.  **Direct Approver** specifies that an approval request entry is only created for the requester’s immediate approver, regardless of the approver’s approval limit.<br />3.  **First Qualified Approver** specifies that an approval request entry is only created for the requester’s first qualified approver.<br />|  
    3.  To specify options for a workflow response that involves creating journal lines, fill the fields as described in the following table.  

        |Field|Description|  
        |----------------------------------|---------------------------------------|  
        |**General Journal Template Name**|Specify the name of the general journal template that the specified journal lines are created in.|  
        |**General Journal Batch Name**|Specify the name of the general journal batch that the specified journal lines are created in.|  

11. Choose the **Increase Indent** and **Decrease Indent** buttons to indent the event name in the **When** field to define the step’s position in the workflow.  
    1.  Indicate that the step is the next in the workflow sequence by indenting the event name under the event name of the previous step.  
    2.  Indicate that the step is one of more alternative steps that may start depending on its condition by placing the event name at the same indentation as the other alternative steps. Order such optional steps according to priority by placing the most important step first.  

    > [!NOTE]  
    >  You can only change the indent of a step that does not have a subsequent step.  

12. Repeat steps 7 through 11 to add more workflow steps, either before or after the step that you have just created.  
13. Select the **Enabled** check box to specify that the workflow will start as soon as the event on the first step of type **Entry Point** occurs. For more information, see [Using Workflows](across-use-workflows.md).  

> [!NOTE]  
>  Do not enable a workflow until you are sure that the workflow is completed and that the involved workflow steps can start.  

> [!TIP]  
>  To see relations between tables that are used in workflows, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and then enter **Workflow – Table Relations**.  

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md)   
[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md)   
[Setting Up Workflow Notifications](across-setting-up-workflow-notifications.md)   
[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)   
[How to: Delete Workflows](across-how-to-delete-workflows.md)   
[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Setting Up Workflows](across-set-up-workflows.md)   
[Using Workflows](across-use-workflows.md)   
[Workflow](across-workflow.md)      
