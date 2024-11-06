---
product-area: reporting
navigation-topic: reporting-elements
title: 修改列宽和顺序
description: 阅读本文，了解列宽指南以及如何在Workfront中更改列宽和顺序。
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# 修改列宽和顺序

<!-- Audited: 11/2024 -->

以下是有关Adobe Workfront中列宽的工作原理的准则：

* 默认情况下，Workfront定义列表和报表中的列宽。
* 除非在列的文本模式下另外指定，否则Workfront会根据所有列表和报告中的`valueformat`信息自动调整列的宽度。

  >[!NOTE]
  >
  >Workfront不会根据“设置”和“报告”区域中可用列表中的`valueformat`信息来调整列宽。

  `valueformat`值定义列中显示的信息的类型。 例如，显示数字的列比显示说明字段的列窄。

* 您可以根据自己的需求，自定义Workfront列表和报表中的列宽，具体取决于要在列中显示的信息的种类。

  您可以在查看列表或报表时暂时修改列的宽度，也可以在视图生成器中调整列的宽度，永久修改列的宽度。 有关临时修改列宽的信息，请参阅本文中临时修改列宽和列顺序时的[注意事项](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)部分。

* 内置视图中显示的列具有以前由Workfront定义的硬编码宽度。 要修改这些宽度，必须使用视图生成器中的文本模式手动更新这些列的宽度。

  有关在文本模式下修改列的信息，请参阅[视图：永久编辑列的宽度](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>参与者或更高版本</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>请求或更高版本</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的视图</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理对报告的权限以编辑报告中的视图</p> <p>管理视图的权限以编辑它</p></td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 修改列宽和顺序

您可以通过以下方式修改报表中的列宽度和顺序：

* [临时修改列的宽度和顺序](#modify-width-and-order-of-columns-temporarily)
* [永久修改列的宽度和顺序](#modify-width-and-order-of-columns-permanently)

### 临时修改列的宽度和顺序 {#modify-width-and-order-of-columns-temporarily}

您可以拖动列边框来调整列的大小，也可以通过拖放来临时重新排序Workfront网站中大多数列表中的列。 这包括报表、视图、功能板上的报表和甘特图。

有关Workfront列表的详细信息，请参阅文章[开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

* [临时修改列的宽度和顺序时的注意事项](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [临时调整列大小](#resize-columns-temporarily)
* [临时对列重新排序](#reorder-columns-temporarily)

#### 临时修改列的宽度和顺序时的注意事项 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

您可以临时修改列表中列的宽度和顺序，而无需编辑其视图。

临时调整列大小和排序列时，请考虑以下事项：

* 在调整列大小时，新的列大小将存储在浏览器的本地存储中，并默认保存。 使用不同的浏览器、清除缓存或浏览数据会导致列大小恢复为默认值。 刷新页面会保留您对列宽所做的更改。

>[!NOTE]
> 
>列宽受浏览器窗口大小的限制；如果刷新页面，列宽将减小，直到所有列都可容纳在窗口中而不进行水平滚动。 要强制列保持比浏览器可容纳的宽度更宽，必须在文本模式下设置列的宽度，如[永久修改列的宽度和顺序](#modify-width-and-order-of-columns-permanently)中所述，并避免通过拖动列边框手动调整任何列宽。
>

* 重新排列列时，只有在离开列表或刷新浏览器页面之前，才会维持您选择的顺序。 离开列表或刷新浏览器页面后，列将返回到其默认顺序。
* 为获得最佳性能，您重新排序的列不应在列表中包含超过100个项目。
* 在调整列大小时所做更改仅应用于当前使用的视图，并且仅对您可见。 与其他用户共享视图不会共享您定义的列大小。
* 通过向右拖动列边框来调整列大小后，除了以下情况外，相邻列的宽度将保持不变：

   * 设置区域
   * 报告区域
   * 文档列表和报告

  >[!NOTE]
  >
  >不能将列的左边框移动到任何列表中相邻列的左边框之外。

* 如果将任何列表导出到文件，则列的临时顺序不会传输到导出的文件。 在重新排序列之前，导出的文件显示原始列表中列的顺序。

有关从列表和报告导出数据的详细信息，请参阅文章[导出数据](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

#### 临时调整列大小 {#resize-columns-temporarily}

1. 转到要修改的列表。
1. 拖动列标题的边框，直到列达到所需大小为止。\
   ![](assets/column-resize-350x124.png)

#### 临时对列重新排序 {#reorder-columns-temporarily}

1. 转到要修改的列表。
1. 单击并拖动要移动到所需位置的列标题。

>[!TIP]
>
>在同时查看甘特图和列表视图时，此功能特别有用。 查看甘特图时，列可能会变为隐藏。 要在显示甘特图的同时查看列，只需拖动要查看的列，使其显示在页面的左侧。

### 永久修改列的宽度和顺序 {#modify-width-and-order-of-columns-permanently}

要永久重新排序列，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)一文中的[创建或自定义标准视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view)部分。

只有使用文本模式才能永久修改列的宽度。

有关使用文本模式和永久修改列宽的详细信息，请参阅文章[文本模式的常见用法概述](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。
