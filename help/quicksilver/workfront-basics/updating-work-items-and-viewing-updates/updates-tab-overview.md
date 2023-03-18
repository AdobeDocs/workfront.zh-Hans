---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新部分概述
description: “更新”部分显示了过去90天内最近进行的200次更新。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# 更新部分概述

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

对象的“更新”部分显示用户对跟踪对象更改的对象或系统更新所做的注释。

## 更新部分概述

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

对象的“更新”部分显示了过去90天内最近进行的200次更新。

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

“更新”部分显示以下信息：

* 用户的评论以及对这些评论的回复。
* 系统更新，这些信息性消息是Workfront创建的，用于记录对象上的某些事件。 例如，您可以通过系统更新捕获状态、名称或自定义字段中的更改。 您的Workfront或组管理员可以为您的项目启用系统更新。 有关更多信息，请参阅 [配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

将显示以下对象的“更新”部分：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>文档</li> 
     <li>目标</li> 
     <li>问题</li> 
     <li>迭代</li> 
     <li>项目</li> 
     <li>项目群</li> 
     <li>项目组合</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>故事</li> 
     <li>任务</li> 
     <li>模板</li> 
     <li>模板任务</li> 
     <li>时间表</li> 
     <li>用户</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## 也显示在较高级别对象上的更新

如下表所示，对某些对象的更新所做的回复也会显示在排名较高的对象的“更新”部分。

例如，在向任务添加更新时，该更新将显示在任务的“更新”部分和包含该任务的项目的“更新”部分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>添加原始更新的对象</strong> </th> 
   <th> <p><strong>还显示原始更新的排名较高的对象</strong> </p> </th> 
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
   <td>项目，Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>文档 </td> 
   <td>附加文档的对象，项目 </td> 
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
   <td>用户、团队</td> 
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
   <td>迭代</td> 
   <td>团队</td> 
  </tr>

<tr> 
   <td>目标</td> 
   <td>结果，活动</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>添加到系统更新的回复不会汇总到父对象。 只有对子对象的直接回复和添加到现有更新的回复才会汇总到父对象。
>
>有关Adobe Workfront中对象层次结构的信息，请参阅 [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## “更新”部分的限制

### 用户和团队的限制

无法对团队进行更新。 团队的“更新”部分由在以下对象上输入的更新填充：

* 用户
* 时间表
* 故事
* 迭代

在用户和团队的“更新”部分中，您可以查看过去90天内输入的更新。

如果您想要查看对用户或团队所做的所有更新（超出90天限制），则可以构建报表以进行注释。 报表不应具有时间过滤器来显示为用户或团队进行的所有更新。 有关更多信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他用户输入评论时的限制

Adobe Workfront管理员和组管理员可以以其他用户身份登录，并在Workfront中执行一些操作，如输入注释。 (有关信息，请参阅 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) 代表其他用户发表的任何评论都会在评论中指出。

群组管理员可以代表他人进行评论，但无法删除该评论。 只有Adobe Workfront管理员才能删除他们代表其他用户发表的评论。

## 使用日记帐分录报表查看工作项的系统更新

“日记帐分录”报表显示系统从项目、任务和问题的“更新”区域进行的更新。

报表允许您查看：

* 发生了多少次状态更改
* 删除任务或问题时
* 重要自定义字段中的值在项目过程中有何变化
* 在项目过程中，哪些重要日期发生了更改
* 如果在项目过程中优先级发生了更改
* 如果项目的所有者发生更改

有关更多信息，请参阅 [报告更新区域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
