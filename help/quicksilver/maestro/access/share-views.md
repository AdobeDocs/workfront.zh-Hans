---
title: 共享视图
description: 在使用Adobe Workfront Planning时，您可以与他人共享视图以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# 共享视图

{{planning-important-intro}}

在Adobe Workfront Planning中使用记录时，您可以与其他人共享视图以确保协作。

向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。

当您共享视图时，您会向他人授予访问视图所有元素的权限。 例如，当授予他们视图的管理权限时，他们可以修改分组、筛选器、排序或条形外观。


您可以与以下实体共享视图：

* Workfront用户
* Workfront组
<!--* Publicly, with users outside Workfront
-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> Adobe Workfront Planning没有访问控制 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td> <p>管理视图的权限</p>

</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅 <a href="/help/quicksilver/maestro/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## 共享对视图的权限 <!--internally-->

您可以共享您创建的视图或您拥有管理权限的视图 <!--with users or groups in Workfront-->.

>[!NOTE]
>
>系统管理员无法查看或共享他们自己未创建的视图。 他们只能访问或共享与其共享的视图。
>
>系统管理员只能拥有视图的管理权限。

{{step1-to-maestro}}

1. 打开要共享其视图的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 在视图选项卡中，将鼠标悬停在要共享的视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 视图名称的右侧，然后单击 **共享**.

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   <!--The Internal sharing tab should be selected by default.-->

1. （可选）从以下选项中进行选择以共享视图：

   * **只有受邀人员才能访问**：您必须指定要与其共享视图的用户或组。 这是默认选项。
   * **工作区中的每个人都可以查看**：所有对工作区具有“查看”或更高权限的用户都可以访问视图。

1. 在 **授予查看权限** 字段中，开始键入用户或组的名称，然后在列表中显示该名称或组时单击该名称。  <!--***********replace screen shot below when public sharing is released***********-->

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 管理

     有关权限级别以及用户可以在每个级别执行的操作的信息，请参阅 [在Adobe Workfront Planning中共享权限概述](../access/sharing-permissions-overview.md).

     系统管理员始终获得对与其共享的视图的管理权限。

1. 单击 **复制链接** 以将指向视图的链接复制到剪贴板。
1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。
1. 单击&#x200B;**保存**。

<!--
## Share permissions to a view publicly

You can share views you created or views you have Manage permissions to with people that do not have a Workfront license and who might be external to your organization. 

Consider the following when publicly sharing a Workfront Planning view: 

* You can share a public link to a record type page that displays in the view you are sharing.
* People accessing the record type with the public link you provide have View permissions to the record page. They cannot modify the view, the records, or any of the fields that are visible in the view. 
* The shared public link must have an expiration date after which the link is no longer accessible. 

To share a view publicly in Workfront Planning: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Click **Public sharing**.

1. Enable the **Create public link** setting.

   A link becomes available. This is a public link. When shared, anyone with the link, including people from outside your organization can access the record type page, and view records and fields on the page. 

1. Click the **Copy link** icon ![](assets/copy-link-view.png) to copy the link to your clipboard. 

1. Manually enter a date, or use the calendar in the **Link expiration date** field to select an expiration date for the public link. The record page view will not be accessible after the selected date. 

1. Click **Save**.

1. Paste the link you copied to an email, chat message, document, or in a Workfront comment to share it with others. 

-->


## 删除视图的权限

{{step1-to-maestro}}

1. 打开要停止共享其视图的工作区，然后单击记录类型卡片。 这将打开记录类型页面。
1. 将鼠标悬停在要删除共享的视图的选项卡名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **共享**.
1. 查找要删除的用户或组，然后单击 **移除** 用户或组名称右侧的“权限”下拉菜单中。
1. 单击 **保存**.
属于已删除组的用户或用户不再具有查看权限。 对于因访问视图而被移除的用户，不会通知他们已失去此访问权限。

<!--Replace the above instructions with the following when public sharing is released: 

{{step1-to-maestro}}

1. Open the workspace whose view you want to stop sharing, then click a record type card. This opens the record type page.
1. Hover over the tab name of the view you want to remove sharing from and click the **More** menu ![](assets/more-menu.png), then click **Share**.
1. To remove the internal sharing of a view, do the following: 

   1. Ensure the **Internal sharing** tab is selected.
   1. Find the user or group what you want to remove, expand the permissions drop-down menu to the right of the user's or group's name, then click **Remove**.

1. To remove the public sharing of a view, do the following: 

   1. Click the **Public sharing** tab.
   1. Deselect the **Create public link** option. 

1. Click **Save**.
   
   People no longer have access to the view. There is no notification for the users that have been removed from accessing the view that they no longer have this access.-->