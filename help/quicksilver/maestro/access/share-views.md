---
title: 共享视图
description: 在使用Adobe Workfront规划时，您可以与他人共享视图以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live-->

# 共享视图

{{maestro-important-intro}}

在Adobe Workfront Planning中使用记录时，您可以与其他人共享视图以确保协作。

向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。

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
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> Adobe Workfront计划没有访问控制 </p>  
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

## 共享对视图的权限

您可以共享您创建的视图或您对其具有管理权限的视图。

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

1. 在 **授予查看权限** 字段中，开始键入用户或组的名称，然后在列表中显示该名称或组时单击该名称。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 管理

     有关权限级别以及用户可以在每个级别执行的操作的信息，请参阅 [在Adobe Workfront Planning中共享权限概述](../access/sharing-permissions-overview.md).

     <!--System administrators always receive Manage permissions to views shared with them.-->

1. 单击 **复制链接** 以将指向视图的链接复制到剪贴板。
1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。
1. 单击&#x200B;**保存**。

## 删除视图的权限

{{step1-to-maestro}}

1. 打开要共享其视图的工作区，然后单击记录类型卡片。 这将打开记录类型页面。
1. 在视图下拉菜单中，将鼠标悬停在要共享的视图上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 视图名称的右侧，然后单击 **共享**.
1. 查找要删除的用户或组，然后单击 **移除** 用户或组名称右侧的“权限”下拉菜单中。
1. 单击 **保存**.
属于已删除组的用户或用户不再具有查看权限。 对于已从访问视图中删除的用户，不会有任何通知。
