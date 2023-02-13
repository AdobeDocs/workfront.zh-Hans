---
navigation-topic: use-the-gantt-chart
title: 将甘特图导出到PDF
description: 您可以将甘特图导出到PDF。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---

# 导出 [!UICONTROL 甘特图] PDF

您可以导出 [!UICONTROL 甘特图] PDF。

在导出 [!UICONTROL 甘特图] 要PDF，您可以打印它或将其附加到电子邮件，以便与其他用户共享它。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront]许可证*</td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[!UICONTROL视图]或更高版本对项目和任务的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL视图]或更高级别访问项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 导出 [!UICONTROL 甘特图]

1. 访问 [!UICONTROL 甘特图] 要导出到PDF的ID，如 [开始使用 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 确保您已配置 [!UICONTROL 甘特图] 以在导出信息之前显示相应的信息。

   >[!NOTE]
   >
   >如果导出 [!UICONTROL 甘特图] 在项目列表中，PDF文件仅包含列表中的项目，而不包含每个项目的任务。 如果要导出任务列表，可以从与之关联的项目中执行此操作，或者通过构建任务报告并在 [!UICONTROL 甘特视图].

   您可以配置以下信息：

   * 任务列表中的过滤器、视图和分组。 查看 [!UICONTROL 甘特图]. 视图会反映在导出的 [!UICONTROL 甘特图] 仅在 [!UICONTROL 甘特图] 中。 视图未显示在 [!UICONTROL 甘特图] 自己。

      >[!TIP]
      >
      >为 [!UICONTROL 甘特图] 本身，则应用尽可能少的列的视图。

   * 上的配置选项 [!UICONTROL 甘特图]. 例如，您可以启用里程碑、日期、 [!UICONTROL 基线]或 [!UICONTROL 百分比完成] 显示在 [!UICONTROL 甘特图].

      有关更多信息，请参阅   [配置信息在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

      >[!NOTE]
      >
      > 分配未显示在 [!UICONTROL 甘特图] 当 [!UICONTROL 甘特图] 导出为PDF。 当 [!UICONTROL 甘特图] 导出为PDF时，分配仅在列表视图中显示。

   * 显示在 [!UICONTROL 甘特图].\

      有关更多信息，请参阅 [在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

      时间段在导出文件中的显示方式取决于您是否选择 **[!UICONTROL 我看到的]** 或 **[!UICONTROL 多个页面]** 在后续步骤中。

1. （可选）要在导出的PDF中仅包含某些任务，请选择要包含的任务。

   如果未选择任何任务，则所有任务都将包含在导出的PDF中。

   例如，如果您查看的是 [!UICONTROL 甘特图] 对于包含50个任务，但您只想在导出的 [!UICONTROL 甘特图]，选择要显示的10项任务。

1. 单击打印机图标。\
   的 **[!UICONTROL 导出到PDF]** 对话框。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 选择是仅导出您看到的内容还是整个 [!UICONTROL 甘特图]:

   * **[!UICONTROL 我看到的]:** 导出最多500个项目之前，会导出屏幕上显示的所有任务（包括任何子任务）。 (这不是 **[!UICONTROL 预览]** 部分；the [!UICONTROL 预览] 部分仅包含示例数据。)

      即使父任务折叠且子任务不可见，子任务也会包含在导出的PDF中。 要仅包含父任务，请选择要包含的父任务，然后取消选择任何子任务。

      您可以使用 **[!UICONTROL 缩放到]** 下拉菜单或滑块工具，以仅显示 [!UICONTROL 甘特图]，如 [在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 多个页面]:** 导出整个 [!UICONTROL 甘特图]，即使在当前屏幕上不可见，也最多500个项目。\

      您可以使用 **[!UICONTROL 缩放到]** 下拉菜单或滑块工具来确定每个页面上显示的信息量，如 [配置信息在 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). 选择一个更精细的选项以显示要导出的更多页面，或选择一个更精细的选项以显示要导出的更少页面。

      >[!NOTE]
      >
      >如果需要导出 [!UICONTROL 甘特图] 包含500个以上项目的报表包中，请在查看 [!UICONTROL 甘特图] 以便显示的项目少于500个或页面不足250个。 有关如何应用过滤器的信息，请参阅  [过滤器概述 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
      >
      >
      >在以下情况下，您无法导出整个甘特图：
      >
      >   
      >   
      >   * 跨页数超过250页时
      >   * 当它包含500个以上项目时





1. 如果PDF在导出到PDF后将打印，则在 **[!UICONTROL 页面大小]** 下拉菜单中，选择要打印的纸张大小。\
   您可以选择 **[!UICONTROL 信件]**, **[!UICONTROL 法律]**, **[!UICONTROL 分类帐]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** （仅适用于某些语言）或 **[!UICONTROL A4]**.
1. 在 **[!UICONTROL 页面方向]** 部分，选择是希望以横向还是纵向导出PDF。
1. 选择 **[!UICONTROL 显示图例]** 要在导出的PDF中包含图例。
1. 单击 **[!UICONTROL 导出]**.

   的pdf [!UICONTROL 甘特图] 会创建并下载到您的计算机。

   请注意导出文件底部的图例。 它仅说明您在 [!UICONTROL 甘特图] 和。

   例如，仅当您至少有一个任务与里程碑关联时，里程碑才会显示在图例中。

   ![gantt_chart_with_updated__limited__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
