---
title: "Personalizing Your Workspace - Overview"
description: Learn how to customize the user interface to suit your way of working.

documentationcenter: ''
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: "dynamics-nav-2018"
---
# Personalizing Your Workspace - Overview
You can customize, or *personalize*, your workspace to suit your work and preferences by changing the layout of pages so that they display only the information you need, where you need it. The personalization changes that you make will only affect what you see, not what other users see.

You can personalize your workspace by using the [[!INCLUDE[nav_windows_md](includes/nav_windows_md.md)]](ui-personalization-windows-client.md) and [[!INCLUDE[nav_web_md](includes/nav_web_md.md)]](ui-personalization-user.md). The personlization changes that you make will also be seen in the [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] and [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].

> [!NOTE]  
> The administrator in your company may have already customized your user interface to a role-specific layout for all users who have the same profile as you and use the same Role Center. Personalizations that you make to your workspace are saved under your user account, so they will be preserved even if an administrator rolls out a new set of role-specific layouts  in your company. For more information, see [Configuring the User Interface](admin-configure-user-interface.md).

## Comparing Personalization in the Dynamics NAV Windows and Web Clients
Depending on the page, you can personalize many parts of the user interface, such as what fields or columns are shown and where they are placed, what actions are included on the ribbon, and more. Many of these things you can do in both the Windows client and Web client. The following table provides an overview of the personalization capabilities in each client.

|  Personalize  | |  Windows client  |  Web client  |
|---------------|-|------------------|--------------|
|**Fields in FastTabs**| | | |
||Add, move, remove |x|x|
||Show in collapsed header|x||
||Hide under **Show more fields** action|x||
|**Lists or document lines** | | | |
||Add, move, remove columns  |x|x|
||Add, move, remove freeze pane  |x|x|
|**FactBoxes**| | | |
||Move, remove|x|x|
||Add|x||
||Add, move, remove fields|x|x|
|**Cues**| | | |
||Move, remove|x|x|
||Add |x||
|**Charts**| | | |
||Move, remove|x|x|
||Add|x| |
|Ribbon and actions||x||
|Navigation Pane||x||

Another difference is that when personalizing by using the Windows client, you can have various personalized versions of the same page, based on different access points to the page. For example, the **Sales Orders** page personalized to look different when it is opened from the **Customer Card** page than when it is opened from the **Sales Order Processor Role Center** page. When you personalize a page by using the Web client, there is only one personalized version per page, so the changes will be seen in the page no matter where you open it from.

##  <a name="PersonalizationWinWeb"></a>Working with Personalization Between the Dynamics NAV Windows and Web Client
Before you start personalizing pages, it is important to understand how the personalization between the Window client and Web client works. If you will only ever use either the Windows client or the Web client, this information is not so relevant. However, it becomes important if you begin to personalize pages using both clients or when transitioning from using the Windows client to using the Web client permanently.  

-   If you use the Windows client to personalize a specific page from the start, you will also see the personalization changes to the page in the [!INCLUDE[nav_web_md](includes/nav_web_md.md)] as well.

-   As long as you continue to use the Windows client to personalize the page, any personalization changes you make, will also take effect on the page in the Web client.

-   However, as soon as you start to personalize the page by using the Web client, the personalization for that page becomes separate between the two clients, and you will have a personalized version for each client. In the Web client, the previous personalizations on the page are cleared, which means that the page will return to its original layout, and you will essentially start personalizing the page from scratch. The previous personalizations in the Windows client are unchanged.

- From this point on, you will personalize the page in the Windows and Web client independent of each other, which means the page can potentially look different in each client. The Phone and Tablet clients will show the same page personalizations as the Web client.  

> [!Tip]  
>If you open the **Delete User Personalization** page, you can see all the pages that have been personalized by each user. The **Legacy Personalization** column gives you an indication as to whether the personalization was done in the Windows client or Web client. If there is a check mark in the column, the personalization was done in the Windows client (or in the Web client prior to [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## See Also
[Dynamics 365 Business Central](https://docs.microsoft.com/dynamics365/business-central/)  
[Personalizing Your Workspace in the Dynamics NAV Windows Client](ui-personalization-windows-client.md)  
[Personalizing Your Workspace in the Dynamics NAV Web Client](ui-personalization-user.md)  
[Managing Personalization](ui-personalization-manage.md)  
[Customizing Dynamics NAV](ui-customizing-overview.md)  
