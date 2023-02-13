---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任务和问题的提交日期
description: 您可以手动更新任务或分配给的问题的提交日期。 有关Adobe Workfront中“提交日期”的更多信息，请参阅“提交日期”概述。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 更新任务和问题的提交日期

您可以手动更新任务或分配给的问题的提交日期。 有关Adobe Workfront中提交日期的更多信息，请参阅 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## 访问要求

<!--drafted for P&P

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   For the current licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>工作或更高级别完成任务</p> 
   <p>请求或更高级别的问题</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务或问题的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，必须将您分配到需要更新其提交日期的任务或问题。

## 更新任务和问题的提交日期

对于任务和问题，更新提交日期是相同的。

1. 转到分配给您的任务或问题作为 **任务所有者**.

   有关确定问题或任务的任务所有者的详细信息，请参阅部分 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 在文章中 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. 在任务或问题标题中单击“处理”

   或

   单击 **启动任务** 或 **开始问题** 如果您的环境中已自定义“处理该项目”按钮，表示您当前正在处理该工作项。

   此时，任务或问题的提交日期和计划完成日期相同。

1. （可选）如果单击“开始任务”或“开始问题”，请单击 **撤消** 屏幕左下角。 提交日期将被删除。

   有关将“Work On It（处理）”按钮替换为“Start（开始）”按钮的信息，请参阅  [将“Work On It（处理它）”按钮替换为“Start（开始）”按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >单击后，用于撤消选择以开始工作的选项将不可用 **处理它**.

1. 单击 **更新** 在左侧面板中，单击 **开始新更新** >**提交日期**

   或

   单击 **任务详细信息** 或 **问题详细信息** 在左侧面板中，双击 **提交日期** 从日历中选择新日期，然后单击 **保存更改**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   进行此更改后，会发生以下情况： 

   * 提交日期和计划完成日期不再相同。

      任务或问题的提交日期和预计完成日期将变为相同。

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 当您从“更新”区域选择新日期时，将自动保存更改。
   * 系统会通知项目所有者您建议为任务或问题设置新的提交日期，并且此时可以更新任务或问题的计划完成日期，以与您建议的提交日期匹配。

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      有关此更改触发的通知和更新的信息，请参阅部分 [通过更改提交日期触发的通知和更新](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) 在文章中 [提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
