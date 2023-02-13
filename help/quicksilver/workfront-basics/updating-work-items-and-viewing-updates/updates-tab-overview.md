---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: “更新”选项卡概述
description: “更新”选项卡会显示过去90天内最近进行的200次更新。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 799a2f3463ee98d57b13edfda8a0c93629439ea3
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 6%

---

# “更新”选项卡概述

“更新”选项卡会显示过去90天内最近进行的200次更新。 您可以回复以下对象的更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>项目</li> 
     <li>项目组合</li> 
     <li>项目群</li> 
     <li>模板</li> 
     <li>模板任务</li> 
     <li>任务</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>问题</li> 
     <li>迭代</li> 
     <li>故事</li> 
     <li>用户</li> 
     <li>文档</li> 
     <li>时间表</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 也显示在较高级别对象上的更新

如下表所示，对某些对象的更新所做的回复也会显示在排名较高的对象的“更新”(Updates)选项卡中。

例如，在向任务添加更新时，该更新会显示在任务的“更新”选项卡和包含该任务的项目的“更新”选项卡中。

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
 </tbody> 
</table>

>[!NOTE]
>
>添加到系统更新的回复不会汇总到父对象。 只有对子对象的直接回复和添加到现有更新的回复才会汇总到父对象。

有关Adobe Workfront中对象层次结构的信息，请参阅 [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## “更新”选项卡的限制

### 用户和团队的限制

无法对团队进行更新。 团队的“更新”(Updates)选项卡由在以下对象上输入的更新填充：

* 用户
* 时间表
* 故事
* 迭代

在用户和团队的更新选项卡上，您可以查看过去90天内输入的更新。

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
