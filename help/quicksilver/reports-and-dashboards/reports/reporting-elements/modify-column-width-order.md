---
product-area: reporting
navigation-topic: reporting-elements
title: 修改列宽和顺序
description: 请参阅本文，了解列宽准则以及如何在Workfront中更改列宽和顺序。
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# 修改列宽和顺序

以下是列宽在Adobe Workfront中如何工作的准则：

* 默认情况下，Workfront会在列表和报表中定义列的宽度。
* Workfront会根据 `valueformat`除非在列的文本模式中另有指定，否则将在所有列表和报表中显示相应信息。

   >[!NOTE]
   >
   >Workfront不会根据 `valueformat` “设置”和“报表”区域的可用列表中的信息。

   的 `valueformat` 值定义列中显示的信息类型。 例如，显示数字的列比显示“描述”字段的列要窄。

* 您可以根据要在列中显示的信息类型，自定义Workfront列表和报表中列的宽度以满足您的需求。

   在查看列表或报表时，您可以临时修改列宽，也可以通过调整视图生成器中列的宽度来永久修改列宽。 有关临时修改列宽的信息，请参阅 [临时修改列宽和顺序时的注意事项](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 章节。

* 内置视图中显示的列具有以前由Workfront定义的硬编码宽度。 要修改这些宽度，您必须在视图生成器中使用文本模式手动更新这些列的宽度。

   有关在文本模式下修改列的信息，请参阅 [查看：永久编辑列的宽度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理报表的权限以编辑报表中的视图</p> <p>管理要编辑的视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 修改列宽和顺序

您可以通过以下方式修改报表中列的宽度和顺序：

* [临时修改列的宽度和顺序](#modify-width-and-order-of-columns-temporarily)
* [永久修改列的宽度和顺序](#modify-width-and-order-of-columns-permanently)

### 临时修改列的宽度和顺序 {#modify-width-and-order-of-columns-temporarily}

您可以拖动列边框以调整列大小，并拖放列以临时重新排序整个Workfront网站中大多数列表中的列。 这包括报表、视图、功能板报表和甘特视图。

有关Workfront列表的更多信息，请参阅文章 [开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [临时修改列宽和顺序时的注意事项](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [临时调整列大小](#resize-columns-temporarily)
* [临时重新排序列](#reorder-columns-temporarily)

#### 临时修改列宽和顺序时的注意事项 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

您可以临时修改列表中列的宽度和顺序，而无需编辑其视图。

临时调整列大小和对列进行排序时，请考虑以下事项：

* 调整列大小时，新列大小会存储在浏览器的本地存储中，并且默认情况下会进行保存。 使用其他浏览器或清除缓存或浏览数据会导致列大小恢复为默认值。 刷新页面会保留您对列宽所做的更改。
* 重新排序列时，只有在您离开列表或刷新浏览器页面之前，才会保留您选择的顺序。 在离开列表或刷新浏览器页面后，列将返回其默认顺序。
* 为了获得最佳性能，要重新排序的列在列表中应不超过100个项目。
* 调整列大小时，所做的更改将仅应用于当前使用的视图，并且仅对您可见。 与其他用户共享视图时，不会共享您定义的列大小。
* 在通过向右拖动列的边框来调整列大小后，将保留相邻列的宽度，以下情况除外：

   * 设置区域
   * “报告”区域
   * 文档列表和报表

   >[!NOTE]
   >
   >无法在任何列表中将列的左边框移到相邻列的左边框之上。

* 如果将任何列表导出到文件，则列的临时顺序不会传输到导出的文件。 导出的文件显示原始列表中列的顺序，然后列才重新排序。

有关从列表和报表导出数据的更多信息，请参阅文章 [导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### 临时调整列大小 {#resize-columns-temporarily}

1. 转到要修改的列表。
1. 拖动列的边框，直到列达到所需大小。\
   ![](assets/column-resize-350x124.png)

#### 临时重新排序列 {#reorder-columns-temporarily}

1. 转到要修改的列表。
1. 单击要移动到其他位置的列以选取该列。
1. 将列拖到正确的位置。
1. 将列拖放到位置中，以将其移动。

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>当同时查看甘特图和列表视图时，此功能特别有用。 查看甘特图时，列可能会变为隐藏。 要在显示甘特图时查看列，只需拖动要查看的列即可，使其显示在页面的左侧。

### 永久修改列的宽度和顺序 {#modify-width-and-order-of-columns-permanently}

要永久重新排序列，请参阅 [创建或自定义标准视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) 在文章中 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

只能使用文本模式永久修改列的宽度。

有关使用文本模式和永久修改列宽的详细信息，请参阅文章 [文本模式常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
