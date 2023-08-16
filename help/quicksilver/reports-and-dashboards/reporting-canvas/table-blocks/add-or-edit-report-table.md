---
title: 在报告画布中添加或编辑表块
description: 在报告画布中添加或编辑表块
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: d706659c-457f-4da0-a6e7-03ea29cab700
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# 在报告画布中添加或编辑表块

表格以可过滤、分组和排序的列的形式显示字段信息。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 添加或编辑表块

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **报表**.
1. 单击 **新报告**.

   或

   转到现有报表，单击 **更多** 图标 ![](assets/more-icon-27x15.png) 在报表标题中，然后单击 **编辑**.

1. 在屏幕右侧下方的 **添加块**，可以：

   拖动 **表** 图标 ![](assets/table-icon.png) 直接放到画布上，到您所需的位置。

   或

   双击 **表** 图标 ![](assets/table-icon.png) 在画布顶部添加表格。

   >[!TIP]
   >
   >可以通过拖动块拐角手柄来更改块放置后的大小。

1. 单击 **无标题的表** 在表标题中，键入表的标题。

   ![](assets/table-name-350x142.png)

1. 单击 **编辑** ，以配置表。

   >[!NOTE]
   >
   >如果表格已经是画布的一部分（例如，在编辑现有报表时），则 **编辑** 按钮未显示在块中心。 要编辑表，请单击 **编辑** 图标 ![](assets/edit-icon.png) 在表标题中。
   >![](assets/edit-icon-table-header-350x71.png)

1. 在 **字段** 在右侧的面板中，找到要作为列添加到表中的字段，然后将其拖动到所需的表中，或者双击该字段以将其添加为表中的最后一列。

   您可以在 **Search** 框，以按名称查找特定字段。 您还可以使用此框下的两个下拉菜单，将显示的字段列表缩小到以下一项或两项：

   * 与所需字段关联的对象类型，如项目或任务
   * 所需的字段类型，如日期或货币

   对要添加为列的每个字段重复此步骤。

   >[!TIP]
   >
   >可以通过将选定列拖到新位置来更改表中列的顺序。

1. 执行以下任一操作以进一步配置表：

   * **添加公式字段**：单击 **新建+** 在顶部 **字段** 列表。 有关创建公式字段的详细说明，请参阅 [在报告画布中构建公式字段](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **添加筛选器**：将您希望作为表格过滤依据的字段拖到 **筛选** 部分。 有关设置筛选规则的更多信息，请参阅 [在报告画布中过滤表](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **按特定属性对行进行分组**：将您希望作为表格分组依据的字段拖到 **组** 部分。 有关创建行组的详细信息，请参见 [在报告画布中对表行进行分组](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).
