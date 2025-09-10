---
title: 在GenStudio Planning中管理Adobe Workfront Workspace
description: 当您的公司同时购买了两款产品，并且您的GenStudio for Performance Marketing实例与公司的GenStudio实例集成时，Adobe Workfront Planning中会提供Workfront工作区。 您可以从Planning中查看GenStudio工作区，并更新两个系统中的信息。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 0%

---


<!--Better metadata, at publishing:
---
title: Manage the GenStudio Workspace in Adobe Workfront Planning
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can view the GenStudio workspace from Planning and update information in both systems.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

<!--MUST update the access requirements below - not complete!!!!!!!!!-->

# 在Adobe Workfront Planning中管理GenStudio工作区

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

当您的公司同时购买了两款产品，并且您的Adobe GenStudio for Performance Marketing实例与公司的GenStudio实例集成时，Adobe Workfront Planning中会提供Workfront工作区。

您可以从Planning中查看GenStudio工作区，并更新两个系统中的信息。

有关从GenStudio性能营销中使用和管理GenStudio工作区的信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

有关GenStudio与Workfront Planning集成的一般信息，请参阅[Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

>[!IMPORTANT]
>
>本文中描述的步骤说明了当您具有GenStudio工作区的“管理”权限时，如何从Workfront Planning中更新该工作区。
>&#x200B;> 当您对GenStudio工作区具有“贡献”权限时，并非所有功能都可用。
>
>如果贵公司拥有多个Workfront实例，则所有用户都将在Workfront Planning中获得GenStudio工作区的Contribute权限。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront包</p>
<p>任何规划包</p>

</td> </tr>
   <tr> 
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 标准</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing用户角色</p></td> 
   <td><p><ul><li>用于访问营销活动、产品和角色的任何GenStudio用户角色</li>
   <li>GenSudio System Manager访问激活 <!--and Events--></li></ul>
   有关信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">用户角色和权限</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  
   <p>在Workfront规划中： </p>
   <ul>
   <li><p>管理GenStudio工作区的权限以向GenStudio工作区添加新字段或记录类型</p></li>
   <li><p>向GenStudio工作区提供权限以在GenStudio工作区中添加、更新或删除记录</p> </li>  
   </ul>
   <p>任何用户都不能从Workfront Planning的GenStudio for Performance Marketing工作区中删除GenStudio记录类型或字段</p>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何权限</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中创建权限以创建项目</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

有关Adobe Workfront Planning访问权限的信息，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

有关Adobe GenStudio for Performance Marketing的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

+++   

## 在Workfront Planning中管理GenStudio工作区的注意事项

* 贵组织必须先购买Adobe GenStudio for Performance Marketing，然后才能在Workfront Planning中查看GenStudio工作区。

* 根据贵组织拥有的Workfront实例数量，您在Planning中自动对GenStudio工作区具有以下权限：

  <!--this table is also in the Get started article-->

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
      <tr> 
      <td role="rowheader"><p>一个Workfront实例</p></td> 
      <td> 
   <p>GenStudio工作区在您的Workfront Planning实例中可见</p>
   <p>Workfront管理员对Planning中的GenStudio工作区具有管理权限</p>
   <p>所有其他用户均具有在Planning中对GenStudio工作区的“参与”访问权限</p>
   </td> </tr>
      <tr> 
   <td> 
      <p> Workfront的多个实例</p> </td> 
      <td> 
      <p>GenStudio工作区在所有Workfront实例中均可见</p>
   <p>所有有权访问GenStudio for Performance Marketing和Workfront Planning的用户都拥有对Planning中的GenStudio的“贡献”权限</p> </td> 
   </tr>
      </tbody> 
   </table>

* 更新GenStudio工作区的工作区配置、记录类型、视图和字段与更新Workfront Planning工作区及其元素的方式相同。

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## 从Workfront Planning管理GenStudio工作区

>[!NOTE]
>
>在管理GenStudio工作区之前，请参阅文章[Workfront Planning与GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)以了解更多信息。
>

1. 以也可访问GenStudio的用户身份登录Workfront。
1. 单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 计划]**。

   Workfront Planning主页将打开。

1. 单击&#x200B;**其他工作区**，然后找到具有由&#x200B;**系统**&#x200B;创建的指示且卡上有&#x200B;**GenStudio**&#x200B;标记的工作区。

   带有标记的![GenStudio工作区信息卡](assets/genstudio-card-with-tag-highlighted.png)

1. 单击&#x200B;**GenStudio工作区信息卡**&#x200B;以在Workfront Planning中打开GenStudio工作区。
1. 默认情况下，在Workfront Planning中创建和显示以下GenStudio记录类型：

   * 营销活动
   * 产品
   * 角色
   * 激活
   * 渠道
   * 区域

   GenStudio记录类型卡片上表明它们最初是在GenStudio中创建的。

   <!--check screen shot-->

   带有标记的![GenStudio记录类型卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击以下任一项：

   * **编辑**

     有关信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。
     <!--* **Delete** - this will generate an error message, per Iskuhi, so don't document as an option/ possibility-->

     <!--For information, see [Delete workspaces](/help/quicksilver/planning/architecture/delete-workspaces.md). -->

1. 单击右上角的&#x200B;**共享**&#x200B;以与他人共享工作区。

   有关信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

1. 单击任何记录类型卡片以查看该类型的记录。

   要管理记录类型、视图和字段，请参阅本文中的[从GenStudio Planning管理Workfront记录类型](#manage-genstudio-record-types-from-workfront-planning)部分。


## 在Workfront Planning中从GenStudio工作区管理记录类型、视图和记录

>[!NOTE]
>
>在管理GenStudio工作区之前，请参阅文章[Workfront Planning与GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)以了解更多信息。
>

1. 转到Workfront Planning中的GenStudio工作区，然后打开记录类型页面，如本文中[从Workfront Planning管理GenStudio工作区](#manage-the-genstudio-workspace-from-workfront-planning)部分所述。

1. 单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击以下任一项：

   * **编辑**

     有关信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。
   * **管理自动化**

     有关信息，请参阅[配置Adobe Workfront计划自动化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。
   * **管理请求表单**

     您可以创建多个请求表单。 申请表将在Workfront的申请区域提供，您也可以公开或通过链接共享它们。

     有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

1. 要共享视图或记录类型，请执行以下操作：

   * 单击记录类型页面右上角的&#x200B;**共享**，然后单击以下任一项：
      * **共享记录类型**
有关信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。
      * **共享当前视图**
有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。
      * **复制视图链接**
指向视图的链接已复制到您的剪贴板中。
      * **导出当前视图**
有关信息，请参阅[从表视图](/help/quicksilver/planning/records/export-records-from-the-table-view.md)导出记录。

1. 要管理记录类型视图，请执行以下操作：

   * 单击&#x200B;**+视图**&#x200B;以创建GenStudio记录类型的视图。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   * 单击&#x200B;**全屏**&#x200B;图标![以全屏模式打开全屏图标](assets/open-full-screen-icon.png)以全屏模式打开任何视图。

   * 从任何视图管理视图的元素。

     例如，您可以更改视图的过滤器、分组、排序和设置（如果可用）。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

1. 要添加记录，请执行下列操作之一：

   * 从任何视图中单击&#x200B;**新建记录**&#x200B;以从头开始创建记录

   * 在表视图中使用Excel或CSV文件导入记录

   * 单击时间轴或日历视图中的任意位置以添加记录。

     有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

     记录在Workfront和GenStudio中均可见。

     >[!NOTE]
     >
     >您无法添加激活记录类型的记录。

1. 要编辑记录，请执行下列操作之一：

   * 编辑表视图中的内联记录

   * 单击任何视图中的记录以打开其详细信息页面。

     有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

     您在Planning中的GenStudio工作区中所做的更改会立即从GenStudio中可见。

1. 在表视图中选择记录，然后单击&#x200B;**删除**。

   有关信息，请参阅[删除记录](/help/quicksilver/planning/records/delete-records.md)。

   删除的记录会立即从GenStudio中删除。

   >[!TIP]
   >
   >已删除的记录可以从Workfront Planning的表视图“最近删除的框”中恢复。 从GenStudio中删除的记录也可以从Workfront Planning中最近删除的回收站恢复。

   有关信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/restore-deleted-records.md)

1. 单击表格视图右上角的+图标以创建以下内容：

   * 记录字段

     有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)

   * 记录连接

     有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)

     从GenStudio工作区创建的字段在以下区域可见：

      * Workfront Planning视图
      * Workfront Planning记录详细信息
      * GenStudio记录详细信息

     >[!TIP]
     >
     >在Workfront Planning中创建的字段在GenStudio的列表视图中不可见。

1. 将鼠标悬停在表视图中的字段上，然后单击下拉菜单以执行以下操作之一：

   * 按其排序
   * 隐藏它
   * 编辑其设置
     <!--* Delete it - not possible now, per Iskuhi; the link is there but it will generate an error-->

     <!--GenStudio-native fields are note removed from GenStudio. -->

     >[!NOTE]
     >
     >仅当您在GenStudio中具有“管理”权限时，才能编辑字段的配置并添加更多字段。

