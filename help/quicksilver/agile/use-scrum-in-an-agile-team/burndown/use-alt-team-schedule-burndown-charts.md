---
product-area: agile-and-teams
navigation-topic: burndown
title: 使用备用燃尽图小组计划
description: 在 [!DNL Adobe Workfront] 中定义的计划通过从燃尽中排除休息日（周末和假日）而影响燃尽图。
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 将备用组计划用于燃尽图

在[!DNL Adobe Workfront]中定义的计划通过从燃尽中排除休息日（周末和节假日）而影响燃尽图。

默认情况下，燃尽图使用默认计划。 除了默认计划之外，Agile团队还可以选择使用替代计划以合并团队特定的非工作日。 然后，此备用计划会反映在分配给团队的任何迭代的燃尽图中。 替代计划仅影响燃尽图。 （有关默认计划以及[!DNL Workfront]管理员如何创建团队特定计划的详细信息，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。）

燃尽图未将部分天数考虑在内。 例如，如果您的团队每个星期五工作4小时，则燃尽图中显示为全天。

有关使用燃尽图的更多信息，请参阅[Agile燃尽图概述](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [!UICONTROL Standard]</p> 
   或
   <p>当前： [!UICONTROL Work]或更高版本</p> </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将备用组计划用于燃尽图

1. 确保[!DNL Workfront]管理员已创建备用计划，如[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)中所述。

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分的&#x200B;**[!UICONTROL 计划]**&#x200B;区域，从下拉菜单中选择新计划。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
