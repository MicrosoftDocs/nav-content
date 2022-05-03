---
title: Personalizing Your Workspace Using the Dynamics NAV Web Client
description: Learn about the different options to customize the user interface to suit your way of working.
documentationcenter: ''
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalize page, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
author: jswymer
ms.author: jswymer
ms.prod: "dynamics-nav-2018"
---
# Personalizing Your Workspace Using the Dynamics NAV Web Client
<!--NAV in the Web client-->
You can customize, or *personalize*, your workspace to suit your work and preferences by changing pages so that they display only the information you need, where you need it. The personalization changes that you make will only affect what you see, not what other users see.

Depending on the type of page and what it includes, you can:

- Add, move, and remove fields.
- Add, move, and remove columns in a list.
- Change the freeze pane of columns in a list. The freeze pane locks one or more columns to the left side of a list so that are always present, even when you scroll horizontally.
- Move and remove Cues (tiles).
- Move and remove parts. Parts are subdivisions or areas on a page that contain things like multiple fields, another page, a chart, or tiles.  

## To personalize a page

1. In the upper-right corner, select your avatar, and then **Personalize**.

    The **Personalizing** banner appears at the top, which indicates that you can start making changes.

    ![Personalize mode](media/ui_personalize_mode_small.png "Personalize mode")

    > [!Note]  
    >   If you do not see the **Personalize** action, then personalization has not been enabled. Contact to your administrator or see [Enabling or Disabling Personalization in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)]](ui-personalization-manage.md#EnablePersonalization) for information about how to enable it.

2. Go to a page that you want to personalize.

   If there is a ![Personalization locked](media/personalization-lock-icon.png "Personalization locked") icon in the banner, see [Why the Page is Locked](ui-personalization-locked.md) for more details.

   If there is a ![Personalization blocked](media/ui_personalization_blocked.png "Personalization blocked") icon, you cannot personalize the page because it has been configured by an administrator.

3. Point to an area that you want to personalize, such as a field or column header in a list. Anything that you can personalize is immediately highlighted with an arrow or border.
   <!--
   -  If a component can be personalized, an arrow head (![Personalization indicator arrow left](media/ui_personalize_arrow_left.png "Personalization indicator arrow left") or ![Personalization indicator arrow down](media/ui_personalize_arrow_down.png "Personalization indicator arrow down")) appears.
   -   If the component is a part, the extent of the part is indicated by a border.
   -   The freeze pane in a list is indicated by a vertical line along the entire right-side of the last column of the freeze pane.
   -->

4. Use this table to help make changes:
       <table>
       <tr><th>What do you want to do</td><th>How to do it</th></tr>
       <tr><td>Move something, like a field, column in list, tile, or part</td><td> Point anywhere on what you want to move, and drag it to its new location. The location is indicated by either a thick horizontal or vertical line.</td></tr>
       <tr><td>Remove something</td><td>Select the arrowhead, and choose <b>Remove</b>. </td></tr>
       <tr><td>Add a field or column</td><td>In the <b>Personalizing</b> banner, choose <b>More</b>, and then choose <b>Field</b>.<br /></br>The <b>Add Field to Page</b> pane opens on the right. It lists the fields that you can add to the page. Fields marked as <b>Placed</b> are already on the page. Fields marked as <b>Ready</b> are not currently on the page.<br /></br>To add a field, drag it from the pane to the location that you want it. The location is indicated by either a thick horizontal or vertical line.</td></tr>
       <tr><td>Change the freeze pane in a list to another column</td><td>Select the arrowhead of the column that you want as the last column of the freeze pane, and then choose <b>Set Freeze Pane</b>.<br /><br/>If you want to set the freeze pane back to its original designed location, select the arrowhead for the current freeze pane column, and choose <b>Clear Freeze Pane</b>. Note: You cannot remove original freeze pane. There will always be a freeze pane that includes at least one column.</td></tr>
     </table>

   > [!IMPORTANT]  
   >   You cannot make changes to a list if the list is shown as tiles. You must first switch the page to the list view by selecting the ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon.

5. You can continue to make changes on the same page or move to another page. Your changes are automatically saved as you make them. When you are done, in the **Personalizing** banner, choose **Done**.

## Clearing Personalization to Change a Page Back to its Original Layout
At some point, you might want to undo all the personalization changes that you have made to a page over time so that page looks like it did originally. To do this, in the **Personalizing** banner, choose **More**, and then **Clear personalization**.

## Personalization in Detail
To help you better understand personalization, here are some pointers.  
-   When you make changes to a card page that you open from a list, the changes will take effect on all records that you open from that list. For example, let us say you open a specific customer from the **Customers list** window, and then personalize the page by adding a field. When you open other customers from the list, the field that you added will also be shown.
-   Changes that you make will take effect on all your Role Centers. For example, if you make a change to the Customer list when the Role Center is set to Business Manager, you will also see the change in the Customer list when Role Center is set to Sales Order Processor.
-   Changes to a page in a pane will take effect on the page where ever it is shown.  
-   You can only add fields and columns from a predefined list, which is based on the page. You cannot create new ones.

## See Also
[Dynamics 365 Business Central](/dynamics365/business-central/)  
[Personalization Overview](ui-personalization-overview.md)  
[Managing Personalization](ui-personalization-manage.md)  
[Working with [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[How to: Change the Role Center](change-role.md)  
[Configuring the User Interface (UI) for Users](admin-configure-user-interface.md)  
