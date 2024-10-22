---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新任务和问题的提交日期
description: 您可以手动更新任务或您分配到的问题的提交日期。 有关Adobe Workfront中提交日期的详细信息，请参阅提交日期概述。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# 更新任务和问题的提交日期

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

您可以手动更新任务或您分配到的问题的提交日期。 有关Adobe Workfront中提交日期的详细信息，请参阅[提交日期概述](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

## 访问要求

<!--Audited: 01/2024-->

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   新增：
   <ul>
   <li><p>任务标准</p> </li>
   <li><p>问题的投稿人或更高版本</p></li>
   </ul>
   当前：
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

* 有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您必须被分配到需要更新其提交日期的任务或问题，然后才能编辑任务或问题的提交日期。

## 更新任务和问题的提交日期


您可以在Workfront的以下区域中更新任务或问题的提交日期：

* 任务或问题的详细信息部分
* 任务或问题标题

  您的Workfront或组管理员必须将提交日期添加到布局模板的任务或问题标题中，才能从任务或问题页面查看该日期。
有关信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

对于任务和问题，更新提交日期的步骤相同。

>[!NOTE]
>
>您可以要求系统或组管理员将提交日期字段添加到摘要面板，使其更易于在Workfront的各个区域中进行更新。
>
>有关更多信息，请参阅以下文章：
>
>* [摘要概述](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [使用布局模板自定义摘要面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。


1. 转到分配为&#x200B;**所有者**&#x200B;的任务或问题。

   有关确定问题或任务的任务所有者的更多信息，请参阅文章[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)中的[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments)部分。

1. （视情况而定，可选）如果Workfront或组管理员将提交日期添加到任务或问题标题，请单击标题中的&#x200B;**提交日期**&#x200B;字段，然后从日历中选择日期。 如果提交日期不在标题中，请继续执行以下步骤。

   ![](assets/commit-date-task-header.png)

1. 单击左侧面板中的&#x200B;**任务详细信息**&#x200B;或&#x200B;**问题详细信息**。
1. 单击&#x200B;**概述**&#x200B;展开它。
1. 更新&#x200B;**提交日期**&#x200B;字段。

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. 单击&#x200B;**保存更改**。

   进行此更改后，会发生以下情况：

   * 任务或问题的提交日期和计划完成日期不再相同。

     相反，任务或问题的提交日期和预计完成日期变为相同。

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * 在Workfront应用程序内通知中，项目所有者收到您为任务或问题建议了新的提交日期的通知。
   * 在更新部分中通知项目所有者，您已建议新的提交日期，此时，他们可以更新任务或问题的规划完成日期，以匹配您建议的提交日期。

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     有关此更改触发的通知和更新的信息，请参阅提交日期概述[一文中的“更改提交日期触发的通知和更新”部分。](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->