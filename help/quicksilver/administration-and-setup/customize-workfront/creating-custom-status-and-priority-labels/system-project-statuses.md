---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系统项目状态
description: Workfront具有9个内置系统项目状态。 下表中的前3个是必需的，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。 更改项目状态通常是手动过程。 但是，有时项目状态会根据系统中发生的其他因素自动进行更改。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# 系统项目状态

Workfront具有9个内置系统项目状态。

下表中的前3个是必需的，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。

更改项目状态通常是手动过程。 但是，当项目状态自动更改时，根据系统中发生的其他因素，下面的列表中会列出一些情景。

随您的Workfront实例提供了以下项目状态：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>系统项目状态</th> 
   <th>此项目状态发生在</th> 
   <th>此状态中会发生什么情况</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>计划（必需状态）</td> 
   <td> <p>项目经理正在规划项目的时间表、任务的分配和批准。 项目经理会在项目中手动设置此状态。</p> <p>提示：我们建议您将Workfront中新项目的默认状态设置为Planning。 作为Workfront管理员，您可以在项目首选项的项目区域中更改所有新项目的默认状态。</p> </td> 
   <td> <p>默认情况下，项目团队的用户可以在其项目列表的Workfront项目区域中看到项目。 项目中分配给他们的任务和问题不会填充其工作列表。 只有批准和已接受的工作项目才会显示在“主页工作列表”中。</p> <p>项目处于此状态时不会发送通知。</p> <p>我们建议在项目处于“计划”状态时进行所有可触发项目时间轴更新的更改，或对任务和问题分配所做的任何更改。 这样可最大限度地减少用户收到的通知数量。</p> <p>系统不会自动计算项目的时间轴。</p> </td> 
  </tr> 
  <tr> 
   <td>当前（必需状态）</td> 
   <td> <p>用户正在处理它。 项目经理应将项目转为“当前”，以表示项目已开始。</p> <p>这是Workfront中新项目的默认状态。</p> <p>提示：作为Workfront管理员，您可以在项目首选项的项目区域中更改新项目的默认状态。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
   <td> <p>默认情况下，项目团队的用户可以在其项目列表的Workfront项目区域中看到项目。 项目中分配给他们的任务和问题将填充其工作列表。 他们可以开始接受有关任务和问题的工作，并将其移至“工作”列表。</p> <p>此外，在“当前”项目上，所有有关时间轴更改、分配、所需操作和批准的通知都会发送给项目团队中的用户。</p> <p>如果项目的“更新类型”设置为“自动”、“更改时”或“自动”和“更改时”，则系统会自动计算项目的时间轴。</p> <p>提示：最好在项目处于此状态时将项目计划调整保持在最低程度，以便用户不会收到太多通知。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必需状态）</td> 
   <td> <p> 项目已完成：</p> 
    <ul> 
     <li> <p>如果项目的“完成模式”设置为“手动”，项目经理将手动选择此状态，以通知项目团队的用户停止处理项目。</p> </li> 
    </ul> 
    <ul> 
     <li>如果项目的“完成模式”设置为“自动”，则当项目中的所有任务和问题都标记为“完成”时，Workfront会自动将项目标记为“完成”。 </li> 
    </ul> <p><b>重要信息</b>:只有在项目的所有任务、问题和批准都得到解决后，才能将项目标记为已完成。</p> </td> 
   <td>
    <ul>
     <li>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 在项目中分配给他们的任务和问题不会填充他们的工作请求或处理列表。</li>
     <li>与项目相关的所有通知（状态更改通知除外）均停止发送给项目团队中的用户。 </li>
     <li>系统不再计算项目的时间轴。</li>
     <li>无法复制项目。</li>
    </ul><p>当项目标记为完成时，您可以阻止用户执行其他操作。 </p><p>有关如何对标记为“完成”的项目限制操作的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p></td> 
  </tr> 
  <tr> 
   <td>废弃</td> 
   <td>该项目尚未完成，但由于存在障碍或范围更改，该项目无法继续运行且已被放弃。 项目经理将状态更改为“无效”，以提醒项目团队中的用户此项目将永远无法完成，他们不应再继续处理该项目。</td> 
   <td> <p>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 在项目中分配给他们的任务和问题会从其工作列表中消失。</p> <p>不能对任务或问题做出批准决定。</p> <p>有关时间轴更改、分配、所需操作和批准的通知不会发送给项目团队中的用户。</p> <p>由于项目被视为已完成，因此系统不会自动计算项目的时间表。</p> <p>当项目标记为“已停用”时，您可以阻止用户执行某些操作。 有关如何限制对“无效”项目的操作的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>保持</td> 
   <td>项目尚未完成，但由于某些延误，项目需要暂时暂停。 项目经理选择使用此状态来提醒项目团队中的用户在当前时间停止处理项目。</td> 
   <td> <p>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 在项目中分配给他们的任务和问题会从其工作列表中消失。 </p> <p>不能对任务或问题做出批准决定。</p> <p>有关时间轴更改、分配、所需操作和批准的通知不会发送给项目团队中的用户。</p> <p> <p><b>注意</b>:将项目置于暂挂状态时，项目的时间轴不会停止。 即使没有人在积极处理项目，项目仍会显示为“处于风险或处于故障”。 再次将项目恢复到“当前”时，可能需要手动调整剩余未完成任务的日期，以便项目可以显示更新的进度。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>已请求</td> 
   <td>当项目请求的业务案例已完成并提交审批时，系统会自动将项目状态标记为“请求”。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 分配给他们的项目中的任务和问题不会填充他们的工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）均不会发送给任何用户。</p> <p>系统不会自动计算项目的时间轴。</p> </td> 
  </tr> 
  <tr> 
   <td>已批准</td> 
   <td>当项目请求的业务案例获得批准时，项目状态会自动标记为已批准。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队的用户可以在其项目列表的Workfront项目区域中看到项目。 项目中分配给他们的任务和问题不会填充其工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）均不会发送给任何用户。</p> <p>系统不会自动计算项目的时间轴。 </p> </td> 
  </tr> 
  <tr> 
   <td>被拒绝</td> 
   <td>当项目请求的业务案例被拒绝时，项目状态会自动标记为已拒绝。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 项目中分配给他们的任务和问题不会填充其工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）均不会发送给任何用户。</p> <p>系统不会自动计算项目的时间轴。</p> </td> 
  </tr> 
  <tr> 
   <td>想法</td> 
   <td>在您提交项目请求时，项目状态会自动标记为构思。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队的用户在其项目列表的Workfront的项目区域中看不到该项目。 项目中分配给他们的任务和问题不会填充其工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）均不会发送给任何用户。</p> <p>系统不会自动计算项目的时间轴。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>以下项目状态不能更改为“无效”、“暂挂”或“完成”状态：
>
>* 已请求
>* 想法
>* 已批准
>* 已拒绝（或其等效项）
>

