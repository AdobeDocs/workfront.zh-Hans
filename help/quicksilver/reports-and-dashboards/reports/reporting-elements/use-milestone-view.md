---
product-area: reporting
navigation-topic: reporting-elements
title: 使用里程碑视图
description: 您可以将“里程碑”视图应用到项目列表或报表。
author: Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# 使用里程碑视图

您可以将“里程碑”视图应用到项目列表或报表。

在使用里程碑视图之前，需要配置里程碑，需要将里程碑路径添加到项目，并且需要将里程碑与任务关联，如文章中所述 [创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) 和 [将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

查看项目列表或项目报表时，可以使用里程碑视图。 以下各节介绍了如何查看和使用里程碑视图。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看或更高权限访问报表、功能板、日历</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看项目报表的权限以将里程碑视图应用到报表</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 切换到里程碑视图 {#switch-to-the-milestone-view}

1. 转到项目列表或包含要查看的里程碑的项目报表。
1. 单击 **查看** 下拉菜单，然后单击 **里程碑**.

   列表或报表显示在里程碑视图中。

   有关里程碑视图的信息，请参阅部分 [里程碑视图概述](#milestone-view-overview) 在本文中。

## 里程碑视图概述 {#milestone-view-overview}

“里程碑”视图可在项目列表和项目报表中使用。 通过此视图，您可以快速查看与您正在查看的项目中的任务相关联的所有里程碑。


>[!NOTE]
>
>“里程碑”视图在以下区域中不可用：
>* 工时单，在项目列表中添加项目时。



有关如何切换到里程碑视图的信息，请参阅部分 [切换到里程碑视图](#switch-to-the-milestone-view) 在本文中。

![具有里程碑视图的项目](assets/project-with-milestone-view-with-complete.png)

### 里程碑视图部分

将“里程碑”视图应用于项目列表时，项目会显示在以下部分中：

* 与里程碑路径关联的项目将首先显示，并列在其各自里程碑路径的名称下。

   Workfront按以下顺序按以下条件对第一部分中的项目进行排序：

   1. 里程碑路径 ID. 您可以在里程碑路径报表中查看里程碑路径ID。

   2. 在您选择“里程碑”视图之前，在之前应用于项目列表的视图中选择的字段作为项目列表的第一个排序字段。

* 未与里程碑路径关联的项目将在“未分配”部分下方显示。 在您选择“里程碑”视图之前，Workfront会对“未分配”部分中的项目进行排序，该字段将作为之前应用于项目列表的视图中项目列表的第一个排序字段。

### “里程碑”视图中的项目信息

在“里程碑”视图中查看项目列表或项目报表时，可以使用以下信息：

* **计划日期或预计日期：** 指定您是要在“里程碑”视图中显示计划日期还是预计日期。\
   将显示开始和完成日期以及里程碑路径中每个里程碑的日期。\
   如果您正在查看计划日期，并且还具有对项目的“管理”访问权限，则可以直接从“里程碑”视图编辑以下日期：（如果您正在查看“预计日期”，则无法编辑日期，因为“预计日期”是计算的，不能人工更改。）

   * **项目开始日期：** 如果项目是从开始日期开始计划的，您可以手动更改项目的开始日期，然后计算完成日期。
   * **项目完成日期：** 如果项目计划从完成日期开始，您可以手动更改项目的完成日期，然后计算开始日期。
   * **任务完成日期：** 您可以直接从里程碑视图手动更新任务的完成情况。

* **完成百分比：** 显示每个任务和项目的完成百分比。\
   您可以禁用显示完成百分比的功能，如 [配置在“里程碑”视图中显示的信息](#configure-what-information-displays-in-the-milestone-view) 在本文中。\
   您可以直接从里程碑视图中调整完成百分比，如部分中所述 [在“里程碑”视图中为任务调整完成百分比](#adjust-percent-complete-for-tasks-in-the-milestone-view) 在本文中。

* **任务状态图标：** 在“里程碑”视图中，每个项目和任务旁边都会显示一个状态图标。

   * 准时\
      ![](assets/gantt-ontime.png)

   * 滞后\
      ![](assets/gantt-behind.png)

   * 处于风险中\
      ![](assets/gantt-atrisk.png)

   * 延迟\
      ![](assets/gantt-late.png)
   您可以禁用这些状态图标，使其无法显示，如 [配置在“里程碑”视图中显示的信息](#configure-what-information-displays-in-the-milestone-view) 在本文中。\
   有关每种状态类型的更多详细信息，请参阅文章 [任务进度状态概述](../../../manage-work/tasks/task-information/task-progress-status.md).

* **已完成任务的任务状态底纹**:将任务标记为完成后，任务的背景会在“里程碑”视图中显示阴影，以指示任务是按时完成还是延迟完成：

   * **任务列的红色底纹**:进度状态为 **延迟**.

   * **任务列的绿色底纹**:当进度状态为 **开始时间**.

* **“项目开始”和“完成”列的项目状态底纹**:

   * **项目开始列**:只有在填充了“实际开始日期”时，“项目开始”列的背景才为红色或绿色：

      * **“项目开始”列的红色底纹**:当项目的进度状态为 **延迟**.

      * **“项目开始”列的绿色底纹**:当项目的进度状态为 **开始时间**.
   * **“项目完成”列**:只有在填充了“实际完成日期”时，“项目完成”列的背景才为红色或绿色：

      * **“项目完成的红色底纹”列**:当项目的进度状态为 **延迟**.

      * **“项目完成”列的绿色底纹**:当项目的进度状态为 **开始时间**.
   * 当任务的进度状态为“处于风险或落后”时，“开始”和“完成”列不会分配颜色底纹。

   ![具有底纹的里程碑视图](assets/milestone-view-with-shading.png)

* **项目名称**:随即会显示项目名称，并包含指向该项目的链接。
* **“项目条件”图标**:项目名称旁会显示一个图标，用于指示项目的条件。

## 配置在“里程碑”视图中显示的信息 {#configure-what-information-displays-in-the-milestone-view}

您可以配置以下元素是否显示在里程碑视图中：

* 进度状态图标
* 项目和任务完成百分比

默认情况下，会显示项目状态图标和项目完成百分比。

您对这些选项所做的任何更改仅适用于您；其他用户不受影响。 您所做的更改将在下次登录Adobe Workfront时保留。

要配置是否显示项目状态图标和项目的完成百分比，请执行以下操作：

1. 转到项目列表或包含要查看的里程碑的项目报表。
1. 单击 **查看** 下拉菜单，然后单击 **里程碑**.\
   如果要查看Portfolio或项目群中的项目列表，请选择 **里程碑** 子选项卡。

1. 单击 **选项** 位于“里程碑”视图的右上角。\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. 从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">进度状态</td> 
      <td> <p>选择此选项可在每个项目和任务旁边显示进度状态图标。</p> <p>默认情况下，此选项处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>选择此选项可在每个项目和任务旁边显示完成百分比。</p> <p>默认情况下，此选项处于启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 在“里程碑”视图中为任务调整完成百分比 {#adjust-percent-complete-for-tasks-in-the-milestone-view}

您可以在“里程碑”视图中为任务调整完成百分比。 您无法调整父任务（包含子任务的任务）的完成百分比。

要在“里程碑”视图中调整任务的完成百分比，请执行以下操作：

1. 转到项目列表或包含要查看的里程碑的项目报表。
1. 单击 **查看** 下拉菜单，然后单击 **里程碑**.

1. （视情况而定）如果“里程碑”视图中显示的完成百分比不是当前百分比，请单击 **选项** 在里程碑视图的右上角，确保 **完成百分比** 启用。

1. 单击任务下方的完成百分比，指定新百分比，然后按Enter。
