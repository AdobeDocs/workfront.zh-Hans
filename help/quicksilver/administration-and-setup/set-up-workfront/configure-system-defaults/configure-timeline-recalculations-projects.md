---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 配置项目的时间线重新计算
description: 重新计算时间表使经理能够了解项目之外的力量对项目时间表的影响。 项目时间线是指项目的计划和预计日期。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# 配置项目的时间线重新计算

重新计算时间表使经理能够了解项目之外的力量对项目时间表的影响。 项目时间线是指项目的计划和预计日期。

作为 [!DNL Adobe Workfront] 管理员，您可以手动重新计算系统中所有项目的时间表。 项目所有者还可以手动重新计算单个项目的时间表。 有关更多信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

本文描述了您如何作为 [!DNL Workfront] 管理员，可以确定如何以及何时 [!DNL Workfront] 通过在以下位置配置项目首选项，自动计算项目时间线： [!UICONTROL 设置] 区域。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员访问级别</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置自动重新计算

作为 [!DNL Adobe Workfront] 管理员，您可以配置时间 [!DNL Workfront] 自动重新计算项目时间线。 [!DNL Workfront] 可以每晚或在项目范围更改时重新计算项目时间线，或两者都重新计算。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于右上角，或 [!UICONTROL **主菜单**] 图标 ![](assets/lines-main-menu.png) 位于的左上角 [!DNL Workfront]，如果可用，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 项目].**

1. 在 **[!UICONTROL 时间线]** 部分，启用或禁用以下一项或两项设置。 默认情况下，这两个设置都处于启用状态。

   * **每天晚上：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] 仅在晚上，每24小时重新计算一次时间表，并且只针对具有以下状态的项目 [!UICONTROL 当前] 在过去三个月里又更新了。 根据系统负载和其他因素，重新计算时间可能会延迟超过24小时。

     在本例中， [!DNL Workfront] 重新计算所有具有项目的 [!UICONTROL 更新类型] 之 [!UICONTROL 自动] 或 [!UICONTROL 更改时自动更新].

   * **当项目范围更改时**：有关构成项目范围更改的内容的信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     在本例中， [!DNL Workfront] 重新计算更新类型为的所有项目的时间表 [!UICONTROL 更改时自动更新] 或 [!UICONTROL 仅更改时].
有关项目更新类型的信息，请参阅 [项目更新类型概述](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

   系统中所有项目的时间表会根据每个项目的更新类型自动重新计算。

## 重新计算整个时间线 [!DNL Workfront] 实例

您可以运行 [!UICONTROL 重新计算时间线] 诊断以手动重新计算 [!DNL Workfront] 系统。 这使所有项目经理能够立即查看外部更改对计划和计划日期的影响。 有关更多信息，请参阅 [使用诊断触发自动化流程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
