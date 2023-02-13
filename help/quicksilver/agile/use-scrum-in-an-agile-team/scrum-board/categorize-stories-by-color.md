---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 按颜色在Scrum展示板上对文章进行分类
description: Scrum展示板文章的默认颜色关联会因文章展示板位于小版本还是项目而异。
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 在 [!UICONTROL Scrum] 展示板

## 更改文章的默认颜色关联

文章的默认颜色关联因文章展示板位于小版本还是项目而异：

* **[!UICONTROL 迭代]**:在迭代中，文章板图块会根据与文章关联的项目进行颜色编码。 （每个项目在文章板上被任意指定一种颜色。） 您可以为每个敏捷团队更改此默认行为。 小版本上敏捷文章的颜色可以与项目（默认）、文章优先级、所有者或自由形式绑定。 有关更多信息，请参阅 [配置如何在敏捷文章展示板上将颜色指示器用于文章](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) 在文章中 [配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL 项目]**:在项目中，任何子任务都与父任务的颜色相匹配，因此任何给定泳道中所有文章的颜色都相同。 如果任务没有子任务或没有父任务，则在创建任务时，会随机为任务分配颜色。 您可以通过修改敏捷视图来更改此默认行为。 项目中敏捷文章的颜色可以绑定到父文章（默认）、文章优先级、所有者或自由形式。 有关更多信息，请参阅 [创建或自定义 [!UICONTROL 敏捷] 视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [视图概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL Worker]或更高版本</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 使用自由形式时更改文章的颜色

如果已配置敏捷团队设置，则 [!UICONTROL 将卡片颜色与] 选项设置为 [!UICONTROL 自由格式]，则用户可以手动更改单个文章图块的颜色。 这对于传达对团队或组织而言非常重要的其他类型的信息非常有用：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

1. 在左侧面板中，选择 **[!UICONTROL 迭代]** 选择特定小版本，或选择 **[!UICONTROL 当前迭代]**.
1. 将鼠标悬停在文章图块顶部的彩色横幅上。

   ![](assets/agile-story-color1-nwe-350x140.png)

1. 单击 **[!UICONTROL 更改颜色]**，然后选择所需的颜色。

   ![](assets/agile-story-color2-nwe-350x138.png)
