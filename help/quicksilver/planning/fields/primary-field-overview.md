---
title: 主字段概述
description: 在Adobe Workfront Planning中记录类型的表视图中，可以指定单行文本、数字或公式字段作为主字段。 主字段将成为该类型记录的标题。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: fe3127ab-3f59-46a0-a747-9e9e1582265b
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---


# 主字段概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

主字段是显示在Adobe Workfront Planning中记录类型表视图的第一列中的字段。

默认情况下，“名称”字段是主字段。 但是，您可以将以下类型的任意字段指定为记录的主字段：

* 单行文本字段
* 数字
* 公式

![](assets/another-text-field-as-a-primary-field-highlighted.png)

有关如何将某个字段指定为主字段的信息，请参阅[管理表视图](/help/quicksilver/planning/views/manage-the-table-view.md)。

## 主要字段概述

* 指定为主要字段中的信息将成为记录的标题。

  >[!NOTE]
  >
  >    在Workfront Planning中，名称“主字段”和“记录标题”是同义词。 在表视图中查看记录时，首选“主字段”。


* 记录的标题在以下区域显示：

   * 记录页面和预览框的标题区域
   * 连接的记录字段
   * 视图
* 您不能移动、隐藏或删除表格视图中的主字段，除非指定其他字段作为主字段。
* 主字段始终处于锁定状态，它不是表视图水平滚动的一部分。
* 更改表格视图中的主字段会影响选择它的所有其他用户的视图。
* 更改表视图中的主字段将影响该记录类型的所有表视图。
* 主字段中列出的值始终以超链接方式链接到记录的页面。
* 如果您对工作区<!--<span class="preview">and record type</span>-->具有Contribute或更高权限，则可以编辑主字段（公式字段除外）的值。 公式是自动更新的计算。
