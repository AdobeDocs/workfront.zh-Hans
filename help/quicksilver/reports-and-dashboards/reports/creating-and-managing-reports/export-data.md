---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 导出数据
description: 导出数据的一些原因是 — 编辑我。
author: Nolan
feature: Reports and Dashboards
exl-id: 7fd45fa2-f5d2-411d-849e-cff5be420fbc
source-git-commit: 754ff1d13cd2549f09cfb127786a0a1eeda51a9d
workflow-type: tm+mt
source-wordcount: '2181'
ht-degree: 0%

---

# 导出数据

您可以从各种列表、报表、功能板和搜索中导出Adobe Workfront数据。
本条中的信息不适用于下列出口：

* 从图表报表导出信息。

   有关导出图表报表的更多信息，请参阅 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 从甘特图导出信息。

   有关导出甘特图的更多信息，请参阅 [将甘特图导出到PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md).

* 从资源计划器导出信息。

   有关从资源计划器导出信息的详细信息，请参阅 [资源计划员导航概述](../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

导出数据的一些原因包括：

* 您希望向Workfront以外的人员提供数据的硬拷贝。
* 要将报表结果作为附件发送给外部用户。
* 要创建Workfront数据的外部备份。
* 限制在Workfront Web应用程序内的一个页面上只显示2,000个结果。 如果您的报表生成的结果超过2,000个，则可以将报表导出为以下任何格式，并在一个列表中查看报表中的所有结果。

您可以从Workfront界面手动导出报表，也可以计划报表的提交，该报表稍后会发送给您。 有关计划提交报表的更多信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限可导出报表、功能板、日历</p> <p>查看或更高访问列表中查看的对象以导出列表</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表或功能板的更高权限以导出报表或功能板</p> <p>查看或更高权限，以在列表中查看以导出列表的对象</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

必须先创建报表，然后才能导出其数据。

有关创建报表的更多信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 导出格式和限制

* [导出格式](#export-formats)
* [导出限制](#export-limits)

### 导出格式 {#export-formats}

信息可以采用以下格式导出：

* PDF（信件横向或纵向、法律、分类帐和A4）
* Excel(.xls)
* Excel(.xlsx)
* 制表符分隔

>[!NOTE]
>
>功能板只能打印或导出为.pdf文件。

### 导出限制 {#export-limits}

<!--
NOTE: Alina: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."]
-->

报表在Workfront中的显示方式以及通过手动导出、提交报表或API导出的方式存在一些限制。

* **50,000行：** .pdf和制表符分隔文件的报表导出中允许的数据行数。

   * 对于Excel .xls文件，此限制为 **65,000行**.
   * 对于Excel .xlsx文件，此限制为 **10万行**.
   * 这些限制不包括列标题以及报表中分组的行。 例如，如果您在一个报表中有6个分组，并且有50,000行或数据，则导出的文件将有50,000行。

   >[!IMPORTANT]
   >
   >导出在列中包含集合引用的报表时，可能会导致错误，即使该报表在其他情况下位于所列的导出限制范围内也是如此。 如果引用的集合太大，则导出过程会超时，并随后导致错误。
   >
   >要避免出现此错误，请在导出之前排除引用较大集合的列，或减小引用的集合的大小。

   如果报表的项目数超过这些限制，则会收到导出失败的错误。 将屏幕上显示的项目数量减少到小于或等于这些限制的数量，以便能够导出结果。

   如果您的报表超过50,000/65,000/100,000行，并且您想要导出所有数据，我们建议您使用过滤器或提示来获取较小数据负载，并执行多次导出。

   有关使用过滤器的信息，请参阅 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   有关使用提示的信息，请参阅 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* 这些限制适用于：

   * 手动导出报表。
   * 计划报表。
   * 通过API集成导出。
   * 通过启动导出的数据。

      有关通过启动导出数据的更多信息，请参阅 [通过Kick-Starts从Adobe Workfront导出数据](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md)

      >[!NOTE]
      >
      >虽然您只能将数据导出为Excel格式文件，但您可以在启动文件中导出50,000行。 

   * 导出项目的利用率信息。

      有关导出项目利用率信息的更多信息，请参阅 [资源利用率报告概述](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md#exporting-utilization-information-for-a-project).

* **10MB文件大小：** 计划提交的任何导出报表的文件大小限制。 如果附加到电子邮件的导出文件大于5MB，则会通过电子邮件发送可下载文件的链接，而不是附加的导出报表。
* **65,530个超链接：** 这是Excel对包含65,530个以上超链接的文档所施加的限制。 这些文档在手动导出或在提交的报表中发送时无法打开。 请注意，Excel文档可能只有200行数据，但如果文档内有超过65,530个链接，则该文档不会打开。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。 
* **256列**:这是Excel对包含256列以上的文档所施加的限制。 这些文档无法手动导出，也无法在提交的报表中发送。 此限制仅存在于Excel文件中，而不存在于其他支持的格式中。

如果尝试导出超出限制的数据，您可能不会在导出中收到所有预期数据。 而是在限制内生成修改的报告。

此外，运行时间超过60分钟的报表将被停止。

如果您对限制有任何疑问或疑问，请联系Workfront技术支持。

## 导出数据

* [从报表或列表导出数据](#export-data-from-a-report-or-list)
* [从功能板导出数据](#export-data-from-a-dashboard)

### 从报表或列表导出数据 {#export-data-from-a-report-or-list}

1. 转到要导出的报表或列表。
1. 选择要导出的项目。 （选择单个项目时，只会导出您选择的项目。）

   例如，在项目中，选择要导出的任务。

   或

   取消选择所有项目以导出整个列表。

1. 单击 **导出**，然后选择格式。

   >[!NOTE]
   要导出功能板报表，您必须拥有计划许可证。\
   ![](assets/nwe-dashboard-export-note-350x271.png)

   或

   单击 **导出** 图标 ![](assets/export-icon-nwe.png)，然后选择格式。

   可用于PDF导出的选项取决于Workfront用户设置中的区域设置设置：

   * 北美 — 信件（默认）、法律、分类帐、A4

      <!--   
     <img src="assets/north-america.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

   * 北美以外的所有地点 — A3、A4（默认）、信件、法律、分类帐

      <!--   
     <img src="assets/everywhere-else.jpg" alt="" data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     -->

1. （视情况而定）根据您使用的操作系统，您可能可以选择打开或保存文件。 使用关联的应用程序打开文件或将其保存到硬盘。
1. 继续 [使用导出的文档](#use-the-exported-document).

### 从功能板导出数据 {#export-data-from-a-dashboard}

您可以打印功能板中的信息，也可以将其导出为.pdf文件。

有关从功能板导出数据的更多信息，请参阅 [导出功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

## 使用导出的文档 {#use-the-exported-document}

* [文件名](#file-names)
* [标题](#titles)
* [时间戳](#timestamps)
* [格式](#formatting)
* [链接](#links)
* [品牌化](#branding)

### 文件名 {#file-names}

无论导出对象列表还是报表，导出的文件都将具有文件名和标题。 您可以通过引用文件名在计算机上找到导出的文件。 当您将导出的文件与用户共享时，报表的标题将向用户指示导出的文件代表什么。

* [导出列表的文件名](#file-names-for-exported-lists)
* [导出报表的文件名](#file-names-for-exported-reports)

#### 导出列表的文件名 {#file-names-for-exported-lists}

导出对象列表时，对象类型会显示在导出文件的文件名和列表标题中。

导出任务或问题列表时， **文件名** 可以是以下任一选项：

* 在项目中导出任务和问题列表时：

   * *The_project_name_Exported_Tasks*(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*
   * *The_project_name_Exported_Issues*(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*

* 在任务（子任务）中导出任务和问题列表时：

   * **The_project_name_the_task_name_Exported_Tasks**(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*
   * **The_project_name_the_task_name_Exported_Issues**(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*

将任何其他对象的列表从项目导出到PDF文件时，导出文档的文件名表示导出的对象类型。\
例如，文件名可能为：

* *Exported_Users*，在导出项目(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*
* *Exported_Risks*，在导出项目风险列表(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*

#### 导出报表的文件名 {#file-names-for-exported-reports}

导出报表时，导出报表的文件名为：

*The_report_name*(*PDF、Excel、Excel(.xlsx)或制表符分隔格式*

### 标题 {#titles}

导出对象列表时，只有采用PDF格式的文件才具有标题。 如果将列表或报表导出为Excel、Excel(.xlsx)或制表符分隔格式，则文件将没有标题。

* [导出列表的标题](#titles-for-exported-lists)
* [导出报表的标题](#titles-for-exported-reports)

#### 导出列表的标题 {#titles-for-exported-lists}

将项目中的任务和问题列表导出到PDF文件时，导出文档的标题如下所示：

* *项目名称 — 导出的任务*
* *项目名称 — 导出的问题*

将任务中的任务和问题列表导出到PDF文件时，导出文档的拼贴如下所示：

* *项目名称 — 任务名称 — 导出的任务*
* *项目名称 — 任务名称 — 导出的问题*

将任何其他对象的列表从项目导出到PDF文件时，导出文档的标题会指示导出的对象类型。\
例如，标题可能为：

* *导出的用户*，在导出项目的“人员”选项卡时。
* *出口风险*，在导出项目风险列表时。

#### 导出报表的标题 {#titles-for-exported-reports}

导出到PDF文件的报表将具有标题。

如果报表导出为Excel、Excel(.xlsx)或制表符分隔格式，则导出的报表将没有标题。 导出文件的标题是在Workfront Web应用程序中显示的报表名称。

如果报表包含描述，则该描述将包含在导出的文件中。

### 时间戳 {#timestamps}

导出项目的用户上下文中的导出文档上会显示时间戳。

时间戳包括：

* 日期
* 时间
* 导出项目的时区

根据您导出的文档类型，时间戳会显示在不同位置：

* **PDF:** 时间戳显示在每个页面的页脚和文件名中。
* **Excel:** 时间戳显示在文件名中。

### 格式 {#formatting}

将项目导出为.pdf时，任何子任务都会缩进显示在其父任务中。 导出的列表不会折叠任何父任务。

在发送或计划发送报表以进行提交时，您始终会收到报表的默认选项卡，除非报表具有特殊视图。

如果您的报表在Web应用程序中具有特殊格式，则当仅为.pdf和Excel文件交付详细信息和矩阵选项卡时，报表应使用特殊格式交付。

>[!NOTE]
如果要导出的数据包含共享列，并且导出为Excel或制表符分隔格式，则这些列在导出的文件中会分开。

有关如何自定义报表格式的更多信息，请参阅 [在视图中使用条件格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

### 链接 {#links}

链接可以指向Workfront中支持链接的任何对象。 将Workfront中的列表导出为.pdf时，原始文档中存在的任何受支持的链接在导出的文档中仍处于活动状态。

>[!TIP]
如果行 `valueformat=HTML` 在文本模式下显示自定义字段列，而链接值不在导出的.pdf文件中显示，您需要在文本模式下为列输入额外的代码行。
例如，如果您有一个名为“打开的第1季度项目”的自定义字段包含链接，则需要添加以下代码：

```
link.url=customDataLabelsAsString(Open Q1 Projects)
linkedname=direct
```

导出为Excel格式时，导出的文件中只包含指向Workfront中对象的链接，并且这些链接仅在可以选择允许导出的Excel文档（如报表提交）中的链接的位置受支持。

## 品牌化 {#branding}

如果您的Workfront管理员已为全局导航栏的Workfront实例添加了自定义品牌标识，则导出的.pdf文件也将包含您的个性化徽标。

以任何其他格式导出的数据无法使用您的徽标进行个性化。

有关品牌化Workfront实例和全局导航栏的更多信息，请参阅 [品牌化Adobe Workfront实例](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).
