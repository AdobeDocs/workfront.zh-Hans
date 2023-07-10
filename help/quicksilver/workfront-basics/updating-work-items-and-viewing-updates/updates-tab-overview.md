---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新部分概述
description: 对象的“更新”部分显示用户对对象所做的注释或跟踪对象更改的系统更新。
author: Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 38f46324219f297523ff262b083f41a2dd388579
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 3%

---

# 更新部分概述

<!--take "Beta" references out when we remove the beta-->

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅适用于预览环境中的所有客户。</span>

>[!NOTE]
>
>我们目前正在重新设计Adobe Workfront中的评论体验。
>
>有关新评论体验的更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>您可以访问以下对象的新体验：
> * 问题， <span class="preview">项目、任务和文档</span>.
>
>     当您启用备注测试版体验时，该选项可用。
>
>     此功能仅适用于“更新”部分，不适用于以下区域：
>
>     * 主页
>     * 列表中的摘要面板
>     * 时间表中的“摘要”面板
>
> * 讨论区中的目标、信息卡
>
>   新的评论体验是目标和信息卡的唯一体验。 您必须拥有其他许可证才能访问Workfront目标。 有关更多信息，请参阅 [使用Workfront目标的要求](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     在信息卡上启用“注释”和“系统活动”部分时，您可以在“信息卡”区域中添加和查看信息卡的更新。 有关更多信息，请参阅 [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md).

对象的“更新”部分显示用户对对象所做的注释或跟踪对象更改的系统更新。

## “更新”部分的概述

根据您从中访问信息的环境，“更新”部分中的信息将以不同的方式组织。

### “当前更新”部分的概述

对象的“更新”部分显示过去90天内进行的最近200次更新。

![](assets/updates-tab-before-unified-experience-for-issues.png)

当前的“更新”部分显示以下信息：

* 用户发表的评论以及对这些评论的回复。
* 系统更新，Workfront创建的信息性消息，用于记录对象上的特定事件。 例如，您可以使用系统更新捕获状态、名称或自定义字段中的更改。 您的Workfront或组管理员可以为您的对象启用系统更新。 有关更多信息，请参阅 [配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

“更新”部分显示以下对象：

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
     <li>故事*</li> 
     <li>任务</li> 
     <li>模板</li> 
     <li>模板任务</li> 
     <li>时间表</li> 
     <li>用户</li>
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
*故事是任务。 所有与任务相关的信息也可用于故事。

### Beta版评论体验中“更新”部分的概述

![](assets/updates-tab-after-unified-experience-for-issues.png)

有关哪些功能可用于新注释体验以及哪些对象的信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

“更新”部分在新注释体验的以下选项卡中显示信息：

* **注释**：显示用户所做的评论以及对这些评论的回复。 有关更新新注释体验中的对象的信息，请参见 [更新工作](../updating-work-items-and-viewing-updates/update-work.md).
* **系统活动**：显示系统更新，这些是信息性消息，由Workfront创建，用于记录对象上的某些事件。 例如，您可以使用系统更新捕获状态、名称或自定义字段中的更改。 您的Workfront或组管理员可以为您的对象启用系统更新。 有关更多信息，请参阅 [配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

目前，您可以在以下对象上使用新的注释体验添加注释和回复更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><p>目标</p>
     <li>展示板区域中的信息卡*</li>
      这是唯一的目标和卡片体验。
     </li> 
     <li><span class="preview">项目</span></li>
    </ul> </td> 
   <td> 
    <ul> 
     <li>问题</li> 
     <li><span class="preview">任务</span></li>
     <li><span class="preview">文档</span></li>
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

*在信息卡上启用“备注”和“系统活动”部分时，您可以在信息卡区域中添加和查看信息卡的更新。 有关更多信息，请参阅 [向展示板添加临时信息卡](../../agile/get-started-with-boards/add-card-to-board.md).

## 更新也会显示在较高级别的对象中

对特定对象更新所做的注释或回复也会显示在较高排名对象的“更新”部分中。

例如，将更新添加到任务时，该更新会显示在任务的更新部分以及包含该任务的项目的更新部分中。

>[!NOTE]
>
>启用新的备注测试版体验时，备注会显示在以下排名较高的对象上：
>
>* 问题
>* <span class="preview">项目</span>
>* <span class="preview">任务</span>
>
>有关更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

下表显示其注释也显示在较高排名的对象上的对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>添加了原始更新的对象</strong> </th> 
   <th> <p><strong>还会显示原始更新的更高排名对象</strong> </p> </th> 
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
>添加到系统更新的回复不会汇总到父对象。 只有对子对象的直接回复和添加到现有更新的回复会汇总到父对象。
>
>有关Adobe Workfront中对象层次的信息，请参阅 [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
>
> 无法回复新评论测试版体验中的系统更新。 有关更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

## “更新”部分的限制

团队的更新部分和代表其他用户输入更新时，存在一些限制。

### 用户和团队的限制

您无法对团队进行更新。 团队的“更新”部分由在以下对象中输入的更新填充：

* 用户
* 时间表
* 故事
* 迭代

在用户和团队的更新部分中，您可以查看在过去90天内输入的更新。

如果要查看对用户或团队进行的所有更新（超过90天的限制），您可以构建注释报表。 报告不应具有显示针对用户或团队所做所有更新的时间过滤器。 有关更多信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### 代表其他用户输入评论时的限制

Adobe Workfront管理员和组管理员可以其他用户身份登录，并在Workfront中执行输入注释等操作。

有关信息，请参阅 [以其他用户身份登录](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

代表其他用户所做的任何评论都将显示在评论中。

>[!NOTE]
>
><span class="preview">使用新的评论体验时，评论添加为以其他用户身份登录的用户，并且没有迹象表明他们代表其他人添加评论。
>
>例如，如果Workfront管理员以其他用户身份登录，则与评论关联的用户是Workfront管理员。 有关更多信息，请参阅 [新的评论体验](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


组管理员可以代表他人发表评论，但不能删除该评论。 只有Adobe Workfront管理员可以删除他们代表其他用户所做的评论。

## 使用日记帐分录报表查看工作项的系统更新

日志条目报表显示项目、任务和问题的更新区域中的系统更新。

该报告允许您查看：

* 发生了多少个状态更改
* 删除任务或问题时
* 重要自定义字段中的值在项目过程中如何变化
* 项目过程中更改了哪些重要日期
* 如果在项目过程中优先级发生变化
* 如果项目所有者已更改

有关更多信息，请参阅 [报告“更新”区域](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
