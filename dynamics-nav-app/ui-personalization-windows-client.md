---
title: Personalizing Pages in the Dynamics Windows Client
description: Learn how to customize the user interface to suit your way of working.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: "dynamics-nav-2018"
---
# Personalizing Your Workspace in the Dynamics Windows Client
You can personalize, or customize, your workspace to suit your work and preferences by changing pages so that they display only the information you need, where you need it. The personalization changes that you make will only affect what you see, not what other users see. You can personalize many parts of the user interface (UI), including which actions to include on the ribbon, how fields are positioned on FastTabs or in FactBoxes, and which menu items to include in the navigation pane.

> [!NOTE]  
> You can also personalize pages by using the [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. To learn how personalization works between the two clients, see [Personalization Overview](ui-personalization-overview.md).
 
## How to personalize your workspace
You perform most of the personalization work by using the **Customize** feature, which you can access from practically all types of pages by doing the following:

1.  Open the page that you want to personalize.
2.  In the top left, choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, choose **Customize**, and then select one of the customization options.

There are also some basic UI changes, such as adjusting the size of any window or expanding the width of columns, which you do directly on the page, outside of the **Customize** option.

## General information
While customizing the UI, it is a good idea to keep these points in mind: 

-   You can record multiple customizations of the same page based on different access points to the page. For example, the Sales Orders window can be customized to look different when it is opened from the Customer Card window than when it is opened from the Sales Order Processor Role Center. The point from which you access the page to be customized is recorded in that specific page customization. Accordingly, there may be multiple page-customization records in the database, as you can see in the **Delete User Personalization** window.

-   The application can be configured to show and hide user interface (UI) elements (such as fields, FatTabs, and FactBoxes)lbased on your license or permissions. You will only be able to view and customize elemnts fields that you have permission to.

## Customize Ribbons
The ribbon provides you access to several actions. By customizing the ribbon, you can optimize it for your work processes and preferences. For example, if you frequently use the **Dimensions** window, you can add the **Dimensions** action to the **Process** actions group. You can also remove actions that you never use for better overview.  
  
You can perform the following tasks to customize ribbons on pages:  
  
-   Add, rename, or remove tabs, groups, actions, and menus.  
-   Change the order of actions.  
-   Restore the ribbon to its default setting.  
  
### To customize a ribbon
1. Open the page that you want to change.
2. In the top left, choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, choose **Customize** , and then **Customize Ribbon**.

The **Organize actions in the ribbon** dialog box is divvided into two panes. The **Available actions** pane lists all the actions that you can choose to add to the page. The **Show actions in this order** pane shows the structure of all the actions currently shown on the page.

-   Root-level items define tabs.

    -   Second-level items define a group in a tab.

        -   Third-level item define a menu of actions in a group

### Add a group
Select the tab under which you want the group, and then select **Create Group**. You cannot add a group under a menu.

### Add a menu
Select the group under which you want the menu, and then select **Create Menu**. You can only add a menu to a group or another menu. 

#### Add an action
Select it in the **Available actions** pane, choose **Add** to add it to the **Show actions in this order** pane, then use the **Move Up** and **Move Down** buttons to place it where you want it.

You cannot add an action to a tab; only to a group or menu.

###  Limitations and recommendations 
Be aware of the following limitations when you customize the ribbon:  
  
-   System tabs or groups such as **Home** or **New** cannot be moved or renamed. The position of some groups, such as **New Document** is fixed.  
-   Actions or groups that have dynamic visibility cannot be added or removed. 
-   You can only create menus inside groups, not inside tabs.  
-   You can nest a menu within another menu, but this is not recommended.  
-   If you see unexpected behavior with groups and actions after having customized the ribbon, do the following:  
    
    1.  Empty, but do not delete, the group where the problem occurs.  
    2.  Close the dialog using the **OK** button.  
    3.  Open the dialog again and re-add the actions to the group.  

> [!IMPORTANT]  
>  Any customization that alters the ribbon could affect the guidance provided in the [!INCLUDE[navnow_md](includes/navnow_md.md)] Help, because navigation steps in Help may refer to a different ribbon layout.

## Customize FastTabs
FastTabs help organize information about pages into simple, manageable groups. You can customize FastTabs on pages so that they support your workflow. For example, you may want to show fewer FastTabs or hide specific fields on FastTabs. You can also promote the most important fields to be included in the FastTab headers when the FastTabs are collapsed.  

### To customize a FastTab  
  
1.  Open the page that you want to change.
2.  Choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, select **Customize**, and then choose **Customize This Page**.  
3.  In the **Customize <Page Name>** dialog box, choose **FastTabs**.  
  
### Add, move, or remove FastTabs
The **Show FastTabs in this order** box contains the FastTabs that are currently on the page, and the order in which they are displayed. Use the **Add**, **Remove**, and **Move Up** and **Move Down** buttons to make changes.

### Show and hide fields on FastTabs
In **Show FastTabs in this order box**, select the FastTab that you want to change, and then choose **Customize FastTab**. Use the buttons to customize the fields you want to display and their order on the page.

Set the **Importance** as follows:
-   If you want to display the field in the FastTab header when the FastTab is collapsed, set this to **Promoted**.
- If you want the field to be hidden unless the user chooses the **Show More Fields** action on the FastTab, set this to **Additional**.
-   **Standard** is the default or normal setting.

### Set up field for Quick Entry 
Select the **Quick Entry** check box to add the field to the quick entry field list. When you work on the page, and press the Enter key in a field, the pointer jumps to the next field that is set to be a Quick Entry field. 

## Customize FactBoxes
You use FactBoxes to see information that relates to the record that you have selected in the list or opened in a task page. You can select which FactBoxes to display in your FactBox pane. You can also customize FactBoxes to display only the fields that you need.  
  
### To show or hide the FactBox pane
FactBoxes are contained in a FactBox pane, which you can choose to show or hide on a page basis. This enables you to easliy hide multiple FactBoxes without having to remove them individually. 

1.  Open the page that you want to change. 
2.  Choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, select **Customize**, and then choose **FactBoxes**. A check mark indicates that the FactBox pane is displayed.  

### To customize the FactBox pane  
1.  Open the page that you want to change. 
2.  Choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, select **Customize**, and then choose **Choose FactBoxes**.  
    
### Add a FactBox  
  
Select the FactBox that you want to add to the FactBox pane in the **Available FactBoxes** box, and then choose the **Add** button.  
  
### Remove a FactBox  
  
In the **Show FactBoxes in this order** box, select the FactBoxes , and then **Remove** button.   
  
### Change the order of the FactBoxes  
  
In the **Show FactBoxes in this order** box, select the FactBox that you want to move, and then choose the **Move Up** or **Move Down** buttons until it is positioned where you want it.  
  
### Change the fields in a FactBox  
  
1.  In the **Show FactBoxes in this order** box, select the FactBox, and then choose **Customize Part**.  
  
2.   The **Available fields** box list all the fields that you can choose from. The **Fields shown** box shows all the fields that are currently displayed in the FactBox. Use the buttons to add, remove, and move the fields.   


## Customize Columns in a List or on Document Lines
To get a better overview of the information that you need, you can customize list pages and card pages by adding or removing columns in the grids, rearranging columns, and adding a freeze pane.  
  
### To add, remove, and arrange columns  
  
1.  You can add, remove, or rearrange columns two ways:

    -   Choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, choose **Customize**, and then **Choose Columns**.
    -   Right-choose a column header and then choose **Choose Columns**.

2.  In the **Choose wich columns to show in list** dialog boxThe **Available columns** pane contains columns that are hidden. The **Show columns in this order** pane contains columns that are shown. Use the **Add** and **Remove** buttons to move columns from one field to the other. Use the **Move Up** and **Move Down** buttons to position the columns. 

>[!TIP]
>Select the **Quick Entry** check box to add the field to the quick entry field list. When you work on the page, and press the Enter key in a field, the pointer jumps to the next field that is set to be a Quick Entry field. 

### To set the freeze pane
A list can have many columns, which can force you to scroll horizontally to see all the columns. There might be some columns that you always want to display even as you scroll. To achieve this, you can add a vertical freeze pane to restrict some columns from scrolling. This enables you to ensure that only less important columns move when you scroll.

To set the freeze pane, select the column after which you want the freeze pane to start, and then choose **Add Freeze Pane**.

## Customizing the Navigation Pane
The navigation pane displays a menu of links to different list pages. Links are grouped under root-level buttons. 

### To customize the navigation pane  
  
Choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, choose **Customize**, and then choose **Customize Navigation Pane**.  
  
### Rename or Rearrange Buttons in the Navigation Pane  
In the **Customize Navigation Pane** dialog box, in the left pane, select the button that you want to move, rename, or remove and then choose the relevant button in the middle of the window.

You cannot move, rename, or remove the **Home** button. The **Departments** button can be removed from the navigation pane, but not renamed or moved. 
  
### Add a new menu button 
You can create a new root-level button, and then add a menu of links under the button to open different pages.

1. In the **Customize Navigation Pane** dialog box, choose **New**, and then type a name in the **Name** field.
2.  Choose the **OK** button.

You can add links to the button.  
  
### Add a link to a button   
If you have permission to view a list, such as the sales order list, you can add a link to the list from a button in your navigation pane.  
  
1.  In the **Customize Navigation Pane** dialog box, in the **Navigation pane buttons** field, select the menu that you want to add the link to.  
  
2.  Choose the **Add** button.  
  
3.  Browse to the link that you want to add, and then choose the **OK** button.  
> [!TIP]
> If you find a link in the **Departments** pages, you can also add it to the navigation pane. For more information, see the section Adding a Link from Departments to Your Role Center.  
  
### Move or copy a link from one button to another  
  
1.  In the **Customize Navigation Pane** dialog box, in the **Navigation pane buttons** field, select the menu where the link currently appears.  
  
2.  In the **Lists** pane, select the link that you want to move, and then choose **Move To** or **Copy To**  
  
3.  Select the navigation button that you want to add the link to, and then choose the **OK** button.  
  
### Rearrange the order of a links under a button  
  
1.  In the **Lists** pane, select the link that you want to move.  
  
2.  Use the **Move Up** and **Move Down** buttons to position the link.

## Adding Department Links to the Role Center
Sometimes you may find a link on a **Departments** page that you want to add to your Role Center for easy access. Where you can place the link on the Role Center depends the category of the link on the **Departments** page.

The following table describes the types of links in each category on the **Departments** pages, and where on your Role Center you can add them.  
  
|**Category**|**Contains**|**Add link to**|  
|------------------|------------------|---------------------|  
|Lists|List pages|**Home** button in navigation pane|  
|Tasks|Task pages, batch jobs, worksheets, journals|**Actions** tab in the ribbon|  
|Reports and Analysis|Reports, batch jobs, matrix windows|**Reports** tab in the ribbon|  
|Documents|Documents such as invoices and reminders|**Reports** in the ribbon|  
|Archive/History|Posted/finished documents, registers|**Home** button in navigation pane|  
|Administration|Setup windows|**Actions** tab in the ribbon|  
  
### To copy department links to your role center  
  
1.  Open the **Departments** page.  
  
2.  Right-choose the link, and then choose of the following (only one of these options will be available).  
  
    |**Select**|**To add the link to**|  
    |----------------|----------------------------|  
    |**Add to Navigation Pane**|The **Home** button in navigation pane on your Role Center.|  
    |**Add to Actions on Role Center Ribbon**|The **Actions** menu on the ribbon on your Role Center|  
    |**Add to Reports on Role Center Ribbon**|The **Reports** menu on the ribbon on your Role Center|  
  
3.  Confirm the message that appears.  
  
 The new link now appears in the menu to which you added it. However, you may want to move the link to another position in the menu. For example, if you added a link to the navigation pane, it will appear on the **Home** menu, but you can move it to another menu in the navigation pane. For more information, see the section Customizing the Navigation Pane. 

## Adding Charts to Role Centers and List Pages
When you have complex information, you may want to view a visual representation of the data to help see trends and make decisions. For example, you may want to monitor the balances per bank account for your company in a chart. You use the chart pane to visually show data from a list on the following types of pages:  
  
-   On your Role Center, where you can select from predefined generic charts.  
  
-   On a list page, where you can select to view a list as a chart.  
  
### To add a generic chart to your Role Center  
  
1.  On your Role Center, choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, select **Customize**, and then **Customize this Page**.  
  
2.  In the **Customize the Role Center** window, in the **Available parts** field, select **Chart Part**, and then choose **Add**.  
  
3.  Use the **Move Up**, **Move Down**, **Move Left**, and **Move Right** buttons to position the Chart Part on your Role Center.  
  
4.  Select the chart part, choose **Customize Part**.  
  
5.  In the **Customize Chart** window, select the predefined chart that you want to display, and then choose the **OK** button.  
  
### To view a list as a chart  
  
1.  On the list page, select the **Show as Chart** action.  
  
2.  Select a measure and a dimension to create a custom chart. To see additional information, select a secondary dimension. For example, to create a simple bar chart, select a dimension on the x-axis, and then select the **Dimension Count** dimension on the y-axis.  
  
> [!NOTE]  
>  By default, the chart pane is hidden because it can slow down performance. You should only show the chart when you must have the information.  
    
## Handling External Files and Automation Objects
When [!INCLUDE[navnow_md](includes/navnow_md.md)] receives an external file, you are presented with a dialog box. In addition to selecting what to do with the file, you can decide how to treat that file type next time it is received.  
  
When [!INCLUDE[navnow_md](includes/navnow_md.md)] is required to run an automation object, you are presented with a dialog box. You can decide whether that type of object should always or never be able to run.  
  
### To specify how to handle external files  
  
1.  When you are presented with the dialog box, clear the **Always ask before opening this type of file** check box if you want [!INCLUDE[navnow_md](includes/navnow_md.md)] to remember the option that you select in step 2. Next time that type file must be handled, the dialog box will not appear, and the file will be treated as specified in step 2.  
  
     Alternatively, select the **Always ask before opening this type of file** check box to always be presented with the dialog box when this file type is received.  
  
2.  Select **Open**, **Save**, or **Cancel**. The file is treated according to your selection.  
  
### To specify how to handle automation objects  
  
When you are presented with the dialog, select the **Always allow** check box if you want [!INCLUDE[navnow_md](includes/navnow_md.md)] to always run that type of automation object. Next time that type of automation object is required to run, the dialog box will not appear, and the automation object will run directly.  
  
Alternatively, select the **Never allow** check box to. Next time that type of automation object is required to run, the dialog box will not appear, and the automation object will not run.  

## <a name="CancelPersonalization"></a>Cancelling Personalization
Cancelling personalization can be divided into two categories:

-   Cancelling changes that you made by using the **Customize** feature.
-   Cancelling basic UI changes. 

### Cancel Customization
If you want to cancel all UI customization that you have ever made for a page under your current user logon or since you last canceled UI customizations, you can use the **Delete User Personalization** window. The layout of the page for which you delete your personalization is then reset to the default configuration for your profile.  
  
If you only want to cancel UI customization that you have made to a specific UI area on a page, such as the ribbon, you can use the **Restore Defaults** button in the **Customize** window. The layout of the specific UI area on that page is then reset to the default configuration for your profile.  
  
#### To cancel all UI customization that you have made to a page  
  
1.  In the **Search** box,, enter **Delete User Personalization**, and then choose the related link.  
  
2.  Select the page for which you want to cancel your UI customization, and then, on the **Home** tab, in the **View** group, choose **Delete**.  
  
> [!NOTE]  
>  All UI customization of the page that you have ever made under your current user logon or since you last used the **Delete User Personalization** window are canceled. The layout of the page is reset to the default configuration for your profile, as configured by the administrator or as installed with Microsoft Dynamics NAV.  
  
#### To cancel UI customization that you have made to a UI area on a page  
  
1.  From the page where you have customized a UI area, such as the ribbon, choose the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon") icon, choose **Customize**, and then choose **Customize <UI area>**.  
  
2.  At the bottom of the **Customize** window, choose the **Restore Defaults** button.  
  
> [!NOTE]  
>  All customization of the UI area that you have ever made for the page under your current user logon or since you last used the **Restore Defaults** button are canceled. The layout of the UI area on the page is reset to the default configuration for your profile, as configured by the administrator or as installed with Microsoft Dynamics NAV.

### Cancel Basic UI changes
You cancel basic UI changes by opening the **Reset User-Specified Settings** window from your Role Center.  
  
Basic UI changes include things like:
 -  Changing the size and position of any window.
 -  Changing the width of columns
 -  Changing the height of column headers.
 -  Sorting on columns in a list.
 -  Displaying lists as chart.
 -  Specifying how external files and automation objects are handled.  
 
#### To cancel basic UI changes
  
1.  Go to your Role Center.  
  
     On the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon"), choose **Customize**, and then choose **Reset User-Specified Settings**.  
  
2.  Choose the **Reset UI settings** button. Alternatively, choose the **Reset all** button to also cancel your decisions for handling files and automation objects.  
  
 All basic UI changes that you have ever made under your current user logon to [!INCLUDE[navnow_md](includes/navnow_md.md)], or since you last chose the **Reset UI settings** button, are canceled. The user interface is reset to the default configuration for your profile.  
  
#### To cancel your decision for running or saving external files  
  
1.  Go to your Role Center.  
  
     On the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon"), choose **Customize**, and then choose **Reset User-Specified Settings**.  
  
2.  Choose the **Reset file handling decision** button. Alternatively, choose the **Reset all** button to also cancel your view changes and decision for handling automation objects.  
  
 All decisions for default handling of file types that you have ever made under your current user logon, or since you last chose the **Client file access** button, are canceled and reset to the default configuration for your profile. The next time [!INCLUDE[navnow_md](includes/navnow_md.md)] receives an external file of any type, you are presented with a dialog with the options, **Save**, **Run**, and **Cancel**  
  
### To cancel your decision for handling automation objects  
  
1.  Go to your Role Center.  
  
     On the **Application** menu ![Application Menu button in menu bar](media/applicationmenuicon.png "ApplicationMenuIcon"), choose **Customize**, and then choose **Reset User-Specified Settings**.  
  
2.  Choose the **Reset automation decisions** button. Alternatively, choose the **Reset all** button to also cancel your view changes and decision for running or saving external files.  
  
 All decisions about how to run automation objects that you have ever made under your current user logon, or since you last chose the **Reset automation decisions** button, are canceled. The file handling behavior is reset to the default configuration for your profile.The next time [!INCLUDE[navnow_md](includes/navnow_md.md)] must run an automation object of any type, you are presented with a dialog with the options, **Always allow** and **Never allow**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## See Also
[Personalizing Your Workspace in the Dynamics Web Client](ui-personalization-user.md)  
[Personalization Overview](ui-personalization-overview.md)  


