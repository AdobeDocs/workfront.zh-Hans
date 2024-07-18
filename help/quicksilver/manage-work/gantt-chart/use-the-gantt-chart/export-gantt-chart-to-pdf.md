---
navigation-topic: use-the-gantt-chart
title: 将甘特图导出到PDF
description: 您可以将甘特图导出到PDF。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# 将[!UICONTROL 甘特图]导出到PDF

您可以将[!UICONTROL 甘特图]导出到PDF。

将[!UICONTROL 甘特图]导出到PDF后，您可以将其打印或附加到电子邮件中，以便与其他用户共享。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront]许可证*</td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[！UICONTROL视图]或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL视图]或更高版本的项目访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 导出[!UICONTROL 甘特图]

1. 访问要导出到PDF的[!UICONTROL 甘特图]，如[甘特图[!UICONTROL 入门]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)中所述。
1. 在导出[!UICONTROL 甘特图]之前，请确保已将其配置为显示相应的信息。

   >[!NOTE]
   >
   >如果从项目列表中导出[!UICONTROL 甘特图]，则PDF文件仅包含列表中的项目，而不包含每个项目上的任务。 如果要导出任务列表，可以从与任务关联的项目中导出任务列表，也可以通过构建任务报告并在[!UICONTROL 甘特图]中显示报告结果来导出任务列表。

   您可以配置以下信息：

   * 根据需要，在任务列表中添加“筛选器”、“视图”和“分组”。 在查看[!UICONTROL 甘特图]时，将维护在列表视图中选择的任何筛选器和分组。 视图仅在第一页的[!UICONTROL 甘特图]旁边显示的列表中，反映在导出的[!UICONTROL 甘特图]上。 视图未显示在[!UICONTROL 甘特图]本身。

     >[!TIP]
     >
     >要为[!UICONTROL 甘特图]本身留出更多空间，请应用包含尽可能少的列的视图。

   * [!UICONTROL 甘特图]上的配置选项。 例如，您可以启用里程碑、日期、[!UICONTROL 基线]或完成百分比[!UICONTROL 在[!UICONTROL 甘特图]中显示。]

     有关更多信息，请参阅   [配置信息在[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的显示方式。

     >[!NOTE]
     >
     > 将[!UICONTROL 甘特图]导出到PDF时，分配不会显示在[!UICONTROL 甘特图]中。 将[!UICONTROL 甘特图]导出到PDF时，分配仅显示在列表视图中。

   * 显示在[!UICONTROL 甘特图]中的时间段。\

     有关详细信息，请参阅[查看[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的信息。

     在导出文件中显示时间周期的方式取决于您是选择&#x200B;**[!UICONTROL 我看到的内容]**&#x200B;还是在后续步骤中选择&#x200B;**[!UICONTROL 多个页面]**。

1. （可选）要仅包括导出PDF中的某些任务，请选择要包括的任务。

   如果未选择任何任务，则所有任务都将包含在导出的PDF中。

   例如，如果您正在查看包含50个任务的项目的[!UICONTROL 甘特图]，但希望在导出的[!UICONTROL 甘特图]上仅显示10个任务，请选择要显示的10个任务。

1. 单击打印机图标。\
   将显示&#x200B;**[!UICONTROL 导出到PDF]**&#x200B;对话框。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 选择是只导出您所看到的内容，还是导出整个[!UICONTROL 甘特图]：

   * **[!UICONTROL 我所看到的内容]：**&#x200B;导出在导出最多500个项目之前屏幕上显示的所有任务（包括任何子任务）。 （这不是&#x200B;**[!UICONTROL 预览]**&#x200B;节中显示的内容；[!UICONTROL 预览]节仅包含示例数据。）

     即使父任务被折叠并且子任务不可见，子任务也会包含在导出的PDF中。 要仅包括父任务，请选择要包括的父任务，并保留任何子任务未选中。

     您可以使用&#x200B;**[!UICONTROL 缩放到]**&#x200B;下拉菜单或滑块工具来仅显示[!UICONTROL 甘特图]的一部分，如[查看[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)中的信息中所述。

   * **[!UICONTROL 多个页面]：**&#x200B;导出整个[!UICONTROL 甘特图]，即使它在当前屏幕上不可见，最多也导出了500个项目。\

     您可以使用&#x200B;**[!UICONTROL 缩放到]**&#x200B;下拉菜单或滑块工具来确定每个页面上显示的信息量，如[配置信息在[!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)上的显示方式。 选择更细粒度选项以显示更多要导出的页面，或选择更细粒度选项以显示更少要导出的页面。

     >[!NOTE]
     >
     >如果需要导出包含500个以上项目的[!UICONTROL 甘特图]，请在查看[!UICONTROL 甘特图]之前对列表应用筛选器，以便显示少于500个项目或250页。 有关如何应用筛选器的信息，请参阅[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
     >
     >
     >在以下情况下，无法导出整个甘特图：
     >
     >   
     >   
     >   * 跨越250页时
     >   * 当它包含500个以上的项目时




1. 如果PDF在导出到PDF后要打印，请在&#x200B;**[!UICONTROL 页面大小]**&#x200B;下拉菜单中，选择要打印到的纸张大小。\
   您可以选择&#x200B;**[!UICONTROL Letter]**、**[!UICONTROL Legal]**、**[!UICONTROL Ledger]**、**[!UICONTROL A1]**、**[!UICONTROL A2]**、**[!UICONTROL A3]**（仅适用于某些语言）或&#x200B;**[!UICONTROL A4]**。
1. 在&#x200B;**[!UICONTROL 页面方向]**&#x200B;部分中，选择您希望以横向还是纵向导出PDF。
1. 如果要在导出的PDF中包含图例，请选择&#x200B;**[!UICONTROL 显示图例]**。
1. 单击&#x200B;**[!UICONTROL 导出]**。

   [!UICONTROL 甘特图]的PDF已创建并下载到您的计算机。

   请注意导出文件底部的图例。 它仅说明您在[!UICONTROL 甘特图]中启用的选项以及任务列表中可用的选项。

   例如，仅当至少有一个任务与里程碑关联时，里程碑才会显示在图例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
