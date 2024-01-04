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

# 导出 [!UICONTROL 甘特图] 至PDF

您可以导出 [!UICONTROL 甘特图] PDF。

导出 [!UICONTROL 甘特图] 要PDF，您可以将其打印或附加到电子邮件中，以便与其他用户共享。

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
   <td> <p>[！UICONTROL视图]或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[！UICONTROL视图]或更高版本的项目访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 导出 [!UICONTROL 甘特图]

1. 访问 [!UICONTROL 甘特图] 要导出到PDF的内容，如中所述 [开始使用 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 确保您已配置 [!UICONTROL 甘特图] 以在导出之前显示相应的信息。

   >[!NOTE]
   >
   >如果导出 [!UICONTROL 甘特图] 从项目列表中，PDF文件仅包含列表中的项目，而不包含每个项目上的任务。 如果要导出任务列表，可以从与任务关联的项目中导出任务列表，也可以通过构建任务报告并在中显示报告结果来导出任务列表。 [!UICONTROL 甘特视图].

   您可以配置以下信息：

   * 根据需要，在任务列表中添加“筛选器”、“视图”和“分组”。 在查看时，将维护在列表视图中选择的任何筛选器和分组 [!UICONTROL 甘特图]. 视图会反映在导出的上 [!UICONTROL 甘特图] 仅在旁边显示的列表中 [!UICONTROL 甘特图] 在第一页上。 视图不显示在 [!UICONTROL 甘特图] 本身。

     >[!TIP]
     >
     >为提供更多空间 [!UICONTROL 甘特图] 本身，应用包含尽可能少的列的视图。

   * 上的配置选项 [!UICONTROL 甘特图]. 例如，您可以启用里程碑、日期、 [!UICONTROL 基线]，或 [!UICONTROL 完成百分比] 以显示在 [!UICONTROL 甘特图].

     有关更多信息，请参阅   [配置信息在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > 分配不会显示在 [!UICONTROL 甘特图] 当 [!UICONTROL 甘特图] 导出到PDF。 当 [!UICONTROL 甘特图] 导出到PDF时，分配仅显示在列表视图中。

   * 在上显示的时间段 [!UICONTROL 甘特图].\

     有关更多信息，请参阅 [在中查看信息 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     时间段在导出文件中的显示方式取决于您是否选择 **[!UICONTROL 我看到的内容]** 或 **[!UICONTROL 多页]** 在后续步骤中。

1. （可选）要仅包括导出PDF中的某些任务，请选择要包括的任务。

   如果未选择任何任务，则所有任务都将包含在导出的PDF中。

   例如，如果您正在查看 [!UICONTROL 甘特图] 适用于包含50个任务，但希望导出项上仅显示10个任务的项目 [!UICONTROL 甘特图]，选择要显示的10个任务。

1. 单击打印机图标。\
   此 **[!UICONTROL 导出到PDF]** 对话框随即显示。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 选择是只导出您所看到的内容，还是导出整个 [!UICONTROL 甘特图]：

   * **[!UICONTROL 我看到的内容]：** 导出在导出最多500个项目之前显示在屏幕上的所有任务（包括任何子任务）。 (这不是 **[!UICONTROL 预览]** 部分； [!UICONTROL 预览] 部分仅包含示例数据。)

     即使父任务被折叠并且子任务不可见，子任务也会包含在导出的PDF中。 要仅包括父任务，请选择要包括的父任务，并保留任何子任务未选中。

     您可以使用 **[!UICONTROL 缩放为]** 下拉菜单或滑块工具，仅显示 [!UICONTROL 甘特图]，如中所述 [在中查看信息 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 多页]：** 导出整个 [!UICONTROL 甘特图]，甚至那些未在当前屏幕上显示的内容，最多可显示500项。\

     您可以使用 **[!UICONTROL 缩放为]** 下拉菜单或滑块工具来确定每个页面上显示的信息量，如中所述 [配置信息在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 选择更细粒度选项以显示更多要导出的页面，或选择更细粒度选项以显示更少要导出的页面。

     >[!NOTE]
     >
     >如果需要导出 [!UICONTROL 甘特图] 如果包含500多个项目，请在查看 [!UICONTROL 甘特图] 以便显示少于500项或250页。 有关如何应用过滤器的信息，请参阅  [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >在以下情况下，无法导出整个甘特图：
     >
     >   
     >   
     >   * 跨越250页时
     >   * 当它包含500个以上的项目时




1. 如果PDF在导出到PDF后打印，则在 **[!UICONTROL 页面大小]** 下拉菜单，选择要打印到的纸张大小。\
   您可以选择 **[!UICONTROL 书信]**， **[!UICONTROL 法律]**， **[!UICONTROL 分类帐]**， **[!UICONTROL A1]**， **[!UICONTROL A2]**， **[!UICONTROL A3]** （仅适用于某些语言），或 **[!UICONTROL A4]**.
1. 在 **[!UICONTROL 页面方向]** 部分，选择是希望以横向还是纵向导出PDF。
1. 选择 **[!UICONTROL 显示图例]** 如果要在导出的PDF中包含图例。
1. 单击 **[!UICONTROL 导出]**.

   的PDF [!UICONTROL 甘特图] 创建并下载到您的计算机。

   请注意导出文件底部的图例。 它仅说明您已在 [!UICONTROL 甘特图] 以及任务列表中提供的内容。

   例如，仅当至少有一个任务与里程碑关联时，里程碑才会显示在图例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
