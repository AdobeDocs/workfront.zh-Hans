---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任务和问题的提交日期
description: 您可以手动更新任务或您分配到的问题的提交日期。 有关Adobe Workfront中提交日期的详细信息，请参阅提交日期概述。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 更新任务和问题的提交日期

您可以手动更新任务或您分配到的问题的提交日期。 有关Adobe Workfront中提交日期的详细信息，请参阅 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 访问要求

<!--Audited: 01/2024-->

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
   <td> 
   对于新许可证：
   <ul>
   <li><p>任务标准</p> </li>
   <li><p>问题的投稿人或更高版本</p></li>
   </ul>
   对于当前许可证：
<ul>
   <li><p>任务的工作或更高</p></li> 
   <li><p>有问题的请求或更高版本</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和问题的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务或问题的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 先决条件

在开始之前，您必须被分配到需要更新提交日期的任务或问题。

## 更新任务和问题的提交日期

对于任务和问题，更新提交日期的步骤相同。

1. 转到您分配为的任务或问题 **所有者**.

   有关确定问题或任务的任务负责人的更多信息，请参阅部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. 单击 **任务详细信息** 或 **问题详细信息** 在左侧面板中。
1. 单击 **概述** 以将其展开。
1. 更新 **提交日期** 字段。

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. 单击 **保存更改**.

   进行此更改后，会发生以下情况： 

   * 任务或问题的提交日期和计划完成日期不再相同。

     相反，任务或问题的提交日期和预计完成日期变为相同。

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 如果您使用旧版更新区域，项目所有者将收到通知，告知您为任务或问题建议了一个新的提交日期，并且可以在这一时候更新任务或问题的规划完成日期，以匹配您建议的提交日期。 新的评论体验不支持此功能。 有关信息，请参阅 [新的评论体验](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     有关此更改触发的通知和更新的信息，请参阅部分 [通过更改提交日期触发的通知和更新](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) 在文章中 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
