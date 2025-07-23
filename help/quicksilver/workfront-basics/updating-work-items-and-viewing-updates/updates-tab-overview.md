---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新部分概述
description: 对象的“更新”部分显示用户对对象所做的注释或跟踪对象更改的系统更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: de42974a9a5c4c346ef3ae1cce09968befd1381c
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 4%

---


# 更新部分概述

<!-- Audited: 1/2024 -->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>
-->

对象的“更新”部分显示用户对对象所做的注释或跟踪对象更改的系统更新。

<!--
>[!IMPORTANT]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>
>Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:
>* The new experience
>* The legacy experience
>* The new and the legacy experience
>
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
><Span class="preview"> The legacy commenting experience has been removed from projects, tasks, issues, and documents in the Preview environment. </span>
>
>The new commenting experience is available only for the Updates section of Workfront objects, and it is not available when you access updates from the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets 
> * Summary panel in the Workload Balancer
>
><span class="preview">The new commenting experience is available in the Summary panel in lists, timesheets, and the Workload Balancer in the Preview environment and in the Production environment for customers who have opted for the fast release process.
-->

## “更新”部分的概述

对象的“更新”部分显示系统更新，以及用户在过去90天内进行的最近200次更新。

![更新分区](assets/updates-tab-with-unified-experience-for-issues-all-tab.png)

<!--Info for April 11: Add the following right under the screen shot above:-->

以下对象具有“更新”部分，您可以在其中添加注释或查看系统更新：

* 项目
* 任务
* 问题
* 项目群
* 项目组合
* 模板
* 模板任务
* 用户
* 时间表
* 团队
* 目标
* 迭代

以下对象具有可以添加注释和查看系统更新的区域：

* 展示板上的信息卡
* Workfront Planning中的记录

<!--info for April 11: remove all the information below, all the way down to the following section: -->

<!--
Depending on what objects you access the commenting experience for, you might find the following experience for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

  * Project
  * Task (this includes Stories)
  * Issue
  * Document

    >[!TIP]
    >
    >Use the New commenting option to display the new commenting experience (when you enable it) or the legacy commenting experience (when you disable it). The new commenting experience is the default. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

  * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations

    There is no option to enable the new commenting experience for iterations. For more information, see [Manage iteration comments](/help/quicksilver/agile/use-scrum-in-an-agile-team/iterations/manage-iteration-updates.md). 
-->

<!--Info for April 11: reword the section title below to: Overview of the Updates section; and remove the preview tags-->

### 更新部分选项卡概述

![更新分区](assets/updates-tab-after-unified-experience-for-tasks-all-tab.png)

“更新”部分在以下选项卡中显示信息：

* **评论**：显示用户发表的评论以及对这些评论的回复。 使用“注释”选项卡可添加新注释或回复现有注释。 有关更新对象的信息，请参阅[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。
* **系统活动**：显示系统更新，这些更新是Workfront为记录对象上的特定事件而创建的信息性消息。 例如，状态、名称或自定义字段的更改通过系统更新来捕获。 您的Workfront或组管理员可以为您的对象启用系统更新。 对旧版注释体验中的系统活动记录所做的任何回复都将以只读形式填充到“系统活动”选项卡中。 有关详细信息，请参阅[配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)。
* **全部（只读）**：在一个位置同时显示用户注释和系统活动注释。 这是一个仅供查看的选项卡。 您无法在“全部”选项卡的现有注释中回复注释或标记其他用户。 要回复特定注释，请使用“全部”选项卡中指向“注释”选项卡的链接。 有关更新对象的信息，请参阅[更新工作](../updating-work-items-and-viewing-updates/update-work.md)。

  >[!NOTE]
  >
  >“注释”和“系统”活动选项卡实时更新。 必须刷新“全部”选项卡才能查看最新更新。

### 不同对象的“更新”区域之间的异同

不同对象的注释和更新显示方式存在差异。

* 以下对象在更新部分的所有三个选项卡中具有相似的体验：

   * 项目
   * 任务
   * 问题
   * 项目群
   * 项目组合
   * 用户
   * 时间表

* 以下对象没有“系统活动”选项卡或“全部”选项卡，“注释”选项卡中的体验与所有其他对象的体验相匹配：

   * 团队
   * 模板
   * 模板任务

* 以下对象没有“系统活动”选项卡或“全部”选项卡，“注释”选项卡中的体验不同于所有其他对象的体验：

   * 迭代
   * 展示板区域中的临时信息卡

     有关信息卡更新的详细信息，请参阅[将临时信息卡添加到展示板](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)。

* 以下对象具有“系统活动”选项卡，没有“全部”选项卡：

   * 板区域中的已连接卡

     有关信息，请参阅[在展示板上使用连接的卡片](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)。

* 以下对象具有替换系统活动选项卡的“历史记录”选项卡：

   * Workfront Planning中的记录

     有关信息，请参阅[历史记录部分概述](/help/quicksilver/planning/records/history-section-overview.md)。

* 以下对象没有“全部”选项卡，“注释”选项卡中的体验与大多数对象的体验相匹配：

   * 目标

     有关目标更新的详细信息，请参阅[管理目标注释](/help/quicksilver/workfront-goals/goal-management/manage-goal-comments.md)。

<!-- info for April 11: hide the entire section below: -->

<!--
### Overview of the legacy Updates section 

![](assets/updates-tab-before-unified-experience-for-tasks.png)

The legacy Updates section shows the following information:

* **User updates**: Comments made by users and replies to those comments. 
* **System updates**: Informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your objects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

The following objects don't record system updates:

* Team
* Template
* Template Task
* Iterations
-->

## 也出现在较高级别对象上的更新

某些对象的注释、回复或系统更新也会显示在较高级别对象的“更新”部分中。

例如，将更新添加到任务时，该更新会显示在任务的“更新”部分以及包含该任务的项目的“更新”部分中。

下表显示其注释也显示在较高排名的对象上的对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>添加了原始更新的对象</strong> </th> 
   <th> <p><strong>原始更新也出现的较高级对象</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>问题</td> 
   <td>项目</td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>项目</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>Portfolio项目</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>文档 </td> 
   <td>附加文档的对象，项目 </td> 
  </tr> 
 </tr> 
  <tr data-mc-conditions=""> 
   <td>校样 </td> 
   <td>文档 </td> 
  </tr>

<tr> 
   <td>项目群</td> 
   <td>项目组合</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>团队</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td><p>用户、团队</p>
   <p><b>注释</b></p>
   <p>时间表备注显示在做出备注的用户的“更新”部分及其主页团队的“更新”部分。</p>
   </td> 
  </tr> 
  <tr> 
   <td>模板任务</td> 
   <td>模板</td> 
  </tr> 
  <tr> 
   <td>叙述</td> 
   <td>迭代，团队</td> 
  </tr> 
  <tr> 
   <td>开发周期</td> 
   <td>团队</td> 
  </tr>

<tr> 
   <td>结果</td> 
   <td>目标</td> 
  </tr> 
  <tr> 
   <td>活动</td> 
   <td>目标</td> 
  </tr> 
 </tbody> 
</table>

<!--info for April 11: hide the note below-->

<!--
>[!NOTE]
>
>Replies added to system updates do not roll up to the parent object. Only direct replies on a child object and replies added to existing updates roll up to parent objects.
>
>For information about the object hierarchy in Adobe Workfront, see [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> It is not possible to reply to system updates in the new commenting experience. For more information, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
-->


## “更新”部分的限制

团队的“更新”部分以及代表其他用户输入更新时，存在一些限制。

### 有关用户和团队的注意事项

查看用户和团队的更新时，请考虑以下事项：

* 您无法在团队的“更新”部分中添加新注释。

* 您可以向在团队中查看的更新添加回复。 回复显示在团队的“更新”部分以及它所属对象的更新部分中。

* 在用户和团队的更新部分中，您可以查看在过去90天内输入的更新。

  如果想要在90天限制之外查看对用户或团队进行的所有更新，您可以构建注释报表。 报告不应具有显示针对用户或团队所做所有更新的时间过滤器。 有关详细信息，请参阅[创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

* 团队的“更新”部分由添加到以下对象的注释填充：

   * 用户
   * 故事
   * 时间表
   * 迭代

* 用户更新区域的“系统更新”选项卡通过更新其他对象来填充。 以下是在用户配置文件的系统更新选项卡中显示的更新，当这些字段在设置的更新馈送区域中受到跟踪时：

   * 文档添加、删除和其他文档更新
   * 小时添加、删除、代表添加以及其他小时条目更新
   * 注释，自定义字段的更新
   * 用户配置文件更新（更新了用户的头像、手机号码、与我谈论字段、标题）
   * 用户添加、删除、访问级别更改、内置用户字段更改
   * 来自任务和项目的财务信息。

### 代表其他用户输入评论时的限制

Adobe Workfront管理员和组管理员可以其他用户身份登录，并在Workfront中执行操作，例如输入注释。

有关信息，请参阅[以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)。

以其他用户身份登录并添加注释时，请考虑以下事项：

* 代表其他用户所做的任何评论都将在评论中标明。

* 组管理员可以代表他人进行评论，但无法删除该评论。 只有Adobe Workfront管理员可以删除他们代表其他用户所做的评论。

* 仅当Workfront或组管理员以其他用户身份注销并以他们自己身份重新登录时，才能编辑他们代表其他用户添加的评论。 他们不能代表其他用户删除评论。

## 使用日记帐分录报表查看工作项的系统更新

日志条目报表从项目、任务和问题的更新区域显示系统更新。

该报告允许您查看：

* 发生了多少次状态更改
* 删除任务或问题时
* 重要自定义字段中的值在项目过程中如何变化
* 项目过程中更改了哪些重要日期
* 如果在项目过程中优先级发生了更改
* 如果项目所有者已更改

有关详细信息，请参阅日志条目报告[的](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)更新区域报告。
