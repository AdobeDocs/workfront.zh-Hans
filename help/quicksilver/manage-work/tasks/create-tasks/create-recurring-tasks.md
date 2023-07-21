---
product-area: projects
navigation-topic: create-tasks
title: 创建周期性任务
description: 您可以为必须在单个项目中重复的任务创建周期性任务。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 创建周期性任务

您可以为必须在单个项目中重复的任务创建周期性任务。

有关周期性任务的一般信息，包括编辑现有周期性任务的影响，请参阅 [周期性任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问任务的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予任务访问权限</a>. 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>为项目分配权限并有权添加任务或更高版本</p> <p>创建任务时，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务 </a>. </p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建周期性任务

>[!NOTE]
>
>您不能通过修改现有任务来创建周期性任务。 您必须从头开始创建任务。

1. 转到要创建周期性任务的项目，然后单击 **任务** 区域。
1. 单击 **新建任务**.

   此时将显示新建任务对话框。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 单击 **更多选项** 然后，在 **任务名称** 字段。
1. 继续以添加新任务时所用的相同方式更新任务。 有关添加新任务的更多信息，请参见 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   为新周期性任务指示的持续时间和已计划小时数是每个事件的持续时间和已计划小时数。 父级任务的持续时间是指最早任务的计划起始日期与最迟任务的计划完成日期之间的时间。 父任务的已计划小时数是所有发生的所有已计划小时数的总和。

1. 单击 **概述** （在左侧面板中）。
1. 向下滚动到 **周期性计划** 部分，然后选择 **使其成为周期性任务** 选项。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 在 **频率** 下拉列表，选择您希望任务发生的时间单位数以及时间单位类型。 从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>周期性类型</th> 
      <th>描述</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>天</strong> </td> 
      <td> <p>任务会每天、每2天、每3天等重复一次，具体取决于您选择的节奏。 您可以将任务配置为最多每隔6天重复执行一次。 默认设置为1天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作日</strong> </td> 
      <td> <p> 根据您选择的节奏，该任务会在每个工作日、每2个工作日、每3个工作日等间隔重复执行。 您可以将任务配置为最多每隔6个工作日重复执行一次。</p> <p>此选项使用系统管理员定义的默认计划，如中所述 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>周</strong> </td> 
      <td> <p> 任务会每周、每两周、每三周等等重复一次，具体取决于您选择的节奏。</p> <p>在 <strong>重复</strong> 字段中，选择在一周中您希望每个任务发生的日期。 您可以选择多天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>月</strong> </td> 
      <td> <p>任务会每月、每2个月、每3个月等重复，具体取决于您选择的节奏。 您可以选择1到12个月。 </p> <p>在 <strong>重复</strong> 字段，当您希望任务发生时，从以下选项中进行选择：</p> 
       <ul> 
        <li> <p><strong>每个月的第天 &lt;month date=""&gt;</strong> </p> <p>您可以选择1到30之间的天数，也可以选择 <strong>最后</strong>. 例如，您可以选择“每月30日”。 </p> </li> 
        <li> <p><strong>每月 &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>在第一个下拉菜单中，可以为月中一周的编号选择1到4之间的数字，也可以选择“最后一个”。 </p> <p>在第二个下拉菜单中，您可以选择一周中的任意一天。 </p> <p>例如，您可以选择“每个月在第2个星期二”。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您有与项目计划关联的“计划例外”，则周期性任务无法在例外期间启动。 计划例外期间发生的周期性任务，其开始日期安排在例外之后的第一个工作日。 有关计划例外的详细信息，请参阅文章 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. 在 **开始** 字段，选择您希望周期性任务开始的日期和时间。
1. 在 **结束** 字段，选择您希望定期任务完成的日期和时间

   或

   选择 **之后 `<number>` 发生次数** 以指示周期性任务应发生的次数。 Workfront为任务创建的递归次数与您在此字段中指定的次数相同。

1. 单击 **创建任务。**

   此时将显示任务列表。 周期性任务作为父项创建，所有周期性任务都是其子项。 Workfront使用您为父任务输入的名称（后跟一个数字）自动生成子任务名称。 有关从父周期性任务中自动填写的字段的更多信息，请参阅 [周期性任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （可选）修改每个周期性任务，就像修改项目中的任何其他任务一样。

   例如，您可以添加分配、前置任务、持续时间，并修改有关任务的任何其他信息，包括自定义字段。

   >[!IMPORTANT]
   >
   >在单独修改子项后修改父项循环可能会导致子项之间或子项与父项之间出现不同的信息。 有关更多信息，请参阅 [周期性任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
