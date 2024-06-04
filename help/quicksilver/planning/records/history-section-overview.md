---
title: “历史记录”部分概述
description: 您可以在Adobe Workfront Planning中记录的右侧面板中查看对记录所做的更改并由系统记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: 6c50746c4c230d7f9fa2c73b66d13c8b02153b89
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 4%

---

# “历史记录”部分概述

{{planning-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

通过在记录的右侧面板中添加评论或回复，您可以对Adobe Workfront Planning记录进行协作。 您还可以在此区域查看对记录所做的其他更改以及系统记录的更改。

记录的右侧面板显示以下部分：

* **评论**：显示用户添加到记录的评论和回复。 有关管理Workfront Planning记录中的注释的更多信息，请参阅 [管理记录注释](/help/quicksilver/planning/records/manage-record-comments.md).
* **历史记录**：显示用户对记录字段进行的系统记录更改。

## 找到记录的“历史记录”部分

{{step1-to-planning}}

默认情况下，将打开上次访问的工作区。

1. 从中选择表格视图 **视图** 下拉菜单。
1. 单击表视图中记录的名称。

   此时将打开记录的页面。 默认情况下，“注释”区域会在右侧面板中打开。
1. 单击 **显示历史记录** 图标 ![](assets/show-history-icon.png). 对记录字段所做的所有更改都将显示在右侧面板中，从最近的更改开始。
1. （可选）单击 **隐藏历史记录** 图标 ![](assets/hide-history-icon.png) 以关闭右侧面板。

## 有关“历史记录”部分的注意事项

您可以在记录页面的右侧面板的“历史记录”部分中查看对记录字段所做的更改。

![](assets/history-area-in-comments.png)

* Workfront Planning会在“历史记录”部分中记录以下信息：

   * 任何字段更改

   * 字段的旧值和新值（当值更改时）。 旧值以删除线格式显示。

   * 进行更改的用户的全名

   * 更改发生的日期和时间戳。

* 以下类型的字段始终显示旧值（以删除线格式）和新值：

   * 文本
   * 段落
   * 货币
   * 日期
   * 数字
   * 百分比
   * 单选

* 仅当删除了多个值中的至少一个值时，以下类型的字段才会以删除线格式显示旧值：

   * 多选
   * 链接的记录字段
   * 人员

  如果更改仅向字段添加了值，则旧值不会显示，而仅显示新字段值。

* 复选框类型的字段从不以删除线格式显示旧值。 如果字段已编辑，则仅显示进行更改时的当前状态。

  有关Workfront Planning字段的更多信息，请参阅 [创建字段](/help/quicksilver/planning/fields/create-fields.md).

* 对以下类型的字段所做的更改不会显示在“历史记录”部分中：

   * 链接（查找）字段
   * 公式
   * 创建者
   * 创建日期
   * 上次修改者
   * 上次修改日期

* 如果从系统中删除某个字段，则对该字段所做的更新将保留在“历史记录”部分中。 没有迹象表明记录的History部分中已移除该字段。
