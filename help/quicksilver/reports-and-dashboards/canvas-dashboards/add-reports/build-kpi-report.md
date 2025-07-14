---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 构建KPI报告
description: 可将显示单个汇总KPI的突出显示KPI报告添加到画布功能板。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: ba9256255905e139c281099555a6d129fc570984
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# 构建KPI报告

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 有关详细信息，请参阅[画布功能板测试版信息](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)。

您可以构建一个KPI报告并将其添加到画布功能板，该报表将关键绩效指标数据直观地表示为一个数字，然后您便可以使用该数字查看您的项目和团队的执行情况。

![KPI报告示例](assets/kpi-example-main.png)

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

在构建KPI报告之前，您必须创建一个功能板。

## 在画布功能板中构建KPI报告

有许多配置选项可用于构建KPI报表。 在本节中，我们将引导您完成创建规则库的常规过程。

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 单击右上角的&#x200B;**新建仪表板**。

1. 在&#x200B;**创建仪表板**&#x200B;框中，输入仪表板的&#x200B;**名称**&#x200B;和&#x200B;**描述**。

1. 单击&#x200B;**创建**。

1. 在&#x200B;**添加报告**&#x200B;框中，选择&#x200B;**创建报告**。

1. 在左侧，选择&#x200B;**KPI**。

1. 单击右上角的&#x200B;**创建报告**。

1. 按照以下步骤配置&#x200B;**详细信息**&#x200B;部分：

   1. 输入报告&#x200B;**名称**。
   1. 输入报告&#x200B;**描述**。

      >[!NOTE]
      > 
      > 该描述将用作KPI值下方的描述。 如果不输入说明，系统将根据在以下步骤中选择的聚合器和聚合类型为您生成标题。

1. 按照以下步骤配置&#x200B;**生成KPI**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**生成KPI** ![生成KPI图标](assets/build-kpi-icon.png)图标。

   1. 单击&#x200B;**选择字段**，然后指定要添加到报告的字段。

   1. 在&#x200B;**聚合类型**&#x200B;下拉列表中，选择数据如何汇总以生成KPI输出。 此字段中的选项将因上一步中选择的字段类型而异。

1. 按照以下步骤配置&#x200B;**筛选器**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**筛选器** ![筛选器图标](assets/filter-icon.png)图标。

   1. 选择&#x200B;**编辑筛选器**。

   1. 单击&#x200B;**添加条件**，然后指定要作为筛选依据的字段以及定义该字段必须符合何种条件的修饰符。

   1. （可选）单击&#x200B;**添加筛选器组**&#x200B;以添加另一组筛选条件。 集合之间的缺省运算符是AND。 单击运算符以将其更改为OR。

1. 按照以下步骤配置&#x200B;**明细列设置**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**向下钻取列** ![向下钻取列图标](assets/drilldown-column.png)图标。 图表中的字段会自动显示为右侧预览部分中的列。

   1. （可选）要更新任何现有的列配置，请在&#x200B;**当前列**&#x200B;部分中选择要更新的列，然后更新所需的信息（例如，标签、链接状态和格式规则）。

   1. 单击&#x200B;**添加列**，然后选择要显示为表中列的字段。 对要添加的每个列重复此过程。

1. 按照以下步骤配置&#x200B;**深入分析组设置**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**群组设置** ![深入分析群组图标](assets/drilldown-group-icon.png)图标。

   1. 单击&#x200B;**添加分组**&#x200B;按钮，然后选择要创建为分组的字段。

1. 单击&#x200B;**保存**&#x200B;以创建报告并将其添加到仪表板。


