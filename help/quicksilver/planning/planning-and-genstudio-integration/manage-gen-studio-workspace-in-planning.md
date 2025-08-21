---
title: 在GenStudio Planning中管理Adobe Workfront Workspace
description: 当您的公司同时购买了两款产品，并且您的GenStudio for Performance Marketing实例与公司的GenStudio实例集成时，Adobe Workfront Planning中会提供Workfront工作区。 您可以从Planning中查看GenStudio工作区，并更新两个系统中的信息。
hide: true
hidefromtoc: true
exl-id: d6140b05-26c3-4298-a2f9-53695aa021cb
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

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

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

当您的公司同时购买了两款产品，并且您的Adobe GenStudio for Performance Marketing实例与公司的GenStudio实例集成时，Adobe Workfront Planning中会提供Workfront工作区。

您可以从Planning中查看GenStudio工作区，并更新两个系统中的信息。

有关从GenStudio性能营销中使用和管理GenStudio工作区的信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

有关GenStudio与Workfront Planning集成的一般信息，请参阅[Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

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
<p>任何Adobe Workfront Workflow包</p>
<p>任何Adobe Workfront规划包</p>

</td> </tr>
<tr> 
   <td role="rowheader"><p>Adobe GenStudio包</p></td> 
   <td> 
<p>???GEN STUDIO是否有支持此功能的包???</p>

</td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 标准</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio许可证</p></td> 
   <td><p> ???GEN STUDIO是否需要特定的支持此功能的许可证???</p>
  </td> 
  </tr> 
  <tr> 
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>   
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
   <p>GenStudio的配置：???GENS需要什么访问级别???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限*</p></td> 
   <td>  
   <p>在Workfront规划中： </p>
   <ul>
   <li><p>向工作区和记录类型提供或更高权限  </p> </li> 
   <li><p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p></li>
   </ul>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何权限</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中创建权限以创建项目</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
*有关Adobe GenStudio for Performance Marketing的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

+++   

## 在Workfront Planning中管理GenStudio工作区的注意事项

* 贵组织必须先购买Adobe GenStudio for Performance Marketing，然后才能在Workfront Planning中查看GenStudio工作区。

* Workfront用户必须有权访问GenStudio，才能在Workfront Planning中查看GenStudio工作区。

* 您可以从Workfront Planning中更新GenStudio工作区的以下信息：

   * 编辑工作区设置<!--check to see if this is correct? is this editable or read only from Planning??-->
   * 编辑记录类型及其字段<!--check on this-->
   * 共享、编辑和添加视图
   * 添加新记录类型
   * 编辑、添加或删除记录

* 更新GenStudio工作区的工作区配置、记录类型、视图和字段与更新Workfront Planning工作区及其元素的方式相同。

<!--
## Manage GenStudio workspace from Workfront Planning

CAN YOU DO THIS?? 
- OPTIONS FROM THE WORKSPACE CARD ??
- OPTIONS FROM THE MORE MENU ON A WORKSPACE ??
-->

## 从Workfront Planning管理GenStudio记录类型

>[!NOTE]
>
>在管理GenStudio工作区之前，请参阅文章[Workfront规划与GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)。

1. 以也可访问GenStudio的用户身份登录Workfront。
1. 单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 计划]**。

   Workfront Planning主页将打开。

1. 单击&#x200B;**其他工作区**，然后找到具有由&#x200B;**系统**&#x200B;创建的指示且卡上有&#x200B;**GenStudio**&#x200B;标记的工作区。

   带有标记的![GenStudio工作区信息卡](assets/genstudio-card-with-tag-highlighted.png)

1. 单击&#x200B;**GenStudio工作区信息卡**&#x200B;以在Workfront Planning中打开GenStudio工作区。
1. 默认情况下，在Workfront Planning中创建和显示以下GenStudio记录类型：

   * 营销活动
   * 产品
   * 激活次数
   * 渠道
   * 区域

   GenStudio记录类型卡片上表明它们最初是在GenStudio中创建的。

   <!--check screen shot-->

   带有标记的![GenStudio记录类型卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)

1. 单击任何记录类型卡片以查看该类型的记录。

1. 执行下列操作之一：

   * 单击记录类型页面右上角的&#x200B;**共享**，然后单击以下任一项：
      * **复制视图链接**&#x200B;以共享记录类型的链接
      * **导出当前视图**以将其导出为CSV或Excel文件。
只能导出表格视图。<!--check on this later; is this true or are there more options in the Share button-->

   * 单击&#x200B;**+视图**&#x200B;以创建GenStudio记录类型的视图。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   * 单击&#x200B;**全屏**&#x200B;图标![以全屏模式打开全屏图标](assets/open-full-screen-icon.png)以全屏模式打开任何视图。

   * 从任何视图管理视图的元素。

     例如，您可以更改视图的过滤器、分组、排序和设置（如果可用）。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   * 在表或时间线视图中添加记录。

     您只能从头开始或通过导入CSV或Excel文件来创建记录。

     有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。

     记录在Workfront和GenStudio中均可见。

   * 编辑表视图中的内联记录，或单击记录以打开其详细信息页面。

     有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

   * 删除表视图中的记录。

     有关信息，请参阅[删除记录](/help/quicksilver/planning/records/delete-records.md)。

     如果从Workfront中删除已删除的记录，则可以从Workfront Planning的表视图回收站中恢复这些记录。

     有关信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/restore-deleted-records.md)

   * 将光标悬停在表格视图中的字段上可排序或隐藏该字段。

     >[!NOTE]
     >
     >仅当您在GenStudio中具有“管理”权限时，才能编辑字段的配置并添加更多字段。<!--check to see if this is true??-->
