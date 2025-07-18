---
title: 共享视图
description: 在使用Adobe Workfront Planning时，您可以与他人共享视图以确保协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 58d2bf9f14b9a3adf4bacfad58f1b9862aeaf247
workflow-type: tm+mt
source-wordcount: '1871'
ht-degree: 0%

---


# 共享视图

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中使用记录时，您可以与其他人共享视图以确保协作。

>[!IMPORTANT]
>
>* 向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。
>
>* 向视图授予权限不会更改查看记录的权限。 记录权限是通过共享工作区授予的。
>
>* 当您共享视图时，您会向他人授予访问视图所有元素的权限。 例如，当授予他们视图的管理权限时，他们可以修改分组、筛选器、排序或条形外观。


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## 访问要求

+++ 展开以查看访问要求。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>您的组织必须载入到Adobe Unified Experience，用户才能从权限请求请求向视图请求和授予权限。 </p>
<p>必须将用户添加到Adobe Admin Console才能获得Workfront Planning视图的权限。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
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
   <td>  <p>管理视图的权限</p>  
   <p>只有对工作区具有管理权限的用户才能公开共享视图。</p></td> 
  </tr>

</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享视图时的注意事项

* 您可以通过以下方式共享视图：

   * 在内部，包含Workfront用户、组、团队、公司和职位角色
   * 公开，使用Workfront之外的用户
   * 复制并共享视图的链接
   * 将其导出到Excel或CSV文件。 只能将表格视图导出到文件。 有关信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

* 有关在Workfront Planning中共享对象的一般信息，另请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
* 您可以向内部Workfront用户授予查看或管理视图的权限。

* 具有管理权限的用户可以修改视图设置、共享、复制或删除它。

* 您可以通过公共链接与组织外部的人员共享视图。

* 当您公开共享某个视图时，您公司以外的任何人都可以在限定时间内访问该链接，具体时间由到期日期指示。 无需登录即可查看共享视图。

* 组织外部有权访问视图的人员无法创建其他视图、编辑共享视图，或者在视图中添加、删除或编辑记录信息。

## 在内部共享对视图的权限

您可以在Workfront Planning中将您创建的视图或您拥有管理权限的视图与用户、组、团队、公司和职位角色共享。

>[!NOTE]
>
>系统管理员无法查看或共享他们自己未创建的视图。 他们只能访问或共享与其共享的视图。
>
>系统管理员只能拥有视图的管理权限。

{{step1-to-planning}}

1. 打开要共享其视图的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 在“视图”选项卡中，执行下列操作之一：

   * 将鼠标悬停在要共享的视图的选项卡名称上，然后单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。

     视图的![更多菜单](assets/more-menu-for-views-expanded-with-share-option.png)

   * 单击&#x200B;**共享** > **共享当前视图**

     ![具有记录类型和视图共享选项的“共享”按钮](assets/share-button-with-record-type-and-view-sharing-options.png)

   将打开&#x200B;**共享视图**&#x200B;框，默认情况下应选择&#x200B;**内部共享**&#x200B;选项卡。

1. （可选）在&#x200B;**谁有权访问**&#x200B;区域，从以下选项中选择：

   * **只有受邀人员才能访问**：您必须指定要与其共享视图的用户、组、团队、公司或工作角色。 这是默认选项。

   >[!NOTE]
   >
   >除了团队、组、公司和职位角色之外，您只能与已添加到Adobe Admin Console的用户共享。 您无法添加仅限Workfront的用户。 有关信息，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。


   * **工作区中的每个人都可以查看**：所有对工作区具有“查看”或更高权限的用户都可以访问该视图。

1. 在&#x200B;**授予此视图的访问权限**&#x200B;字段中，开始键入用户、组、团队、公司或工作角色的名称，然后在列表显示该名称时单击该名称。

   ![与组共享视图](assets/sharing-a-view-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 管理

     有关权限级别以及用户可以针对每个级别执行的操作的信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

     系统管理员始终获得对与其共享的视图的管理权限。

1. 单击&#x200B;**保存**。

   视图以人员图标![与他人共享的视图图标](assets/view-shared-with-others-people-icon.png)更新，表示该视图现在与其他用户共享。

   您共享该视图的用户会收到有关拥有其权限的应用程序内通知和电子邮件通知。

   >[!TIP]
   >
   >没有人员或全局图标的视图是您创建的视图，不会与他人共享。 非共享视图仅对您可见。

1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。

## 公开共享视图的权限

您可以将创建的视图或您拥有管理权限的视图与没有Workfront许可证以及可能属于您组织外部的人员共享。

>[!IMPORTANT]
>
>只有对工作区具有管理权限的用户才能公开共享工作区的视图。


要在Workfront Planning中公开共享视图，请执行以下操作：

{{step1-to-planning}}

1. 打开要共享其视图的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 在“视图”选项卡中，执行下列操作之一：

   * 将鼠标悬停在要共享的视图的选项卡名称上，然后单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。

   使用共享选项扩展的视图的![更多菜单](assets/more-menu-for-views-expanded-with-share-option.png)
   * 单击&#x200B;**共享** > **共享当前视图**

   将打开&#x200B;**共享视图**&#x200B;框。

1. 单击&#x200B;**公共共享**。

   ![视图的公共共享选项卡](assets/public-sharing-tab-for-views.png)

1. 启用&#x200B;**创建公共链接**&#x200B;设置。

   链接将变为可用。 这是一个公共链接。 共享后，拥有该链接的任何人（包括组织外部的人员）都可以访问记录类型页面，并查看该页面上的记录和字段。

1. 单击&#x200B;**复制链接**&#x200B;图标![复制链接视图](assets/copy-link-view.png)以将链接复制到剪贴板。

1. 手动输入日期，或使用&#x200B;**链接到期日期**&#x200B;字段中的日历为公共链接选择到期日期。 在选定日期后，将无法访问记录页面查看。

1. 单击&#x200B;**保存**。

   视图将更新为全局图标![高亮显示的公共共享视图图标](assets/public-shared-view-icon-highlighted.png)，以指示该视图是公共共享的。

   >[!TIP]
   >
   >没有人员或全局图标的视图是您创建的视图，不会与他人共享。 非共享视图仅对您可见。


1. （可选）将您复制的链接粘贴到电子邮件、聊天消息、文档或Workfront注释中，以便与其他人共享。

## 将链接复制到视图

您可以将指向视图的链接复制到剪贴板，然后将其包括在其他应用程序中或与其他人共享。

若要将链接复制到公共共享视图，请参阅本文中的[共享公共视图的权限](#share-permissions-to-a-view-publicly)部分。

本节介绍如何在内部共享视图。

>[!IMPORTANT]
>
>首先，必须先与用户共享视图，然后才能共享指向视图的链接，以便用户查看该视图。


{{step1-to-planning}}

1. 打开要复制并共享链接的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 在视图的选项卡中，执行以下操作之一：

   * 将鼠标悬停在要共享的视图的选项卡上，单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**共享视图**&#x200B;框中的&#x200B;**共享** > **复制链接**。
   * 单击&#x200B;**共享视图**&#x200B;框中的&#x200B;**共享** > **复制视图链接** > **复制链接**。

   指向视图的链接已复制到剪贴板，并且您会在屏幕底部收到确认。

   您现在可以将链接粘贴到其他应用程序或发送给其他应用程序。

## 通过权限请求向视图授予权限

如果用户访问指向没有权限的视图的链接，则可以请求该视图的权限。 所有对视图具有“管理”权限的用户都会收到权限请求，并且可以授予或拒绝权限。

1. （视情况而定）如果您是视图的管理者，则可能会收到其他用户发出的访问以下区域中的视图的请求：

   * 应用程序内通知

     ![视图访问请求的应用程序内通知](assets/in-app-notification-for-access-request-for-view.png)
   * 电子邮件通知

     ![视图访问请求的应用程序内通知](assets/in-app-notification-for-access-request-for-view.png)
1. （视情况而定）在Workfront的通知区域中，单击应用程序内通知
或
在电子邮件通知中，单击&#x200B;**查看所有通知**，然后单击列表中的通知。

   显示&#x200B;**待处理访问请求**&#x200B;框。

   ![通知列表审批框](assets/notifications-list-approval-box.png)
1. （可选）对于要批准其权限的用户，从用户名右侧的下拉菜单中选择以下选项之一：
   * **视图**
   * **管理**
1. 选择要批准或拒绝权限的用户，然后单击&#x200B;**全部批准**&#x200B;或&#x200B;**全部拒绝**。
1. 单击&#x200B;**待处理访问请求**&#x200B;左侧的左箭头，然后单击&#x200B;**保存**。

   如果您批准了请求，用户将添加到视图的共享框中。 请求权限的用户会收到一封电子邮件，确认其请求已被批准。<!--will they also get an in-app notification??-->

## 删除视图的权限

{{step1-to-planning}}

1. 打开要停止共享其视图的工作区，然后单击记录类型卡片。 这将打开记录类型页面。
1. 在“视图”选项卡中，执行下列操作之一：

   * 将鼠标悬停在要共享的视图的选项卡名称上，然后单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。

   * 单击&#x200B;**共享** > **共享当前视图**

   将打开&#x200B;**共享视图**&#x200B;框。
1. 要删除视图的内部共享，请执行以下操作：

   1. 确保选中&#x200B;**内部共享**&#x200B;选项卡。
   1. 查找要删除的用户、组、团队、公司或工作角色，展开权限下拉菜单（位于与你共享视图的实体名称的右侧），然后单击&#x200B;**删除**。

1. 要删除视图的公共共享，请执行以下操作：

   1. 单击&#x200B;**公共共享**&#x200B;选项卡。
   1. 取消选择&#x200B;**创建公共链接**&#x200B;选项。

1. 单击&#x200B;**保存**。

   用户不再具有查看权限。 对于已从访问视图中删除的用户，不会通知他们不再具有此访问权限。
