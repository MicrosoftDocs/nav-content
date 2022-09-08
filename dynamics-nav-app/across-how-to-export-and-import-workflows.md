---
    title: How to Export and Import Workflows 
    description: To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.
    
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
# How to: Export and Import Workflows
To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.  

 Another way to quickly create workflows is to create workflows from workflow templates. For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).  

 In the **Workflow** window, you create a workflow by listing the involved steps on the lines. Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options. You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code. For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).  

## To export a workflow  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.  
2.  Select a workflow, and then choose the **Export to File** action.  
3.  In the **Export File** window, choose the **Save** button.  
4.  In the **Export** window, select a file location, and then choose the **Save** button.  

## To import a workflow  
1.  Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.  
2.  Choose the **Import from File** action.  
3.  In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.  

> [!CAUTION]  
>  If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.  

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[How to: Create Workflows](across-how-to-create-workflows.md)   
 [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md)   
 [How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md)   
 [How to: Delete Workflows](across-how-to-delete-workflows.md)   
 [Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Setting Up Workflows](across-set-up-workflows.md)   
 [Using Workflows](across-use-workflows.md)   
 [Workflow](across-workflow.md)   
