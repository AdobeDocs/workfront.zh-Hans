---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 共享日历报告
description: 您可以与其他用户共享日历，也可以公开显示该日历，从而允许没有 [!DNL Adobe Workfront] 许可证的用户查看该日历。
author: Lisa
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: d90459cb4f6fb1960552f0ab174e963582312b5c
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 共享日历报告

您可以与其他用户共享日历，也可以公开显示该日历，从而允许没有[!DNL Adobe Workfront]许可证的用户查看该日历。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新建：浅色</p>
       <p>或</p>
       <p>当前：复查</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL View]或更高版本的[！UICONTROL Reports]、[！UICONTROL Dashboards]和[！UICONTROL Calendars]访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[！UICONTROL视图]或日历报表的更高权限，有权共享</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 与[!DNL Workfront]用户共享日历 {#share-a-calendar-with-workfront-users}

共享日历与共享其他对象类似。 有关在[!DNL Adobe Workfront]中共享对象的详细信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

与您共享的日历在日历名称旁显示一个星号(&#42;)。

要在[!DNL Workfront]内共享日历，请执行以下操作：

1. 转到要共享的日历。
1. 单击&#x200B;**[!UICONTROL 日历操作]**，然后单击&#x200B;**[!UICONTROL 共享]**。

1. 在&#x200B;**[!UICONTROL 将日历访问权限授予]**&#x200B;字段中，开始键入要共享日历的用户、团队、角色、组或公司的名称，然后单击该名称以将其显示在下拉列表中。\
   要了解有关设置权限的信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （可选）对要授予日历访问权限的每个用户、团队、角色或组重复步骤3。
1. 通过单击下拉菜单指定您在步骤3中添加的每个用户、团队、角色、组或公司的权限，然后选择要授予的权限级别：

   * **[!UICONTROL 查看]：**&#x200B;用户可以查看和共享日历。

     ![共享具有查看访问权限的日历](assets/calendar-share-view-permissions-350x249.png)

   * **[!UICONTROL 管理]：**&#x200B;用户拥有日历的完全访问权限，但缺少在访问级别授予的管理权限以及所有查看权限。

     ![通过“管理”访问权限共享日历](assets/calendar-share-manage-permissions-350x241.png)

     >[!NOTE]
     >
     >[!DNL Workfront]管理员和日历创建者可以从这些实体中删除权限。

1. （可选）根据用户的角色，您可以单击&#x200B;**[!UICONTROL 高级选项]**，然后单击&#x200B;**[!UICONTROL 共享]**&#x200B;以允许用户与其他用户共享日历。

   有关权限级别的详细信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （可选）要使日历对所有[!DNL Workfront]用户都可用，请单击齿轮图标，然后在下拉菜单中单击&#x200B;**[!UICONTROL 使此在系统范围内可见]**&#x200B;以使对象对所有[!DNL Workfront]用户都可用。\
   所有用户都可以根据您设置的权限查看对象。

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 与公共链接共享日历

您可以将日历设为公共日历，并与没有[!DNL Workfront]许可证的人共享链接。

1. 转到要共享的日历。
1. 单击&#x200B;**[!UICONTROL 日历操作]**，然后单击&#x200B;**[!UICONTROL 共享]**。

1. 单击齿轮图标，然后单击&#x200B;**[!UICONTROL 将此设为外部用户公开]**。
1. 单击&#x200B;**[!UICONTROL 复制链接]**。
1. 单击&#x200B;**[!UICONTROL 保存]**。

## 使用专用链接共享日历

您可以与[!DNL Workfront]用户共享专用日历链接。 用户在使用链接时需要登录才能查看日历。

1. 转到要共享的日历。
1. 单击&#x200B;**[!UICONTROL 日历操作]**，然后单击&#x200B;**[!UICONTROL 获取可共享链接]**。

1. 单击&#x200B;**[!UICONTROL 复制链接]**。

   >[!NOTE]
   >
   >[!DNL Workfront]用户必须具有日历的访问权限，才能通过链接访问日历。 要授予访问权限，请参阅[与 [!DNL Workfront] 用户共享日历](#share-a-calendar-with-workfront-users)。\
   >如果用户没有访问权限，则他们可以在将链接粘贴到浏览器后请求访问权限。
