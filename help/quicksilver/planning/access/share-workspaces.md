---
title: 共享工作区
description: 在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 3550d7addcc0bb790f15d141d9470e0b75f940a6
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 1%

---

# 共享工作区

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中工作时，您可以与其他人共享工作区以确保协作。

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。 有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。


## 访问要求

+++ 展开以查看访问要求。

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
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p>
<p>您的组织必须载入到Adobe Unified Experience，用户才能通过权限请求向工作区请求和授予权限。 </p> 
<p>必须将用户添加到Adobe Admin Console才能获得Workfront Planning工作区的权限。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
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
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning区域的布局模板。</p>
<p><span class="preview">在预览环境中，标准用户和系统管理员默认启用Planning区域。</span></p></td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关共享工作区的注意事项

* 有关在Workfront Planning中共享对象的一般信息，另请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
* 您可以与组织内的用户、团队、角色、组或公司共享工作区。
* 除了团队、组、公司和职位角色之外，您只能与已添加到Adobe Admin Console的用户共享。
* 您无法与组织外部的用户共享工作区。
* 共享工作区时，也将共享与工作区关联的所有记录类型、记录和字段。
* 共享工作区时，视图不共享。 您必须单独共享视图。

<div class="preview">

* Workspace权限在记录类型上显示为继承权限。

</div>

## 共享对工作区的权限

以下用户可以与其他用户共享工作区：

* 系统管理员可以共享所有工作区，包括他们未创建的工作区。
* 所有其他用户只能共享他们对其具有管理权限的工作区。

要与他人共享工作区，请执行以下操作：

{{step1-to-planning}}

1. 打开要共享的工作区，然后单击屏幕右上角的&#x200B;**共享**。

   工作区右上方的![共享按钮](assets/share-button-on-workspace-top-right.png)

1. 在&#x200B;**授予此工作区的访问权限**&#x200B;字段中，开始键入用户、组、团队、公司或工作角色的名称，然后在列表显示该名称时单击该名称。

   ![与组共享UI](assets/sharing-ui-with-groups.png)

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

     ![访问请求的应用程序内通知](assets/in-app-notification-for-access-request.png)
   * 电子邮件通知

     ![访问请求的电子邮件通知](assets/email-notification-for-access-request.png)
1. （视情况而定）在Workfront的通知区域中，单击应用程序内通知
或
在电子邮件通知中，单击&#x200B;**查看所有通知**，然后单击列表中的通知。

   显示&#x200B;**待处理访问请求**&#x200B;框。

   ![通知列表审批框](assets/notifications-list-approval-box.png)

1. （可选）对于要批准其权限的用户，从用户名右侧的下拉菜单中选择以下选项之一：
   * **视图**
   * **参与**
   * **管理**
1. 选择要批准或拒绝权限的用户，然后单击&#x200B;**全部批准**&#x200B;或&#x200B;**全部拒绝**。
1. 单击&#x200B;**待处理访问请求**&#x200B;左侧的左箭头，然后单击&#x200B;**保存**。

   如果您批准了请求，则用户将添加到工作区的共享框中。 请求权限的用户会收到一封电子邮件，确认其请求已被批准。<!--will they also get an in-app notification??-->


## 删除对工作区的权限


{{step1-to-planning}}

1. 打开要删除权限的工作区，然后单击屏幕右上角的&#x200B;**共享**。
1. 单击与您共享工作区的实体名称右侧的下拉菜单，然后单击“**删除**”。
1. 单击&#x200B;**保存**。

   被删除的用户不再具有对工作区或其对象的访问权限。
