---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 导出数据
description: 您可以从列表、报表、功能板和搜索中导出Adobe Workfront数据。
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: ae3fc73e93474c75fd03144b66af23f7142867c0
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 0%

---

# 导出数据

<!-- Audited: 5/2025 -->

您可以从列表、报表、功能板和搜索中导出Adobe Workfront数据。

导出数据的一些原因包括：

* 您希望向Workfront外部的人员提供数据的硬拷贝。
* 要将报告结果作为附件发送给外部用户。
* 您要创建Workfront数据的外部备份。
* 在Workfront Web应用程序中，有一个限制是在一个页面上仅显示2,000个结果。 如果您的报告生成超过2,000个，您可以将报告导出为任何可用格式，并在一个列表中查看报告中的所有结果。

您可以从Workfront界面手动导出报表，也可以计划报表的交付，并稍后向您发送该报表。 有关计划传送报表的更多信息，请参阅[报表传送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

本文中的信息不适用于以下导出：

* 从图表报表导出信息。

  有关导出图表报表的详细信息，请参阅[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

* 从甘特图导出信息。

  有关导出甘特图的更多信息，请参阅[将甘特图导出到PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

* 从资源规划者导出信息。

  有关从资源规划者导出信息的更多信息，请参阅[资源规划者导航概述](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“导出选项”。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
    <p>新增：</p>
      <ul>
      <li>浅色或更高</li>
      </ul>
    <p>当前：</p>
      <ul>
      <li>审核或更高</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高权限的报告、功能板和日历以导出报告</p> <p>在列表中查看对象或更高访问权限，以导出列表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表或功能板的权限或更高以导出报表或功能板</p> <p>查看您在列表中查看的对象或更高权限以导出列表</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报表，然后才能导出其数据。

有关创建报告的详细信息，请参阅[创建自定义报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)或[创建报告副本](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

## 导出格式和限制

### 导出格式 {#export-formats}

信息可按下列格式导出：

* PDF（横向或纵向）
* Excel
* Excel (.xlsx)
* 制表符分隔

>[!NOTE]
>
>功能板只能打印或导出到PDF文件。

### 导出限制 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

关于报表在Workfront中的显示方式以及通过手动导出、已交付报表或通过API导出报表的方式，有一些限制。

* **50,000个单元格：**&#x200B;报表导出中允许Excel文件的最大单元格数。
* **50,000行：**&#x200B;报表导出中允许用于PDF和Tab分隔文件的数据行数。

   * 对于Excel文件，此限制为&#x200B;**65,000行**。
   * 对于Excel(.xlsx)文件，此限制为&#x200B;**100,000行**。
   * 这些限制不包括列标题以及报告中分组的行。 例如，如果报表中有6个分组，且有50,000行数据，则导出的文件将有50,000行。

  >[!IMPORTANT]
  >
  >导出列中包含收藏集引用的报告可能会导致错误，即使该报告在列出的导出限制内也是如此。 如果引用的集合过大，导出过程会超时并随后导致错误。
  >
  >要避免此错误，请在导出之前排除引用大型集合的列或减小引用集合的大小。

  如果报表中的项目数超过这些限制，您将收到导出失败错误。 将您在屏幕上看到的项目数减少到小于或等于这些限制的数字，以便能够导出结果。

  如果报表的行数超过50,000/65,000/100,000，并且您想要导出所有数据，我们建议您使用过滤器或提示来获取较小的数据负载，并执行多次导出。

  有关使用筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

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

     有关导出项目的利用率信息的详细信息，请参阅[资源利用率报告概览](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project)。

* **10MB文件大小：**&#x200B;任何计划传送的导出报告的文件大小限制。 如果附加到电子邮件的导出文件大于5MB，则会通过电子邮件发送可下载文件的链接，而不是附加的导出报告。
* **65,530个超链接：**&#x200B;这是Excel对包含65,530个以上超链接的文档施加的限制。 手动导出这些文档或在送达报表中发送它们时，无法打开它们。 请注意，一个Excel文档可能只有200行数据，但如果文档中有超过65,530个链接，则该文档不会打开。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。
* **256列**：这是Excel对包含超过256列的文档施加的限制。 这些文档无法手动导出，也不能在已送达的报告中发送。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。

  >[!IMPORTANT]
  >
  >导出包含“报告”列的报告可能会导致错误，即使该报告不在列出的导出限制之内。
  >
  >如果您使用导出功能与其他人共享包含“报表”列的报表，请考虑改为通过公开该报表来共享该报表。 有关公开报告的详细信息，请参阅[在Adobe Workfront中共享报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。
  >
  >如果您使用导出功能从外部评估数据，我们建议您改用Workfront Data Connect 。 有关详细信息，请参阅[Workfront Data Connect概述](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md)。

如果尝试导出超出限制的数据，则可能不会在导出中收到所有预期的数据。 而是在此限制内生成修改后的报表。

此外，需要超过60分钟才能运行的报表将被停止。

如果您对您的限制有任何顾虑或问题，请联系Workfront技术支持。

## 导出数据

### 从报表或列表导出数据 {#export-data-from-a-report-or-list}

1. 转到要导出的报告或列表。
1. 选择要导出的项目。 选择单个项目仅导出您选择的项目。

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

   可用于导出PDF的选项取决于Workfront用户设置中的电子邮件区域设置：

   * 北美 — 信纸 — 横向、信纸 — 纵向、其他尺寸

   * 北美以外的所有位置 — A4 — 横向、A4 — 纵向、其他尺寸

1. （视情况而定）根据您使用的操作系统，您可以选择打开或保存文件。 使用关联的应用程序打开文件，或将其保存到硬盘驱动器。
1. 若要了解信息在导出文件中的显示方式，请继续阅读本文中的[使用导出的文档](#use-the-exported-document)一节。

### 从功能板导出数据 {#export-data-from-a-dashboard}

您可以从功能板打印信息，也可以将其导出为PDF文件。

有关从仪表板导出数据的详细信息，请参阅[导出仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md)。

## 使用导出的文档 {#use-the-exported-document}

以下各节介绍信息在导出文件中的显示方式：

* [文件名](#file-names)
* [标题](#titles)
* [时间戳](#timestamps)
* [正在格式化](#formatting)
* [个链接](#links)
* [品牌化](#branding)

### 文件名 {#file-names}

无论您是导出对象列表还是导出报告，导出的文件都将具有文件名和标题。 您可以通过引用文件名在计算机上找到导出的文件。 报告的标题将为用户指明在与他们共享导出文件时该文件的内容。

#### 导出列表的文件名 {#file-names-for-exported-lists}

导出对象列表时，对象的类型会显示在导出文件的文件名以及列表标题中。

导出任务或问题列表时，**文件名**&#x200B;可以是以下之一：

* 在项目中导出任务和问题列表时：

   * *The_project_name_Exported_Tasks*(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*
   * *The_project_name_Exported_Issues*(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*

* 导出任务（子任务）中的任务和问题列表时：

   * **The_project_name_the_task_name_Exported_Tasks**(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*
   * **The_project_name_the_task_name_Exported_Issues**(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*

将项目中的任何其他对象列表导出到PDF文件时，导出文档的文件名将指示您导出的对象类型。\
例如，文件名可以是：

* *Exported_Users*，在导出项目(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*&#x200B;的“人员”选项卡时
* *Exported_Risks*，在导出项目(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*&#x200B;的风险列表时

#### 导出报表的文件名 {#file-names-for-exported-reports}

导出报告时，导出的报告的文件名为：

*The_report_name*(*在PDF、Excel、Excel (.xlsx)或Tab分隔格式中)*

### 标题 {#titles}

导出对象列表时，只有PDF格式的文件会有标题。 如果将列表或报表导出为Excel、Excel (.xlsx)或Tab分隔格式，则文件没有标题。

#### 导出列表的标题 {#titles-for-exported-lists}

将项目中的任务和问题列表导出到PDF文件时，所导出文档的标题为以下标题之一：

* *项目名称 — 导出的任务*
* *项目名称 — 导出问题*

将任务中的任务和问题列表导出到PDF文件时，所导出文档的拼贴是以下拼贴之一：

* *项目名称 — 任务名称 — 导出的任务*
* *项目名称 — 任务名称 — 已导出问题*

将项目中的任何其他对象列表导出到PDF文件时，导出文档的标题指示您导出的对象类型。\
例如，标题可以是：

* 在导出项目的“人员”选项卡时，*已导出用户*。
* 在导出项目风险列表时，*导出风险*。

#### 导出报告的标题 {#titles-for-exported-reports}

导出到PDF文件的报告将具有标题。

如果报表导出为Excel、Excel (.xlsx)或Tab分隔格式，则导出的报表将没有标题。 导出的文件的标题是报表在Workfront Web应用程序中显示的名称。

如果报告有说明，则将其包含在导出的文件中。

### 时间戳 {#timestamps}

时间戳显示在导出项目的用户上下文中的导出文档上。

时间戳包括：

* 日期
* 时间
* 导出项目时的时区

根据您导出的文档类型，时间戳会显示在不同的位置：

* **PDF：**&#x200B;时间戳显示在每个页面的页脚和文件名中。
* **Excel：**&#x200B;时间戳显示在文件名中。

### 格式设置 {#formatting}

在将项目导出到PDF时，任何子任务都会显示为缩进到其父任务中。 导出的列表不会折叠任何父级任务。

在发送或计划发送报告时，除非报告具有特殊视图，否则您始终会收到报告的默认选项卡。

如果您的报表在Web应用程序中具有特殊格式，则在交付“详细信息”和“矩阵”选项卡时，应该使用特殊格式交付报表，并且仅适用于PDF和Excel文件。

>[!NOTE]
>
>如果要导出的数据包含共享列，并且要导出为Excel或Tab分隔格式，则导出的文件中会分隔这些列。

有关如何自定义报表中的格式设置的详细信息，请参阅[在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

### 链接 {#links}

链接可以指向Workfront中支持链接的任何对象。 将Workfront中的列表导出到PDF时，原始文档中存在的任何受支持的链接在导出的文档中保持活动状态。

>[!TIP]
>
>如果自定义字段列的行`valueformat=HTML`以文本模式显示，并且链接值未显示在导出的PDF文件中，则需要在文本模式下向列输入其他代码行。
>
>例如，如果您有一个名为“打开第1季度项目”的包含链接的自定义字段，则需要添加以下代码：
>
>`link.url=customDataLabelsAsString(Open Q1 Projects)`
>`linkedname=direct`

在导出为Excel格式时，导出的文件中只包含指向Workfront中对象的链接，并且只有在您可以选择允许导出Excel文档中存在链接的位置（如报表投放）才支持使用链接。

## 品牌化 {#branding}

>[!IMPORTANT]
>
>品牌仅适用于尚未载入Adobe Experience Cloud的组织。
>
>如果您的组织已登记到Adobe Experience Cloud，则品牌推广不可用。

如果您的Workfront管理员为全局导航栏的Workfront实例添加了自定义品牌，则导出的PDF文件还将包含您的个性化徽标。

以任何其他格式导出的数据无法用您的徽标进行个性化。

有关品牌化Workfront实例和全局导航栏的更多信息，请参阅[品牌化Adobe Workfront实例](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md)。
