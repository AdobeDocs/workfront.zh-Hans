---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 为项目启用自定义季度
description: 出于报告目的，如果贵组织的季度基于除日历日期（如工作日或购物日）以外的其他特定标准，则您可能需要创建自定义季度。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# 为项目启用自定义季度

出于报告目的，如果贵组织的季度基于除日历日期（如工作日或购物日）以外的其他特定标准，则您可能需要创建自定义季度。

您最多可以为 [!DNL Adobe Workfront] 系统。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 为 [!DNL Workfront] 系统

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 项目].**

1. 在 **[!UICONTROL 时间轴]** 选择 **[!UICONTROL 启用自定义季度]**.

1. 键入自定义季度的名称，如“2021财季第1季度”。
1. 选择自定义季度的开始和结束日期。

   ![](assets/custom-quarters-nwe.png)

1. （可选）单击 **[!UICONTROL 添加自定义季度]** 向系统添加其他自定义季度。
1. （可选）创建引用会计季度的报表元素。

   **示例：** 为 [!UICONTROL 项目] 列出并包含引用自定义季度的项目的计划完成日期。

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   对“This Quarter”、“Next Quarter”和“Last Quarter”的引用将替换为对自定义季度的新引用。

   有关报表元素的信息，请参阅 [报表元素：过滤器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   有关创建过滤器的信息，请参阅 [在中创建或编辑过滤器 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
