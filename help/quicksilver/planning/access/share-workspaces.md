---
title: 共享工作区
description: 在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1e62d5c7eff86432b4914793d75cdf4f835f3d5d
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 1%

---


# 共享工作区

{{planning-important-intro}}

在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。 有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。


## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具备以下条件才能访问Workfront Planning：

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包含的内容的更多信息，请参阅<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront定价和打包</a>。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>您的组织必须登记到AdobeUnified Experience，用户才能通过权限请求向工作区请求和授予权限。 </p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>管理工作区的权限</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--

OLD: 
 
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## 共享对工作区的权限

以下用户可以与其他用户共享工作区：

* 系统管理员可以共享所有工作区，包括他们未创建的工作区。
* 所有其他用户只能共享他们对其具有管理权限的工作区。

要与他人共享工作区，请执行以下操作：

{{step1-to-planning}}

1. 打开要共享的工作区，然后单击屏幕右上角的&#x200B;**共享**。

   ![](assets/share-button-on-workspace-top-right.png)

1. 在&#x200B;**向**&#x200B;授予工作区访问权限字段中，开始键入用户或组的名称，然后当该名称或组显示在列表中时单击它。

   ![](assets/sharing-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 参与
   * 管理

     有关权限级别以及用户可以针对每个级别执行的操作的信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
1. 单击&#x200B;**复制链接**&#x200B;以将指向工作区的链接复制到剪贴板。
1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问工作区。
1. 单击&#x200B;**保存**。

## 通过权限请求向工作区授予权限

如果用户访问指向工作区的链接，但无权访问该工作区，则可以请求对该工作区的权限。 所有对工作区具有“管理”权限的用户都会收到权限请求，并且可以授予或拒绝权限。

1. （视情况而定）如果您是工作区的管理员，则可能会收到其他用户发出的访问以下区域中的视图的请求：

   * 应用程序内通知
     ![](assets/in-app-notification-for-access-request.png)
   * 电子邮件通知
     ![](assets/email-notification-for-access-request.png)
1. （视情况而定）在Workfront的通知区域中，单击应用程序内通知
或
在电子邮件通知中，单击**查看所有通知**，然后单击列表中的通知。

   显示&#x200B;**待处理访问请求**&#x200B;框。

   ![](assets/notifications-list-approval-box.png)

1. （可选）对于要批准其权限的用户，从用户名右侧的下拉菜单中选择以下选项之一：
   * **视图**
   * **Contribute**
   * **管理**
1. 选择要批准或拒绝权限的用户，然后单击&#x200B;**全部批准**&#x200B;或&#x200B;**全部拒绝**。
1. 单击&#x200B;**待处理访问请求**&#x200B;左侧的左箭头，然后单击&#x200B;**保存**。

   如果您批准了请求，则用户将添加到工作区的共享框中。 请求权限的用户会收到一封电子邮件，确认其请求已被批准。<!--will they also get an in-app notification??-->


## 删除对工作区的权限


{{step1-to-planning}}

1. 打开要删除权限的工作区，然后单击屏幕右上角的&#x200B;**共享**。
1. 单击用户或组名称右侧的下拉菜单，然后单击“**删除**”。
1. 单击&#x200B;**保存**。

   属于已删除组的用户或用户无权再访问工作区或其对象。