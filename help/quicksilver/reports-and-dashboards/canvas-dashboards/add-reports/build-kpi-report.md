---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 在画布功能板中构建KPI报告
description: 可将显示单个汇总KPI的突出显示KPI报告添加到画布功能板。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# 在画布功能板中构建KPI报告

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>&#x200B;>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>&#x200B;>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

您可以构建一个KPI报告并将其添加到画布功能板，该报表将关键绩效指标数据直观地表示为一个数字，然后您便可以使用该数字查看您的项目和团队的执行情况。

![KPI报告示例](assets/kpi-example-main.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>标准</p> 
<p>规划</p> 
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
      >该描述将用作KPI值下方的描述。 如果不输入说明，系统将根据在以下步骤中选择的聚合器和聚合类型为您生成标题。

1. 按照以下步骤配置&#x200B;**生成KPI**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**生成KPI** ![生成KPI图标](assets/build-kpi-icon.png)图标。

   1. 单击&#x200B;**选择字段**，然后指定要添加到报告的字段。

   1. 在&#x200B;**聚合类型**&#x200B;下拉列表中，选择数据如何汇总以生成KPI输出。 此字段中的选项将因上一步中选择的字段类型而异。

1. 按照以下步骤配置&#x200B;**筛选器**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**筛选器** ![筛选器图标](assets/filter-icon.png)图标。

   1. 选择&#x200B;**编辑筛选器**。

   1. 单击&#x200B;**添加条件**，然后指定要作为筛选依据的字段以及定义该字段必须符合何种条件的修饰符。

   1. （可选）单击&#x200B;**添加筛选器组**&#x200B;以添加另一组筛选条件。 集合之间的缺省运算符是AND。 单击运算符以将其更改为OR。

      有关筛选器的详细信息，请参阅[在画布仪表板中编辑报告筛选器](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md)。

1. 按照以下步骤配置&#x200B;**明细列设置**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**向下钻取列** ![向下钻取列图标](assets/drilldown-column.png)图标。 图表中的字段会自动显示为右侧预览部分中的列。

   1. （可选）要更新任何现有的列配置，请在&#x200B;**当前列**&#x200B;部分中选择要更新的列，然后更新所需的信息（例如，标签、链接状态和格式规则）。

   1. 单击&#x200B;**添加列**，然后选择要显示为表中列的字段。 对要添加的每个列重复此过程。

1. 按照以下步骤配置&#x200B;**深入分析组设置**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**群组设置** ![深入分析群组图标](assets/drilldown-group-icon.png)图标。

   1. 单击&#x200B;**添加分组**&#x200B;按钮，然后选择要创建为分组的字段。

1. 单击&#x200B;**保存**&#x200B;以创建报告并将其添加到仪表板。

## 构建KPI报告示例

在此部分中，我们将介绍创建显示待定文档审批的KPI报告的步骤。

有关KPI报告示例的详细信息，请参阅[创建用于审阅和审批的报告仪表板](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)。

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 单击右上角的&#x200B;**新建仪表板**。

1. 在&#x200B;**创建仪表板**&#x200B;框中，输入仪表板的&#x200B;**名称**&#x200B;和&#x200B;**描述**。

1. 单击&#x200B;**创建**。

1. 在&#x200B;**添加报告**&#x200B;框中，选择&#x200B;**创建报告**。

1. 在左侧，选择&#x200B;**KPI**。

1. 单击右上角的&#x200B;**创建报告**。

1. 按照以下步骤配置&#x200B;**详细信息**&#x200B;部分：

   1. 在&#x200B;*名称*&#x200B;字段中键入&#x200B;**Pending**。
   1. 在&#x200B;*描述*&#x200B;字段中键入&#x200B;**待处理审批**。 这会在KPI值下方显示为描述。

1. 按照以下步骤配置&#x200B;**生成KPI**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**生成KPI** ![生成KPI图标](assets/build-kpi-icon.png)。

   1. 单击&#x200B;**选择字段**。

   1. 找到并选择&#x200B;**文档审批**&#x200B;文件夹。

   1. 选择&#x200B;**状态**。

   1. 在&#x200B;**聚合类型**&#x200B;下拉列表中，选择&#x200B;**计数**。

1. 按照以下步骤配置&#x200B;**筛选器**&#x200B;部分：

   1. 在左侧面板中，单击&#x200B;**筛选器** ![筛选器图标](assets/filter-icon.png)图标。

   1. 选择&#x200B;**编辑筛选器**。

   1. 单击&#x200B;**添加条件**。

   1. 单击进入空条件筛选器，单击&#x200B;**选择字段**，然后选择&#x200B;**状态**。
   1. 将运算符保留为&#x200B;**Equal**，然后在文本框中键入&#x200B;_等待审阅_。
      ![待处理KPI过滤器示例](assets/pending-kpi-filter.png)
1. 单击屏幕右上角的&#x200B;**保存**。

## 构建KPI报告时的注意事项

### 利用字段选择器

**生成KPI**&#x200B;部分中的&#x200B;**部分**&#x200B;下拉列表旨在缩小字段选择器中的选择范围，以便在生成表报告时更容易查找对象。 要开始，请选择一个基本实体对象。

* **所有部分**： Workfront Workflow和Workfront Planning中的所有对象类型。
* **Workfront对象**：本机Workfront工作流对象。
* **Planning记录类型**： Workfront Planning中定义的自定义记录类型。

![分区下拉列表](assets/sections-dropdown.png)

选择基本实体对象后，**节**&#x200B;下拉列表会更新为可用的字段类型选项以供选择。

* **所有节**：本机字段、自定义字段和相关对象。
* **所有字段**：本机字段和自定义字段（不包括关系）。
* **自定义字段**：自定义表单或Planning记录中的客户定义字段。
* **Workfront字段**：仅本机字段。
* **关系**：连接的记录。

![可报告对象选择](assets/reportable-objects-selection.png)

### 引用子对象

其他列、筛选器选项和分组属性的可用关系通常仅限于Workfront对象层次结构中较高的对象，或者在报表的基本实体对象上具有单个选择。 这种情况有一些例外，其中包括：

* 项目>任务
* 文档审批>文档审批阶段
* 文档审批阶段>文档审批阶段参与者

使用上面列出的任何父子关系时，您将在表中看到连接到父对象的每个子记录的一行。


