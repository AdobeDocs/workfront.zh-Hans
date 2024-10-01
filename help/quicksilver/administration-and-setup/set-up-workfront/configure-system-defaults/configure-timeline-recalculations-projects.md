---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: 配置项目的时间表重新计算
description: 重新计算时间表使经理能够了解项目之外的力量对项目时间表的影响。 项目时间线是指项目的计划和预计日期。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 7c2d6d1960752a109c02039c1af8d1d1850bcb8c
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 配置项目的时间线重新计算

重新计算时间表使经理能够了解项目之外的力量对项目时间表的影响。 项目时间线是指项目的计划和预计日期。

作为[!DNL Adobe Workfront]管理员，您可以手动重新计算系统中所有项目的时间表。 项目所有者还可以手动重新计算单个项目的时间表。 有关详细信息，请参阅[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

本文介绍了作为[!DNL Workfront]管理员，如何通过在[!UICONTROL 设置]区域中配置项目首选项来确定[!DNL Workfront]自动计算项目时间线的方式和时间。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td><p>新文档： [！UICONTROL Standard]</p>
   或
   <p>当前： [！UICONTROL计划]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置自动重新计算

作为[!DNL Adobe Workfront]管理员，您可以配置[!DNL Workfront]何时自动重新计算项目时间表。 [!DNL Workfront]可以每晚或在项目范围更改时重新计算项目时间表，或同时重新计算两者。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 项目首选项]** > **[!UICONTROL 项目].**

1. 在&#x200B;**[!UICONTROL 时间线]**&#x200B;部分中，启用或禁用以下一项或两项设置。 默认情况下，这两个设置都处于启用状态。

   * **每晚：** [!DNL Workfront&#x200B;&#x200B;&#x200B;]每24小时重新计算一次时间线，在晚上，只针对状态为[!UICONTROL 当前]并且在过去三个月中更新的项目。 根据系统负载和其他因素，重新计算时间可能会延迟超过24小时。

     在这种情况下，[!DNL Workfront]会重新计算具有[!UICONTROL 自动]或[!UICONTROL 自动且更改时]的[!UICONTROL 更新类型]的所有项目的时间表。

   * **当项目范围更改时**：有关构成项目范围更改内容的信息，请参阅[重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

     在这种情况下，[!DNL Workfront]将重新计算更新类型为[!UICONTROL 自动且更改时为]或仅更改时为[!UICONTROL 的所有项目的时间表]。
有关项目更新类型的信息，请参阅[项目更新类型概述](../../../manage-work/projects/planning-a-project/project-update-type-overview.md)。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   系统中所有项目的时间表会根据每个项目的更新类型自动重新计算。

>[!IMPORTANT]
>
>对于预览和自定义刷新沙盒环境，将禁用夜间重新计算，并且不会自动重新计算项目时间线。 您必须手动重新计算预览和自定义刷新沙盒环境的项目时间线。 有关信息，请参阅[重新计算项目时间表](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)。


## 重新计算整个[!DNL Workfront]实例的时间线

您可以运行[!UICONTROL 重新计算时间线]诊断以手动重新计算[!DNL Workfront]系统中的所有时间线。 这使所有项目经理能够立即查看外部更改对计划和计划日期的影响。 有关详细信息，请参阅[使用诊断来触发自动化进程](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)。
