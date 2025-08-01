---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中构建表报告
description: 您可以将表格报表添加到画布功能板，以便以表格格式显示您的数据。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 8b9676c7ef4efcad1294a9aa786aa6fe52d26cc0
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 在画布功能板中构建表报告

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 有关详细信息，请参阅[画布功能板测试版信息](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

您可以将表格报表添加到画布功能板，以便以表格格式显示您的数据。

![表报告示例](assets/table-example-main.png)

+++ 展开以查看访问要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>当前：计划 </p> 
<p>新增：标准</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td><p>编辑对报告、功能板和日历的访问权限</p>
  </td> 
  </tr>  
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

必须先创建功能板，然后才能构建表格报表。

## 在画布功能板中构建表报告

有许多配置选项可用于构建表报告。 在本节中，我们将引导您完成创建规则库的常规过程。

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 单击右上角的&#x200B;**新建仪表板**。

1. 在&#x200B;**创建仪表板**&#x200B;框中，输入仪表板的&#x200B;**名称**&#x200B;和&#x200B;**描述**。

1. 单击&#x200B;**创建**。

1. 在&#x200B;**添加报告**&#x200B;框中，选择&#x200B;**创建报告**。

1. 在左侧，选择&#x200B;**表**。

1. 单击右上角的&#x200B;**创建报告**。

1. （可选）请按照以下步骤配置&#x200B;**详细信息**&#x200B;部分：

   1. 输入报告&#x200B;**名称**。

   1. 输入报告&#x200B;**描述**。

1. 按照以下步骤配置&#x200B;**生成表**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**表列** ![生成表图标](assets/drilldown-column.png)图标。

   1. 单击&#x200B;**添加列**，然后选择要显示为表中列的字段。 该列显示在右侧的预览部分中。

   1. 对要添加的每个列重复上述步骤。

1. 按照以下步骤配置&#x200B;**筛选器**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**筛选器** ![筛选器图标](assets/filter-icon.png)图标。

   1. 选择&#x200B;**编辑筛选器**。

   1. 单击&#x200B;**添加条件**，然后指定要作为筛选依据的字段以及定义该字段必须符合何种条件的修饰符。 该列显示在右侧的预览部分中。

1. （可选）单击&#x200B;**添加筛选器组**&#x200B;以添加另一组筛选条件。 集合之间的缺省运算符是AND。 单击运算符以将其更改为OR。

1. 按照以下步骤配置&#x200B;**深入分析组设置**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**群组设置** ![群组设置图标](assets/drilldown-group-icon.png)图标。

   1. 单击&#x200B;**添加分组**&#x200B;按钮，然后选择要创建为分组的字段。 分组列显示在右侧的预览部分中。

1. 单击&#x200B;**保存**&#x200B;以创建报告并将其添加到仪表板。