---
product-area: reporting
navigation-topic: reporting-elements
title: 使用里程碑视图
description: 您可以将“里程碑”视图应用于项目列表或报告。 您可以使用“里程碑”视图查看与您正在查看的项目中的任务关联的所有里程碑。
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 1ed84baeacda2717c4f58058fb754e7a79b48baf
workflow-type: tm+mt
source-wordcount: '1370'
ht-degree: 0%

---

# 使用里程碑视图

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

您可以将“里程碑”视图应用于项目列表或报告。 您可以使用“里程碑”视图查看与您正在查看的项目中的任务关联的所有里程碑。

在使用里程碑视图之前，必须存在以下元素：

* 里程碑路径已配置。 有关信息，请参阅[创建里程碑路径](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)。
* 需要添加到项目的里程碑路径。 有关信息，请参阅[编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。
* 里程碑与任务相关联。 有关信息，请参阅[将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

查看项目列表或项目报告时，里程碑视图可用。 以下各节介绍如何查看和使用里程碑视图。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</strong></td> 
   <td> 
    <p>标准</p>
    <p>工作或更高</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看或更高的报告、功能板和日历访问权限</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
    <td> <p>查看权限到项目报告以将里程碑视图应用于报告</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 切换到里程碑视图 {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**里程碑**。

   该列表或报告将显示在“里程碑”视图中。

   有关里程碑视图的信息，请参阅本文中的[里程碑视图概述](#milestone-view-overview)部分。

## 里程碑视图概述 {#milestone-view-overview}

里程碑视图在项目列表和项目报告中可用。 您可以快速查看与您正在查看的项目中的任务关联的所有里程碑。

具有里程碑视图的![项目](assets/project-with-milestone-view-with-complete.png)

>[!NOTE]
>
>里程碑视图在以下区域不可用：
>
>* 时间表，在添加项目时显示在项目列表中。

有关如何切换到里程碑视图的信息，请参阅本文中的[切换到里程碑视图](#switch-to-the-milestone-view)部分。


### 里程碑视图部分

将里程碑视图应用于项目列表时，项目显示在以下部分：

* 与里程碑路径关联的项目首先显示，并在其各自的里程碑路径名称下列出。

  Workfront按以下标准对第一部分中的项目排序，顺序如下：

   1. 里程碑路径ID。 您可以在里程碑路径报表中查看里程碑路径ID。

   2. 在选择“里程碑”视图之前，在先前应用于项目列表的视图中选择作为项目列表第一个排序字段的字段。

* 未与里程碑路径关联的项目显示在下一部分，即未分配部分。 在您选择“里程碑”视图之前，Workfront会按在之前应用于项目列表的视图中为项目列表选择的第一个排序字段来排序未分配分区中的项目。

### 里程碑视图中的项目信息

在“里程碑”视图中查看项目列表或项目报告时，可以使用以下信息：

* **计划日期或预计日期：**&#x200B;指定您希望在“里程碑”视图中显示计划日期还是预计日期。\
  其中显示项目的开始和完成日期以及里程碑路径中每个里程碑任务的完成日期。

  如果您查看的是预计日期，则无法编辑日期。 预计日期由Workfront计算，无法手动更改。

  如果您查看的是计划日期，并且您还拥有项目的“管理”访问权限，则可以直接从“里程碑”视图中编辑以下日期：

   * **项目开始日期：**&#x200B;如果从开始日期开始安排项目，则可以手动更改项目的计划开始日期，然后计算计划完成日期。
   * **项目完成日期：**&#x200B;如果从计划完成日期开始安排项目，则可以手动更改项目的计划完成日期，然后计算计划开始日期。
   * **任务完成日期：**&#x200B;您可以直接从“里程碑”视图中手动更新任务的规划完成日期。

* **完成百分比：**&#x200B;显示每个任务和项目的完成百分比。

  您可以禁用显示完成百分比，如本文中[配置里程碑视图](#configure-what-information-displays-in-the-milestone-view)中显示的信息部分所述。

  您可以直接从“里程碑”视图中调整完成百分比，如本文中“里程碑”视图[中任务的](#adjust-percent-complete-for-tasks-in-the-milestone-view)调整完成百分比部分所述。

* **任务进度状态图标：**&#x200B;以下图标指示任务的进度状态：

   * 准时 — 绿色
   * 滞后 — 黄色
   * 处于风险中 — 蓝色
   * 延迟 — 红色

  <!--* In the Production environment, the following status icons display next to each project and task in the Milestone view: 
      * On Time  
      ![On time icon](assets/gantt-ontime.png)
      * Behind  
      ![Behind icon](assets/gantt-behind.png)
      * At Risk  
      ![At risk icon](assets/gantt-atrisk.png)
      * Late  
      ![Late icon](assets/gantt-late.png)
      <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  您可以禁止显示这些状态图标，如本文中[配置里程碑视图](#configure-what-information-displays-in-the-milestone-view)中显示的信息部分所述。

  有关每种状态类型的更多详细信息，请参阅文章[任务进度状态概述](../../../manage-work/tasks/task-information/task-progress-status.md)。

* **已完成任务的任务状态着色**：将任务标记为“完成”后，任务的背景将在“里程碑”视图中着色，以指示任务是按时完成还是延迟完成：

   * **任务列**&#x200B;的红色底纹：当进度状态为&#x200B;**延迟**&#x200B;时，任务的背景为红色。

   * **任务列**&#x200B;的绿色底纹：当进度状态为&#x200B;**开启时间**&#x200B;时，任务的背景为绿色。

* **项目开始和完成列的项目状态底纹**：

   * **项目开始列**：只有在填充了实际开始日期时，项目开始列的背景才显示为红色或绿色：

      * **项目开始列的红色底纹**：当项目的进度状态为&#x200B;**延迟**&#x200B;时，项目开始列的背景为红色。

      * **项目开始列的绿色底纹**：当项目的进度状态为&#x200B;**开启时间**&#x200B;时，项目开始列的背景为绿色。

     >[!TIP]
     >
     >您必须转到项目详细信息页面才能查看项目的实际开始日期。

   * **项目完成列**：只有在填充了实际完成日期时，“项目完成”列的背景才显示为红色或绿色：

      * **项目完成列的红色底纹**：当项目的进度状态为&#x200B;**延迟**&#x200B;时，项目完成列的背景为红色。

      * **项目完成列的绿色底纹**：当项目的进度状态为&#x200B;**开启时间**&#x200B;时，项目完成列的背景为绿色。

     >[!TIP]
     >
     >您必须转到项目详细信息页面以查看项目的实际完成日期。

   * 当任务的进度状态为“风险”或“落后”时，不会为“开始”和“完成”列分配颜色底纹。

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![带有底纹的里程碑视图](assets/milestone-view-with-shading.png)

* **项目名称**：显示项目名称时带有指向项目的链接。
* **项目完成情况图标**：以下指示器显示项目完成情况：

   * 准时 — 绿色
   * 处于风险中 — 黄色
   * 存在问题 — 红色

  <!--* In the Production environment, an icon displays next to the project name, indicating the condition of the project. The Condition of the project might be one of the following:
      * On Target
      * At Risk
      * In Trouble -->


## 配置里程碑视图中显示的信息 {#configure-what-information-displays-in-the-milestone-view}

您可以配置是否在里程碑视图中显示以下元素：

* 进度状态图标
* 项目和任务的完成百分比

默认情况下，将显示进度状态图标以及项目和任务的完成百分比。

您对这些选项所做的任何更改仅适用于您；其他用户不会受到影响。 您所做的更改将在下次登录到Workfront时保留。

要配置是否显示项目状态图标和项目的完成百分比，请执行以下操作：

{{step1-to-projects}}

1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**里程碑**。

1. 从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">进度状态</td> 
      <td> <p>选择此选项可在每个项目和任务旁边显示进度状态图标。</p> <p>此选项默认处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成百分比</td> 
      <td> <p>选择此选项可在每个项目和任务旁边显示完成百分比。</p> <p>此选项默认处于启用状态。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![里程碑视图选项](assets/milestone-view-options-350x141.png)

## 调整“里程碑”视图中任务的完成百分比 {#adjust-percent-complete-for-tasks-in-the-milestone-view}

您可以在“里程碑”视图中调整任务的完成百分比。 您无法调整父任务（包含子任务的任务）或项目的完成百分比。

要在“里程碑”视图中调整任务的完成百分比，请执行以下操作：

{{step1-to-projects}}

1. 单击&#x200B;**视图**&#x200B;下拉菜单，然后单击&#x200B;**里程碑**。

1. （视情况而定）如果完成百分比未在里程碑视图中当前显示，请启用查看任务和项目的完成百分比，如本文中[配置里程碑视图](#configure-what-information-displays-in-the-milestone-view)中显示的信息。

1. 将&#x200B;**完成百分比幻灯片**&#x200B;移动到新完成百分比以对其进行更新。

   <!--In the Production environment, click the completion percentage below a task, specify a new percentage, then press Enter.-->
