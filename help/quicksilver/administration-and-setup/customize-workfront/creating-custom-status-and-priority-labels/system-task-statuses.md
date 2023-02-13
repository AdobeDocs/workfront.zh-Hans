---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系统任务状态
description: Workfront中需要三种内置系统任务状态，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。 您还可以添加新的系统任务状态，以满足贵组织的需求。 更改任务状态通常是手动过程，但有时任务的状态会根据系统中发生的其他因素自动更改。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 系统任务状态

Workfront中需要三种内置系统任务状态，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。

您还可以添加新的系统任务状态，以满足贵组织的需求。

更改任务状态通常是手动过程。 但是，当任务的状态自动更改时，有时会在以下列表中列出，具体取决于系统中正在发生的其他因素。

随Workfront实例提供了以下任务状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系统任务状态</th> 
   <th>出现此状态时</th> 
   <th>任务处于此状态时发生的操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新（必需状态）</td> 
   <td>这是每个新创建任务的默认状态。</td> 
   <td>如果任务位于处于“当前”状态的项目上，则该任务会显示在分配给任务的用户的“工作请求”选项卡中。 用户现在可以开始处理该任务。</td> 
  </tr> 
  <tr> 
   <td>正在进行（必需状态）</td> 
   <td>您可以将任务置于此状态，以指示该任务的工作已开始。</td> 
   <td> <p>将任务标记为“正在进行”时，该任务会显示实际开始日期的值。</p> <p>在手动更新任务完成百分比之前，不会记录任务的进度。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必需状态）</td> 
   <td> <p>您可以在任务完成后手动标记任务完成。</p> <p>当任务的“跟踪模式”设置为“自动完成”时，任务在达到“计划完成日期”时会自动标记为“完成”。</p> </td> 
   <td> <p>任务完成后，任务完成百分比将标记为100%。 任务完成后，将从“主页”(Home)区域的被分派人的工作列表中移除该任务。</p> <p>将任务标记为完成时，该任务会显示实际完成日期的值。</p> <p><b>注意</b>:如果任务有未完成的问题，并且您将任务状态更改为“完成”，则状态会自动更改为“完成 — 待定问题”。</p> </td> 
  </tr> 
 </tbody> 
</table>
