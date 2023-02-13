---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 创建自定义报表
description: 了解如何创建报表有助于您访问贵组织在Adobe Workfront中需要的信息。 您可以使用Workfront中提供的任何内置报表，也可以从头开始构建您自己的报表。
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 1%

---


# 创建自定义报表

了解如何创建报表有助于您访问贵组织在Adobe Workfront中需要的信息。 您可以使用Workfront中提供的任何内置报表，也可以从头开始构建您自己的报表。

有关内置报表的更多信息，请参阅 [使用Adobe Workfront内置报表](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md). 有关通过复制报表来创建报表的信息，请参阅 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>您将获得对所创建报表的管理权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建报表 {#create-a-report}

要观看有关如何创建报表的视频，请参阅此 [创建自定义报表](#Walk-thr) 下。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) ，然后单击 **报表**.
1. 单击 **新建报表**，然后选择要用于报表的对象类型。

   加载报表生成器。

   有关可用对象报表的特定信息，请参阅部分 [对象报告](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >您还可以通过复制现有报表来创建报表。 有关更多信息，请参阅 [创建报表副本](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. 在报表生成器中，将以下内容添加到您的报表：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>功能</th> 
      <th>描述</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>列（视图）</td> 
      <td> <p>向报表添加列可确定报表包含的信息。</p> <p>要了解如何添加列，请参阅 <a href="#add-columns-view-to-a-report" class="MCXref xref">向报表添加列（视图）</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>分组</td> 
      <td> <p>将分组添加到报表可确定报表的组织方式。</p> <p>要了解如何添加分组，请参阅 <a href="#add-groupings-to-a-report" class="MCXref xref">将分组添加到报表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>过滤器</td> 
      <td> <p>将过滤器规则添加到报表可确定您在报表中看到的信息。</p> <p>要了解如何添加过滤器，请参阅 <a href="#add-filters-to-a-report" class="MCXref xref">将过滤器添加到报表</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>图表</td> 
      <td> <p>向报表中添加图表可确定报表中信息的可视呈现方式。</p> <p>要了解如何添加图表，请参阅 <a href="#add-a-chart-to-a-report" class="MCXref xref">将图表添加到报表</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在报告创建过程中的任意时刻，单击 **应用** 以保存更改。
1. 完成后，单击 **保存并关闭**.

### 向报表添加列（视图） {#add-columns-view-to-a-report}

1. 按照 [创建报表](#create-a-report) 章节。
1. 在报表生成器中，选择 **列（视图）** 选项卡，以标识要在报表中显示的列。
1. （可选）单击 **应用现有视图** ，以使用现有视图。

   有关创建新视图的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. 要添加新列，请单击 **添加列**.

   或

   要更改现有列，请选择要更改的列，然后单击当前名称旁边的(x)。

1. 开始键入要添加的字段。 如果字段可用，则会为每个可关联的对象填充该字段。 单击字段的名称以将其添加到列。

   有关您在列中看到的字段的详细信息，请参阅 [Adobe Workfront术语表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![](assets/nwe-add-column-typeahead-350x459.png)

1. （可选）在 **列设置** 区域，选择 **按此列排序** 要按字母顺序以升序方式对列中的值进行排序，请指示列表是否应使用此列作为其首次排序。

   如果要先按一列中的值、第二列中的值等进行排序，则可以在报表视图中有多个级别的排序。

   如果多个结果根据第一个排序条件是相同的，则它们按第二个排序条件的顺序排序。 如果多个结果根据第一和第二排序条件是相同的，则它们按照第三个排序等进行排序。

   >[!NOTE]
   >
   >如果添加的字段引用的对象与要报告的对象之间的距离太远，则可能无法按此字段排序。\
   >例如，问题报表无法按“项目所有者”字段排序，因为它引用了3个其他对象：项目、所有者和名称。 但是，您仍可以将此字段添加到问题报表中，并查看其相关信息。\
   >要了解有关报表中跨对象引用的更多信息，请参阅 [报表和功能板学习路径](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).

1. （可选）如果您使用分组，并且想要在列中汇总（汇总）信息，请单击 **按以下方式汇总此列** 下拉列表 **列设置** ，然后选择要用于聚合列中信息的选项。

   聚合信息显示在分组行的列中。

   ![分组汇总摘要](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   有关汇总列中数据的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >在分组中聚合以下字段的值时，父对象（例如，父任务）会出现以下例外：
   >
   >* 除“实际工时”(例如“计划/实际人工成本”、“计划/实际费用成本”、“计划/实际成本”、“计划/实际工时”之外的所有“数字”和“币种”字段仅汇总子任务和独立任务的值。 它们不会聚合父任务或父代父代的值。
   >* 实际小时数汇总主要父任务和独立任务的值；它们不会聚合父任务或子任务的父任务的数字。
   >* 数字和货币值的自定义数据字段聚合所有任务：父母、子女、父母的父母和独立任务。


   有关在报表中使用分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （可选）单击 **高级选项** 要为列指定以下信息，请执行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">自定义列标签</td> 
      <td> <p>为列指定自定义标签。 此标签将替换默认标签。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">字段格式</td> 
      <td> <p>选择您希望在列中显示字段值的格式。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在仪表板上显示此列</td> 
      <td> <p>当报表与其他报表并排显示时，选择此选项可在功能板上显示此列。 取消选择此选项时，在报表并排显示的功能板上查看报表时，不会显示此列。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">列规则</td> 
      <td> <p>单击 <strong>为此列添加规则</strong> 向列添加条件格式。 添加规则后，您可以定义字段和文本样式，以了解匹配该规则的字段的显示方式。 单击 <strong>添加规则</strong> 完成规则的定义后，您才会再次访问。 有关视图中条件格式的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">在视图中使用条件格式</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **应用** 以应用您目前所做的更改并使用以下选项继续编辑报表。

   单击 **保存并关闭** 如果您已完成对报表中列的编辑，并且希望保存报表。

### 将分组添加到报表 {#add-groupings-to-a-report}

1. 按照 [创建报表](#create-a-report) 章节。
1. 在报表生成器中，选择 **分组** 选项卡，以确定要对报表中的项目进行分组的方式。
1. 单击 **添加分组** 添加新分组。

   或

   选择 **应用现有分组** 选择现有分组
   ![](assets/nwe-add-grouping-350x230.png)

1. 开始键入要添加为分组的字段。 如果字段可用，则会为每个可关联的对象填充该字段。 单击字段名称以将其添加到该分组。
1. （可选）通过单击 **切换到文本模式**. 有关使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   有关创建新分组的更多信息，请参阅 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. （可选）选择 **默认情况下折叠此分组** 如果希望此分组中的结果显示折叠而不是展开。

   默认情况下，此设置处于禁用状态，分组结果始终显示在扩展列表中。

   >[!TIP]
   >
   >* 当您在查看列表时手动调整分组时，Workfront会在您注销之前记住您的手动首选项。 当您重新登录时，将根据此设置显示列表。
   >* 从图表元素访问分组结果后，分组结果始终会显示为已展开。


1. （可选）您可以选择构建矩阵分组，以网格格式显示结果。

   有关构建矩阵报表的更多信息，请参阅 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 单击 **应用** 以应用您目前所做的更改并使用以下选项继续编辑报表。

   单击 **保存并关闭** 如果您已完成对报表中的分组的编辑，并且希望保存报表。

### 将过滤器添加到报表 {#add-filters-to-a-report}

1. 按照 [创建报表](#create-a-report) 章节。
1. 在报表生成器中，选择 **过滤器** 选项卡，以标识您希望报表包含的信息量。
1. 单击 **添加过滤器规则** 添加自定义过滤器。\
   或\
   选择 **应用现有过滤器** ，以使用现有过滤器。

   ![](assets/nwe-add-a-filter-350x93.png)

1. 如果您单击 **添加过滤器规则**，开始键入要添加为过滤器的字段。 如果字段可用，则会为每个可关联的对象填充该字段。 单击字段的名称以将其添加到该过滤器。\
   使用过滤器修饰符来构建过滤器。 有关过滤器修饰符的详细信息，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   有关创建新过滤器的更多信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. （可选）您可以通过单击 **切换到文本模式**.

   有关使用文本模式的更多信息，请参阅 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. 单击 **应用** 编辑完报表中的过滤器以应用到目前为止所做的更改后，使用以下选项继续编辑报表。

   单击 **保存并关闭** 报表时，您需要保存报表。

### 将图表添加到报表 {#add-a-chart-to-a-report}

1. 按照 [创建报表](#create-a-report) 章节。
1. 在报表生成器中，选择 **图表** 选项卡，然后选择要添加的图表类型。

   ![](assets/nwe-add-a-chart-350x247.png)

   有关在报表中构建图表的更多信息，请参阅 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 单击 **应用** 以应用您目前所做的更改并使用以下选项继续编辑报表。

   单击 **保存并关闭** 如果您编辑完报表，并且想要保存报表，则
