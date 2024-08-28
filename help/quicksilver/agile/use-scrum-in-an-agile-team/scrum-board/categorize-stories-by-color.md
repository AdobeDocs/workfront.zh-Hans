---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: 在Scrum展示板上按颜色分类故事
description: Scrum展示板故事的默认颜色关联因故事板位于开发周期还是项目上而异。
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 在[!UICONTROL Scrum]展示板上按颜色分类故事

## 更改文章的默认颜色关联

根据故事板位于开发周期还是项目上，故事的默认颜色关联会有所不同：

* **[!UICONTROL 迭代]**：在迭代中，故事板图块会根据与故事关联的项目进行颜色编码。 （每个项目都会在故事板上任意指定一种颜色。） 您可以更改每个Agile团队的默认行为。 开发周期上Agile文章的颜色可以与项目（默认）、文章优先级、所有者或自由格式绑定。 有关详细信息，请参阅[配置Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)一文中的[配置Agile故事板上的故事如何使用颜色指示器](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4)。

* **[!UICONTROL 项目]**：在项目中，任何子任务均与父任务的颜色匹配，因此任何给定泳道中所有故事的颜色均相同。 如果任务没有任何子任务或没有父任务，则颜色在创建时随机分配给任务。 您可以通过修改敏捷视图来更改此默认行为。 项目上的Agile文章的颜色可以与父文章（默认）、文章优先级、所有者或自由格式绑定。 有关详细信息，请参阅 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)中的[视图概述中的[创建或自定义[!UICONTROL Agile]视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [！UICONTROL Standard]</p> 
   或
   <p>当前： [！UICONTROL Work]或更高版本</p> </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自由格式时更改文章的颜色

如果已配置Agile团队设置，将[!UICONTROL 将卡片颜色关联到]选项设置为[!UICONTROL 自由表单]，则用户可以手动更改单个文章图块的颜色。 这对于传达对团队或组织非常重要的其他类型的信息可能很有用：

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

1. 在左侧面板中，选择&#x200B;**[!UICONTROL 迭代]**&#x200B;以选择特定迭代，或选择&#x200B;**[!UICONTROL 当前迭代]**。
1. 将鼠标悬停在故事拼贴顶部的彩色横幅上。

   ![](assets/agile-story-color1-nwe-350x140.png)

1. 单击&#x200B;**[!UICONTROL 更改颜色]**，然后选择所需的颜色。

   ![](assets/agile-story-color2-nwe-350x138.png)
