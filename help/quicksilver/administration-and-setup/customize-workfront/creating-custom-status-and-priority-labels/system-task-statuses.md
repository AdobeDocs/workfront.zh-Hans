---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系统任务状态
description: Workfront中需要使用三个内置的系统任务状态，这意味着您可以对这三个状态进行解锁、重命名和重新排序，但无法隐藏或删除它们。 您还可以添加新的系统任务状态以匹配组织中的需求。 更改任务的状态通常是手动过程，但有时任务状态会根据系统中发生的其他因素自动更改。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 系统任务状态

Workfront中需要使用三个内置的系统任务状态，这意味着您可以对这三个状态进行解锁、重命名和重新排序，但无法隐藏或删除它们。

您还可以添加新的系统任务状态以匹配组织中的需求。

更改任务的状态通常是手动过程。 但是，当任务状态根据系统中发生的其他因素自动更改时，有时会在下表中列出这些情况。

您的Workfront实例提供了以下任务状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系统任务状态</th> 
   <th>当此状态出现时</th> 
   <th>任务处于此状态时执行的操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新建（必需状态）</td> 
   <td>这是每个新创建的任务的默认状态。</td> 
   <td>如果任务位于状态为“当前”的项目上，则任务会显示在分配给任务的用户的“工作请求”选项卡中。 用户现在可以开始处理该任务。</td> 
  </tr> 
  <tr> 
   <td>进行中（必需状态）</td> 
   <td>您可以将任务置于此状态，以指示该任务上的工作已开始。</td> 
   <td> <p>当您将任务标记为“进行中”时，该任务会显示“实际开始日期”的值。</p> <p>在您手动更新任务的完成百分比之前，不会记录任务的进度。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必需状态）</td> 
   <td> <p>您可以在任务完成时手动将其标记为完成。</p> <p>当任务的“跟踪模式”设置为“自动完成”时，当任务到达“计划完成日期”时，系统会自动将任务标记为“完成”。</p> </td> 
   <td> <p>任务完成后，任务的完成百分比将标记为100%。 任务完成后，该任务会从主页区域被分派人的“我的工作”列表中移除。</p> <p>将任务标记为“完成”时，该任务会显示“实际完成日期”的值。</p> <p><b>注意</b>：如果任务有未完成的问题，并且您将其状态更改为“完成”，则状态会自动更改为“完成 — 未决问题”。</p> </td> 
  </tr> 
 </tbody> 
</table>
