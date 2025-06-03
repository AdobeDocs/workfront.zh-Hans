---
navigation-topic: use-the-gantt-chart
title: 将甘特图导出到PDF
description: 您可以将甘特图导出到PDF。 之后，您可以将其打印或附加到电子邮件中，以便与其他用户共享。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 1%

---

# 将[!UICONTROL 甘特图]导出到PDF

<!--Audited: 5/2025-->

您可以将[!UICONTROL 甘特图]导出到PDF。 之后，您可以将其打印或附加到电子邮件中，以便与其他用户共享。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]许可证</td> 
   <td> <p>新：[！UICONTROL Light]或更高版本</p>
   <p>当前：[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL视图]或更高权限访问项目和任务</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL视图]或更高版本的项目访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 导出[!UICONTROL 甘特图]

1. 访问要导出到PDF的[!UICONTROL 甘特图]，如[甘特图[!UICONTROL 入门]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)中所述。
1. 配置[!UICONTROL 甘特图]以显示要导出的相应信息。

   >[!NOTE]
   >
   >如果您从项目列表中导出[!UICONTROL 甘特图]，则PDF文件仅包含列表中的项目，而不包含每个项目上的任务。 如果要导出任务列表，可以从与任务关联的项目中导出任务列表，也可以通过构建任务报告并在[!UICONTROL 甘特图]中显示报告结果来导出任务列表。

   配置以下任意信息：

   * 单击[!UICONTROL 甘特图]上方的&#x200B;**筛选器**、**视图**&#x200B;和&#x200B;**分组**&#x200B;图标，并添加或编辑应用于[!UICONTROL 甘特图]中项目列表的现有筛选器、视图或分组。

     在查看[!UICONTROL 甘特图]时，将保留在列表视图中选择的任何筛选器和分组。 视图仅在第一页的[!UICONTROL 甘特图]旁边显示的列表中反映在导出的[!UICONTROL 甘特图]上。 视图未显示在[!UICONTROL 甘特图]本身。

     >[!TIP]
     >
     >要为[!UICONTROL 甘特图]留出更多空间，请应用包含尽可能少的列的视图。

   * 选择&#x200B;**切换到预计日期**&#x200B;选项可查看预计日期而不是计划日期。 默认情况下，将显示计划日期。

   * 单击甘特图右上角的&#x200B;**设置**&#x200B;图标![设置图标](assets/settings-icon.png)，然后选择要查看的信息。 选定后，此信息将包含在导出的甘特PDF文件中。

     从以下选项中选择：

      * 实际日期
      * 任务
      * 基准
      * 承诺日期
      * 完成百分比
      * 关键路径
      * 里程碑菱形
      * 里程碑线
      * 前置任务
      * 进度状态
      * （视情况而定）计划日期
      * （视情况而定）预计日期

     有关更多信息，请参阅   [配置信息在[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的显示方式。

     >[!NOTE]
     >
     > 将[!UICONTROL 甘特图]导出到PDF时，分配不会显示在[!UICONTROL 甘特图]中。 导出后，分配将仅显示在列表视图中。

   * 在[!UICONTROL 甘特图]上显示的时间段。 此内容在导出文件中的显示方式取决于您在后续步骤中选择&#x200B;**[!UICONTROL 我看到的内容]**&#x200B;还是&#x200B;**[!UICONTROL 多个页面]**。

     有关详细信息，请参阅[查看[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的信息。



1. （可选）要仅包含导出的PDF中的某些任务，请选择要包含的任务。 如果不选择任何任务，则所有任务都将包含在导出的PDF中。

   例如，如果您正在查看包含50个任务的项目的[!UICONTROL 甘特图]，但希望在导出的[!UICONTROL 甘特图]上仅显示10个任务，请选择要显示的10个任务。

1. 单击甘特图右上角的打印机图标![打印机图标](assets/printer-icon.png)。
此时会显示**[!UICONTROL 导出到PDF]**&#x200B;对话框。

   ![导出到PDF对话框](assets/exported-gantt-ui-350x225.png)

1. 在&#x200B;**导出**&#x200B;部分中，从以下选项中进行选择，以指示您是只导出所看到的内容，还是导出整个[!UICONTROL 甘特图]：

   * **[!UICONTROL 我所看到的内容]：**&#x200B;导出在导出最多500个项目之前屏幕上显示的所有任务（包括任何子任务）。 （这不是&#x200B;**[!UICONTROL 预览]**&#x200B;节中显示的内容；**预览**&#x200B;节仅包含示例数据。）

     即使父任务处于折叠状态且子任务不可见，子任务也会包含在导出的PDF中。 要仅包括父任务，请选择要包括的父任务，并保留任何子任务未选中。

     >[!TIP]
     >
     >您可以使用缩放或滑块工具仅显示[!UICONTROL 甘特图]的一部分，如[查看[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的信息中所述。 选择粒度更细的选项可显示更多要导出的页面，选择粒度更细的选项可显示更少要导出的页面。


   * **[!UICONTROL 多个页面]：**&#x200B;导出整个[!UICONTROL 甘特图]（最多500个项目），包括在当前屏幕上不可见的项目。

     >[!NOTE]
     >
     >* 如果需要导出包含超过500个项目的[!UICONTROL 甘特图]，请在查看[!UICONTROL 甘特图]之前对列表应用筛选器，以便显示少于500个项目或250页。 有关如何应用筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
     >
     >
     >* 在以下情况下，无法导出整个甘特图：
     >   
     >   * 跨越250页时。
     >   * 当它包含500个以上的项目时。


1. 如果PDF在导出到PDF后要打印，请在&#x200B;**[!UICONTROL 页大小]**下拉菜单中选择要打印的纸张大小。
您可以从以下选项中进行选择：

   * **[!UICONTROL 书信]**
   * **[!UICONTROL 法律]**
   * **[!UICONTROL 分类帐]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** （仅适用于某些语言）
   * **[!UICONTROL A4]**
1. 在&#x200B;**[!UICONTROL 页面方向]**&#x200B;部分中，选择要以横向还是纵向导出PDF。
1. 如果要在导出的PDF中包含图例，请选择&#x200B;**[!UICONTROL 显示图例]**。
1. 单击&#x200B;**[!UICONTROL 导出]**。 创建PDF并下载到您的计算机。

   导出文件底部的图例仅说明您在[!UICONTROL 甘特图]中启用的选项以及任务列表中可用的选项。 例如，仅当至少有一个任务与里程碑关联时，里程碑才会显示在图例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
