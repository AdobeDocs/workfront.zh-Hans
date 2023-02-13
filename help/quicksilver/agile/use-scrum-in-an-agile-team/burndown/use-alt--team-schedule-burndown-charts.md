---
product-area: agile-and-teams
navigation-topic: burndown
title: 为燃耗图使用备用团队计划
description: 在中定义的计划 [!DNL Adobe Workfront] 通过从燃耗中排除休息天数（周末和节假日）来影响燃耗图。
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 为燃耗图使用备用团队计划

在中定义的计划 [!DNL Adobe Workfront] 通过从燃耗中排除休息天数（周末和节假日）来影响燃耗图。

默认情况下，燃耗图使用默认计划。 除了默认计划之外，敏捷团队还可以选择使用替代计划，以纳入特定于团队的非工作日。 然后，此备用计划将反映在分配给团队的任何小版本的燃尽图中。 备用计划仅影响燃耗图。 (有关默认计划以及 [!DNL Workfront] 管理员可以创建特定于团队的计划，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

燃耗图不考虑部分天数。 例如，如果您的团队每周五工作4小时，则在燃耗图中将其表示为一整天。

有关使用燃耗图的详细信息，请参阅 [敏捷燃耗图概述](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 为燃耗图使用备用团队计划

1. 确保 [!DNL Workfront] 管理员已创建备用计划，如 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。

1. 选择要管理的敏捷团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 计划]** 区域，从下拉菜单中选择新计划。

1. 单击 **[!UICONTROL 保存更改]**.
