---
product-area: agile-and-teams
navigation-topic: burndown
title: 将备用组计划用于燃尽图
description: 在中定义的时间表 [!DNL Adobe Workfront] 通过从燃尽中排除休息日（周末和节假日）来影响燃尽图。
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 将备用组计划用于燃尽图

在中定义的时间表 [!DNL Adobe Workfront] 通过从燃尽中排除休息日（周末和节假日）来影响燃尽图。

默认情况下，燃尽图使用默认计划。 除了默认计划之外，Agile团队还可以选择使用替代计划以合并团队特定的非工作日。 然后，此备用计划会反映在分配给团队的任何迭代的燃尽图中。 替代计划仅影响燃尽图。 (有关默认时间表以及默认时间表 [!DNL Workfront] 管理员可以创建特定于团队的计划，请参见 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

燃尽图未将部分天数考虑在内。 例如，如果您的团队每个星期五工作4小时，则燃尽图中显示为全天。

有关使用燃尽图的详细信息，请参见 [敏捷燃尽图概述](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Work]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。

## 将备用组计划用于燃尽图

1. 确保 [!DNL Workfront] 管理员已创建替代计划，如中所述 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 团队]**.

1. （可选）单击 **[!UICONTROL 切换组]** 图标 ![“切换团队”图标](assets/switch-team-icon.png)，然后从下拉菜单中选择一个新的Scrum团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

1. 在 **[!UICONTROL 敏捷]** 部分，在 **[!UICONTROL 计划]** 区域，从下拉菜单中选择新计划。

1. 单击 **[!UICONTROL 保存更改]**.
