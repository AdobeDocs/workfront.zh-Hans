---
product-area: projects
navigation-topic: create-tasks
title: 创建定期任务
description: 您可以为必须在单个项目中重复的任务创建定期任务。
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# 创建定期任务

您可以为必须在单个项目中重复的任务创建定期任务。

有关循环任务（包括编辑现有循环任务的影响）的常规信息，请参阅 [定期任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关任务访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">授予对任务的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>具有“添加任务”或更高权限的项目参与权限</p> <p>在创建任务时，您会自动收到该任务的“管理”权限</p> <p> 有关任务权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">共享任务 </a>. </p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建定期任务

>[!NOTE]
>
>不能通过修改现有任务来创建循环任务。 必须从头开始创建任务。

1. 转到要创建定期任务的项目，然后单击 **任务** 的子菜单。
1. 单击 **新任务**.

   此时将显示“新建任务”对话框。

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. 单击 **更多选项** 然后，在 **任务名称** 字段。
1. 继续以与添加新任务相同的方式更新任务。 有关添加新任务的详细信息，请参阅 [在项目中创建任务](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. 单击 **概述** 中。
1. 向下滚动到 **循环计划** ，然后选择 **将此任务设为定期任务** 选项。

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. 在 **频率** 下拉列表中，选择您希望任务发生的时间单位数和时间单位类型。 从以下选项中进行选择：

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
      <td> <p>任务每天、每2天、每3天等重复，具体取决于您选择的频度。 您可以将任务配置为最多每6天重复一次。 默认设置为1天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>工作日</strong> </td> 
      <td> <p> 根据您选择的频率，任务每个工作日、每2个工作日、每3个工作日等重复。 您可以将任务配置为最多每6个工作日重复一次。</p> <p>此选项使用系统管理员定义的默认计划，如 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">创建计划</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>周</strong> </td> 
      <td> <p> 任务每周、每2周、每3周等重复，具体取决于您选择的频度。</p> <p>在 <strong>重复</strong> 字段中，选择您希望每个任务发生的日期。 您可以选择多天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>月</strong> </td> 
      <td> <p>任务每月、每2个月、每3个月等重复，具体取决于您选择的频度。 您可以选择1到12个月。 </p> <p>在 <strong>重复</strong> 字段中，选择以下选项以执行任务：</p> 
       <ul> 
        <li> <p><strong>每月 &lt;month date=""&gt;</strong> </p> <p>您可以选择天数（从1天到30天），也可以选择 <strong>最近</strong>. 例如，您可以选择“每月30日”。 </p> </li> 
        <li> <p><strong>每月 &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>在第一个下拉菜单中，您可以为月中的一周数选择介于1到4之间的数字，也可以选择“最后”。 </p> <p>在第二个下拉菜单中，您可以选择一周中的任意一天。 </p> <p>例如，您可以选择“每月2日星期二”。 </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果存在与项目计划相关联的计划例外，则循环任务无法在例外期间启动。 在计划例外期间发生的定期任务计划在例外之后的第一个工作日开始。 有关计划例外的详细信息，请参阅文章 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. 在 **开始** 字段中，选择希望开始定期任务的日期和时间。
1. 在 **结束** 字段中，选择要完成定期任务的日期和时间

   或

   选择 **after `<number>` 发生次数** 以指示重复任务应发生的次数。 Workfront会为任务创建与您在此字段中指示的编号相同的递归数。

1. 单击 **创建任务。**

   此时会显示任务列表。 循环任务创建为父项，所有循环都是其子项。 Workfront会使用您为父代输入的名称后跟一个数字，自动生成子代任务的名称。 有关从父定期任务自动填充哪些字段的详细信息，请参阅 [定期任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. （可选）像修改项目中的任何其他任务一样修改每个定期任务。

   例如，您可以添加分配、前置任务、持续时间，并修改有关任务的任何其他信息，包括自定义字段。

   >[!IMPORTANT]
   >
   >单独修改子项后修改父项重复项可能会导致子项之间或子项与父项之间的信息不同。 有关更多信息，请参阅 [定期任务概述](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
