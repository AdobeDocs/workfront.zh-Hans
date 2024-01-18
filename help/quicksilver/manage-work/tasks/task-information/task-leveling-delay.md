---
product-area: projects
navigation-topic: task-information
title: 更新任务均衡延迟
description: 有时，项目中的任务计划之间可能存在冲突。 您可以通过重新计划资源和任务来调配资源或解决资源冲突，以便所有任务都能在实际计划内完成。 有关均衡任务的信息，请参阅甘特图中的均衡资源。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# 更新任务均衡延迟

有时，项目中的任务计划之间可能存在冲突。 您可以通过重新计划资源和任务来调配资源或解决资源冲突，以便所有任务都能在实际计划内完成。 有关调配任务的信息，请参阅 [甘特图中的均衡资源](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

作为项目经理或任务受分配人，您还可以在单个任务上添加“均衡延迟”，以解决任何资源或计划冲突。 换言之，任务的计划可能会有所延迟，以确保在Adobe Workfront为任务设置级别时，有一个更加现实的计划可克服资源冲突。

向任务添加均衡延迟可调整任务的预计完成日期。 有关预计完成日期的信息，请参阅 [项目、任务和问题的预计完成日期概述](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限 </p> <p>为项目分配或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 向任务添加均衡延迟

1. 转到要为其添加均衡延迟的任务。
1. 单击 **“更多”图标** 单击任务名称右侧，然后单击 **编辑**.

1. 单击 **设置**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 指定 **均衡延迟**，以小时为单位，然后选择一个时间单位。\
   这是由于资源冲突导致资源延迟启动任务的时间。

   从以下选项中选择时间单位：

   * 分钟
   * 小时。 这是默认设置。
   * 天数
   * 周
   * 月
   * 经过的分钟数
   * 经过的小时数
   * 经过的天数
   * 经过的周数
   * 经过的月数

   >[!TIP]
   >
   >占用时间是任务持续时间的时间单位。 该时间是任务的计划开始日期与计划完成日期之间的时间，包括假日、周末和休息时间。 换言之，经过的时间就是行事历的日数。

1. 单击 **保存**. 

 
