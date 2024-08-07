---
title: 共享视图
description: 在使用Adobe Workfront Planning时，您可以与他人共享视图以确保协作。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%

---

<!--update the metadata and description when we turn this article live-->

# 共享视图

{{planning-important-intro}}

在Adobe Workfront Planning中使用记录时，您可以与其他人共享视图以确保协作。

>[!IMPORTANT]
>
>* 向工作区授予权限不会向其他用户授予对记录类型页面上的视图的权限。 您必须向记录类型页面中的各个视图授予权限才能与其他用户共享它们。
>
>* 向视图授予权限不会更改查看记录的权限。 记录权限是通过共享工作区授予的。
>
>* 当您共享视图时，您会向他人授予访问视图所有元素的权限。 例如，当授予他们视图的管理权限时，他们可以修改分组、筛选器、排序或条形外观。


您可以与以下实体共享视图：

* 内部，包含Workfront用户和组
* 公开，使用Workfront之外的用户

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

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
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>新增：标准</p>
   或
   <p>当前：计划 </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> Adobe Workfront Planning没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理视图的权限</p>  
   <p>只有对工作区具有管理权限的用户才能公开共享视图。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> <p>有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p> 
</td>
  </tr>
 </tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享视图时的注意事项

* 您可以向内部Workfront用户授予查看或管理视图的权限。

* 具有管理权限的用户可以修改视图设置、共享、复制或删除它。

* 您可以通过公共链接与组织外部的人员共享视图。

* 当您公开共享某个视图时，您公司以外的任何人都可以在限定时间内访问该链接，具体时间由到期日期指示。 无需登录即可查看共享视图。

* 组织外部有权访问视图的人员无法创建其他视图、编辑共享视图，或者在视图中添加、删除或编辑记录信息。

## 在内部共享对视图的权限

您可以在Workfront中将您创建的视图或您拥有管理权限的视图与用户或组共享。

>[!NOTE]
>
>系统管理员无法查看或共享他们自己未创建的视图。 他们只能访问或共享与其共享的视图。
>
>系统管理员只能拥有视图的管理权限。

{{step1-to-planning}}

1. 打开要共享其视图的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 在“视图”选项卡中，将鼠标悬停在要共享的视图上，单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**共享**。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   默认情况下应选择&#x200B;**内部共享**&#x200B;选项卡。

1. （可选）在&#x200B;**谁有权访问**&#x200B;区域，从以下选项中选择：

   * **只有受邀人员才能访问**：您必须指定要与其共享视图的用户或组。 这是默认选项。
   * **工作区中的每个人都可以查看**：所有对工作区具有“查看”或更高权限的用户都可以访问该视图。

1. 在&#x200B;**授予对**&#x200B;字段的查看访问权限，开始键入用户或组的名称，然后在列表中显示该名称或组时单击它。

   ![](assets/sharing-a-view-ui-with-groups.png)

1. 从下拉菜单中选择以下权限级别之一：
   * 查看
   * 管理

     有关权限级别以及用户可以针对每个级别执行的操作的信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

     系统管理员始终获得对与其共享的视图的管理权限。

1. 单击&#x200B;**复制链接**&#x200B;以将指向视图的链接复制到剪贴板。
1. 单击&#x200B;**保存**。

   视图以人员图标![](assets/view-shared-with-others-people-icon.png)更新，表示该视图现在与其他用户共享。

   >>
   >[!TIP]
   >>
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

1. 在“视图”选项卡中，将鼠标悬停在要共享的视图上，单击视图名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**共享**。

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. 单击&#x200B;**公共共享**。

   ![](assets/public-sharing-tab-for-views.png)

1. 启用&#x200B;**创建公共链接**&#x200B;设置。

   链接将变为可用。 这是一个公共链接。 共享后，拥有该链接的任何人（包括组织外部的人员）都可以访问记录类型页面，并查看该页面上的记录和字段。

1. 单击&#x200B;**复制链接**&#x200B;图标![](assets/copy-link-view.png)以将链接复制到剪贴板。

1. 手动输入日期，或使用&#x200B;**链接到期日期**&#x200B;字段中的日历为公共链接选择到期日期。 在选定日期后，将无法访问记录页面查看。

1. 单击&#x200B;**保存**。

   视图会以全局图标![](assets/public-shared-view-icon-highlighted.png)更新，以指示该视图已公开共享。

   >>
   >[!TIP]
   >
   >没有人员或全局图标的视图是您创建的视图，不会与他人共享。 非共享视图仅对您可见。


1. （可选）将您复制的链接粘贴到电子邮件、聊天消息、文档或Workfront注释中，以便与其他人共享。

## 删除视图的权限

{{step1-to-planning}}

1. 打开要停止共享其视图的工作区，然后单击记录类型卡片。 这将打开记录类型页面。
1. 将鼠标悬停在要删除共享的视图的选项卡名称上，单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**共享**。
1. 要删除视图的内部共享，请执行以下操作：

   1. 确保选中&#x200B;**内部共享**&#x200B;选项卡。
   1. 找到要删除的用户或组，展开该用户或组名称右侧的权限下拉菜单，然后单击&#x200B;**删除**。

1. 要删除视图的公共共享，请执行以下操作：

   1. 单击&#x200B;**公共共享**&#x200B;选项卡。
   1. 取消选择&#x200B;**创建公共链接**&#x200B;选项。

1. 单击&#x200B;**保存**。

   用户不再具有查看权限。 对于已从访问视图中删除的用户，不会通知他们不再具有此访问权限。