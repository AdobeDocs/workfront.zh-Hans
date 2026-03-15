---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 导出数据
description: 您可以从列表、报表、功能板和搜索中导出Adobe Workfront数据。
author: Courtney
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '2252'
ht-degree: 1%

---

# 导出数据

<!-- Audited: 5/2025 -->

您可以从列表、报表、功能板和搜索中导出Adobe Workfront数据。

导出数据的一些原因包括：

* 您想向Workfront之外的其他人提供数据的硬拷贝。
* 要将报告结果作为附件发送给外部用户。
* 您想要创建Workfront数据的外部备份。
* 在Workfront Web应用程序中，一个页面最多只能显示2,000条结果。 如果您的报告生成超过2,000个，您可以将报告导出为任何可用的格式，并在一个列表中查看报告中的所有结果。

您可以手动从Workfront界面导出报告，也可以计划报告的交付，以便稍后将该报告发送给您。 有关计划传送报表的更多信息，请参阅[报表传送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

本文中的信息不适用于以下导出：

* 从图表报表导出信息。

  有关导出图表报表的详细信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 从甘特图导出信息。

  有关导出甘特图的更多信息，请参阅[将甘特图导出到PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

* 从资源规划者导出信息。

  有关从资源规划者导出信息的更多信息，请参阅[资源规划者导航概述](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“导出选项”。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>轻量</p>
      <p>审阅</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限访问“报表”、“功能板”和“日历”以导出报表</p> <p>查看或访问您在列表中查看的对象以导出列表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看或更高权限的报告或信息板以导出报告或信息板</p> <p>查看您在列表中查看的对象的或更高权限以导出列表</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报告，然后才能导出其数据。

有关创建报告的详细信息，请参阅[创建自定义报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)或[创建报告副本](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

## 导出格式和限制

### 导出格式 {#export-formats}

信息可以用以下格式导出：

* PDF（横向或纵向）
* Excel
* Excel (.xlsx)
* 制表符分隔

>[!NOTE]
>
>仪表板只能打印或导出到PDF文件。

### 导出限制 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

关于报表在Workfront中的显示方式以及通过手动导出、已交付报表或通过API导出报表的方式，有一些限制。

* **50,000个单元格：**&#x200B;报表导出中允许Excel文件的最大单元格数。
* **50,000行：**&#x200B;报表导出中允许用于PDF和Tab分隔文件的数据行数。

   * 对于Excel文件，此限制为&#x200B;**65,000行**。
   * 对于Excel(.xlsx)文件，此限制为&#x200B;**100,000行**。
   * 这些限制不包括列标题以及报表中分组所在的行。 例如，如果报告中有6个分组和50,000行数据，则导出的文件将有50,000行。

  >[!IMPORTANT]
  >
  >导出在列中包含集合引用的报告可能会导致错误，即使报告在列出的导出限制范围内。 如果引用的集合太大，导出过程将超时并随后导致错误。
  >
  >为了避免此错误，请在导出之前排除引用大型集合的列，或减小引用集合的大小。

  如果报告中的项目数超过这些限制，则会收到一条错误，指出导出不成功。 将您在屏幕上看到的项目数减少到小于或等于这些限制的数字，以便能够导出结果。

  如果您的报表超过50,000/65,000/100,000行，并且您想要导出所有数据，我们建议您使用过滤器或提示来获取更少的数据负载，并执行多项导出。

  有关使用过滤器的信息，请参阅[过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

  有关使用提示的信息，请参阅[向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)。

* 这些限制适用于：

   * 手动导出报告。
   * 计划报表。
   * 通过API集成导出。
   * 通过快速启动导出的数据。

     有关通过Kick-Starts导出数据的更多信息，请参阅[通过Kick-Starts从Adobe Workfront导出数据](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)。

     >[!NOTE]
     >
     >尽管您只能将数据导出为Excel格式文件，但可以在快速启动文件中导出50,000行。

   * 导出项目的利用率信息。

     有关导出项目的利用率信息的详细信息，请参阅[资源利用率报告概述](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project)。

* **10MB文件大小：**&#x200B;计划传送的任何导出报告的文件大小限制。 如果附加到电子邮件的导出文件大于5MB，则会通过电子邮件发送可下载该文件的链接，而不是附加的导出报告。
* **65,530个超链接：**&#x200B;这是Excel对包含超过65,530个超链接的文档施加的限制。 当手动导出这些文档或在交付报告中发送这些文档时，无法打开它们。 请注意，一个Excel文档可能只有200行数据，但如果文档内的链接超过65,530个，则该文档无法打开。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。
* **256列**：这是Excel对包含超过256列的文档施加的限制。 这些文档无法手动导出，也不能在已送达的报告中发送。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。

  >[!IMPORTANT]
  >
  >导出包含“报告”(Reports)列的报告时，即使该报告的其他内容在列出的导出限制范围内，也可能会导致错误。
  >
  >如果您使用导出功能与其他人共享包含“报表”列的报表，请考虑改为将其设为公用，以共享该报表。 有关公开报表的详细信息，请参阅[在Adobe Workfront中共享报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。
  >
  >如果您使用导出功能从外部评估数据，我们建议您改用Workfront Data Connect。 有关详细信息，请参阅[Workfront Data Connect概述](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md)。

如果尝试导出超出限制的数据，则可能不会在导出中收到所有预期的数据。 而是在此限制内生成修改后的报表。

此外，需要超过60分钟才能运行的报表将被停止。

如果您对您的限制有任何顾虑或问题，请联系Workfront技术支持。

## 导出数据

### 从报表或列表导出数据 {#export-data-from-a-report-or-list}

1. 转到要导出的报告或列表。
1. 选择要导出的项目。 选择单个项目只会导出您选择的项目。

   例如，在项目中，选择要导出的任务。

   或

   取消选择所有项目以导出整个列表。

1. 单击&#x200B;**导出**，然后选择格式。

   <!--
   This note doesn't seem to be true (I tested with e reviewer and they could export the dashboard and its reports), and there's another article all about exporting dashboards. Lisa 12/23
   >[!NOTE]
   >
   >To export a Dashboard report, you must have a Plan license.  
   >![Export dashboard note](assets/nwe-dashboard-export-note-350x271.png)
   -->

   或

   单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon-nwe.png)，然后选择格式。

   您可用的PDF导出选项取决于Workfront用户设置中的“电子邮件区域设置”设置：

   * 北美 — 信纸 — 横向、信纸 — 纵向、其他尺寸

   * 北美以外的所有位置 — A4 — 风景、A4 — 纵向，其他尺寸

1. （条件）根据您使用的操作系统，您可以选择打开或保存文件。 打开包含关联应用程序的文件或将其保存到硬盘驱动器。
1. 要了解信息在导出文件中的显示方式，请继续阅读本文中[使用导出的文档](#use-the-exported-document)一节。

### 从信息板导出数据 {#export-data-from-a-dashboard}

可以从操控板打印信息，也可以将其导出为PDF文件。

有关从功能板导出数据的更多信息，请参阅[导出功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)。

## 使用导出的文档 {#use-the-exported-document}

以下各节介绍信息在导出文件中的显示方式：

* [文件名](#file-names)
* [标题](#titles)
* [时间戳](#timestamps)
* [格式化](#formatting)
* [链接](#links)
* [品牌化](#branding)

### 文件名 {#file-names}

无论导出对象列表还是报告，导出的文件都将具有文件名和标题。 您可以在计算机上通过引用文件名来查找导出的文件。 报告的标题将指示当您与用户共享导出的文件时，这些文件所表示的内容。

#### 导出列表的文件名 {#file-names-for-exported-lists}

导出对象列表时，对象类型会显示在导出文件的文件名和列表标题中。

导出任务或问题列表时，**文件名**&#x200B;可以是下列之一：

* 在项目中导出任务和问题列表时：

   * *The_project_name_Exported_Tasks*(*采用PDF、Excel、Excel (.xlsx)或Tab分隔格式)*
   * *The_project_name_Exported_Issues*(*在PDF、Excel、Excel(.xlsx)或制表符分隔格式中)*

* 在任务（子任务）中导出任务和问题列表时：

   * **The_project_name_the_task_name_Exported_Tasks**(*在PDF、Excel、Excel(.xlsx)或制表符分隔格式中)*
   * **The_project_name_the_task_name_Exported_Issues**(*采用PDF、Excel、Excel (.xlsx)或Tab分隔格式)*

将任何其他对象的列表从项目导出到PDF文件时，所导出文档的文件名会指示所导出对象的类型。\
例如，文件名可以是：

* *Exported_Users*，在导出项目(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*&#x200B;的“人员”选项卡时
* *Exported_Risks*，在导出项目(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*&#x200B;的风险列表时

#### 导出报表的文件名 {#file-names-for-exported-reports}

导出报告时，导出的报告的文件名为：

*The_report_name*(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*

### 标题 {#titles}

在导出对象列表时，只有PDF格式的文件才会有标题。 如果将列表或报告导出为Excel、Excel (.xlsx)或Tab分隔格式，则文件没有标题。

#### 导出列表的标题 {#titles-for-exported-lists}

将项目中的任务和问题列表导出到PDF文件时，所导出文档的标题为下列标题之一：

* *项目名称 — 导出的任务*
* *项目名称 — 导出问题*

将任务中的任务和问题列表导出到PDF文件时，所导出文档的拼贴是以下拼贴之一：

* *项目名称 — 任务名称 — 导出任务*
* *项目名称 — 任务名称 — 导出的问题*

将任何其他对象列表从项目导出到PDF文件时，导出文档的标题会指示您导出的对象的类型。\
例如，标题可以是：

* 在导出项目的“人员”选项卡时，*已导出用户*。
* 在导出项目风险列表时，*导出风险*。

#### 导出报告的标题 {#titles-for-exported-reports}

导出到PDF文件的报告将具有标题。

如果报表导出为Excel、Excel (.xlsx)或Tab分隔格式，则导出的报表将没有标题。 导出文件的标题是报告在Workfront Web应用程序中的显示名称。

如果报告有描述，则会包含在导出的文件中。

### 时间戳 {#timestamps}

从导出项目的用户的上下文中，在导出的文档上显示时间戳。

时间戳包括：

* 日期
* 时间
* 导出项目时的时区

根据导出的文档类型，时间戳会显示在不同的位置：

* **PDF:**&#x200B;时间戳显示在每个页面的页脚和文件名中。
* **Excel:**&#x200B;时间戳显示在文件名中。

### 格式设置 {#formatting}

在将项目导出到PDF时，任何子任务都会显示为缩进到其父任务中。 导出的列表不会折叠任何父级任务。

在发送或计划发送报告时，除非报告具有特殊视图，否则您始终会收到报告的默认选项卡。

如果您的报表在Web应用程序中具有特殊格式，则在交付“详细信息”和“矩阵”选项卡时，应该使用特殊格式交付报表，并且仅适用于PDF和Excel文件。

>[!NOTE]
>
>如果要导出的数据包含共享列，并且要导出为Excel或Tab分隔格式，则导出的文件中会分隔这些列。

有关如何自定义报表中的格式设置的详细信息，请参阅[在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

### 链接 {#links}

链接可以指向Workfront中支持链接的任何对象。 将Workfront中的列表导出到PDF时，原始文档中是否存在的任何受支持的链接在导出的文档中仍然有效。

>[!TIP]
>
>如果自定义字段列的行`valueformat=HTML`以文本模式显示，而链接值未显示在导出的PDF文件中，则需要在文本模式下为列输入其他代码行。
>
>例如，如果您有一个名为“打开第1季度项目”的自定义字段，其中包含链接，则您需要添加以下代码：
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

在导出为Excel格式时，导出的文件中只包含指向Workfront中对象的链接，并且仅在可以选择允许在导出的Excel文档中进行链接的位置（例如报告交付）才支持这些链接。

## 品牌化 {#branding}

>[!IMPORTANT]
>
>品牌仅适用于尚未迁移到Adobe Experience Cloud的组织。
>
>如果您的组织已迁移到Adobe Experience Cloud，则品牌推广不可用。

如果您的Workfront管理员已将自定义品牌添加到全局导航栏的Workfront实例中，则导出的PDF文件还将包含您的个性化徽标。

以任何其他格式导出的数据无法通过您的徽标进行个性化。

有关为Workfront实例和全局导航栏添加品牌的详细信息，请参阅[为您的Adobe Workfront实例添加品牌](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)。
