---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 为项目配置时间轴重新计算
description: 重新计算时间表使经理能够了解项目外部的力量如何影响项目的时间表。 项目的时间表是指项目的计划日期和预计日期。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 为项目配置时间轴重新计算

重新计算时间表使经理能够了解项目外部的力量如何影响项目的时间表。 项目的时间表是指项目的计划日期和预计日期。

作为 [!DNL Adobe Workfront] 管理员，您可以为系统中的所有项目手动重新计算时间轴。 项目所有者还可以为单个项目手动重新计算时间轴。 有关更多信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

本文介绍了如何 [!DNL Workfront] 管理员可确定如何、何时 [!DNL Workfront] 通过在 [!UICONTROL 设置] 的上界。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>系统管理员访问级别</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置自动重新计算

作为 [!DNL Adobe Workfront] 管理员，您可以配置 [!DNL Workfront] 自动重新计算项目时间表。 [!DNL Workfront] 可以每晚或当项目范围发生更改时重新计算项目时间轴，也可以同时计算两者。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 项目].**

1. 在 **[!UICONTROL 时间轴]** 部分中，启用或禁用以下任一或两个设置。 默认情况下，这两个设置都处于启用状态。

   * **每晚：** [!DNL Workfront&#x200B;&#x200B;&#x200B;] 仅对状态为 [!UICONTROL 当前] 和在过去三个月中进行了更新。

      在这种情况下， [!DNL Workfront] 重新计算具有 [!UICONTROL 更新类型] of [!UICONTROL 自动] 或 [!UICONTROL 自动和更改].

   * **当项目的范围发生更改时**:有关构成项目范围更改的内容的信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

      在这种情况下， [!DNL Workfront] 重新计算“更新类型”为的所有项目的时间表 [!UICONTROL 自动和更改] 或 [!UICONTROL 仅在更改时].
有关项目更新类型的信息，请参阅 [项目更新类型概述](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. 单击&#x200B;**[!UICONTROL 保存]**。

   系统中所有项目的时间表会根据每个项目的“更新类型”自动重新计算。

## 重新计算整个时间表 [!DNL Workfront] 实例

您可以运行 [!UICONTROL 重新计算时间轴] 诊断，以手动重新计算 [!DNL Workfront] 系统。 这允许所有项目经理立即查看外部更改对计划日期和预计日期的影响。 有关更多信息，请参阅 [使用诊断触发自动化进程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
