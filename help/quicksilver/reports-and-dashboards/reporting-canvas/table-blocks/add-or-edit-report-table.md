---
title: 在报表画布中添加或编辑表块
description: 在报表画布中添加或编辑表块
author: Nolan
draft: Probably
feature: Reports and Dashboards
exl-id: d706659c-457f-4da0-a6e7-03ea29cab700
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---


# 在报表画布中添加或编辑表块

表格以列的形式显示字段信息，这些列可以进行过滤、分组和排序。

## 先决条件

在开始之前，您必须注册报表画布测试版。 有关更多信息，请参阅 [报表画布测试版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 添加或编辑表块

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新报告**.

   或

   转到现有报表，单击 **更多** 图标 ![](assets/more-icon-27x15.png) 在报表标题中，单击 **编辑**.

1. 在屏幕右侧，位于 **添加块**，则：

   拖动 **表** 图标 ![](assets/table-icon.png) 直接放到画布上的所需位置。

   或

   双击 **表** 图标 ![](assets/table-icon.png) 向画布顶部添加表。

   >[!TIP]
   >
   >通过拖动块的角手柄来放置块后，可以更改块的大小。

1. 单击 **无标题表** 在表标题中，键入表的标题。

   ![](assets/table-name-350x142.png)

1. 单击 **编辑** 在表块的中心以配置表。

   >[!NOTE]
   >
   >如果表已经包含在画布中（例如，在编辑现有报表时），则 **编辑** 按钮不显示在块的中心。 要编辑表，请单击 **编辑** 图标 ![](assets/edit-icon.png) 在表标题中。
   >![](assets/edit-icon-table-header-350x71.png)

1. 在 **字段** 面板中，找到要作为列添加到表格的字段，然后将其拖动到所需的表格上，或双击该字段以将其添加为表格的最后一列。

   您可以在 **搜索** 框中，可按名称查找特定字段。 您还可以使用此框下的两个下拉菜单，将显示的字段列表缩小为以下一个或两个字段：

   * 与所需字段关联的对象类型，如项目或任务
   * 所需的字段类型，如日期或货币

   对要添加为列的每个字段重复此步骤。

   >[!TIP]
   >
   >通过将选定列拖至新位置，可以更改表中列的顺序。

1. 执行以下任一操作可进一步配置表：

   * **添加公式字段**:单击 **新建+** 在 **字段** 列表。 有关创建公式字段的更多说明，请参阅 [在报表画布中构建公式字段](../../../reports-and-dashboards/reporting-canvas/table-blocks/create-formula-field.md).
   * **添加过滤器**:将您希望表格按过滤的字段拖到 **过滤器** 表格上方的部分。 有关设置过滤器规则的更多信息，请参阅 [在报表画布中过滤表](../../../reports-and-dashboards/reporting-canvas/table-blocks/configure-filter-rules-for-table.md).
   * **按特定属性对行进行分组**：将希望表按分组的字段拖到 **组** 表格上方的部分。 有关创建行组的更多信息，请参阅 [在报表画布中对表行进行分组](../../../reports-and-dashboards/reporting-canvas/table-blocks/group-rows-in-table.md).
