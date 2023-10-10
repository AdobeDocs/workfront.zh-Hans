---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 系统项目状态
description: Workfront具有9个内置的系统项目状态。 下表中的前3个是必需的，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。 更改项目状态通常是手动过程。 但是，有时项目状态会自动更改，具体取决于系统中发生的其他因素。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1572'
ht-degree: 0%

---

# 系统项目状态

Workfront具有9个内置的系统项目状态。

下表中的前3个是必需的，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。

更改项目状态通常是手动过程。 但是，当项目状态根据系统中发生的其他因素自动更改时，下面列出了一些场景。

您的Workfront实例提供了以下项目状态：

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
   <th>此项目状态发生于</th> 
   <th>此状态中发生的情况</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planning（必需状态）</td> 
   <td> <p>项目经理正在规划项目的时间表、任务分配和批准。 项目经理在项目上手动设置此状态。</p> <p><b>提示</p> <p> 我们建议您在Workfront中为新项目将默认状态设置为Planning。 作为Workfront管理员，您可以在项目偏好设置的项目区域中更改所有新项目的默认状态。</p> </td> 
   <td> <p>默认情况下，项目团队中的用户可在其“项目”列表（没有自定义过滤器）的Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题未填充他们的工作列表。 主页工作列表中仅显示批准和已接受的工作项。</p> <p>当项目具有此状态时，不发送通知。</p> <p>我们建议在项目处于“计划”状态时进行所有可能触发项目时间线更新的更改，或任何对任务和问题分配的更改。 这会最大限度地减少用户收到的通知数量。</p> <p>系统不会自动计算项目的时间表。</p> </td> 
  </tr> 
  <tr> 
   <td>当前（必需状态）</td> 
   <td> <p>用户正在处理它。 项目经理应将项目转换为“当前”以表示项目已启动。</p> <p>这是Workfront中新项目的默认状态。</p> <p><b>提示</b></p>

<p> 作为Workfront管理员，您可以在项目偏好设置的项目区域中更改新项目的默认状态。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
   <td> <p>默认情况下，项目团队中的用户可在其“项目”列表（没有自定义过滤器）的Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题会填充他们的工作列表。 他们可以开始接受有关任务和问题的工作，并将其移至其工作列表。</p> <p>此外，在当前项目中，所有关于时间表更改、分配、所需操作和审批的通知都会发送给项目团队中的用户。</p> <p>如果项目的“更新类型”设置为“自动”、“更改时”或“自动和更改时”，则系统会自动计算项目的时间表。</p> <p>提示：当项目处于此状态时，最好将项目计划的调整保持在最低水平，这样用户不会收到太多通知。</p> </td> 
  </tr> 
  <tr> 
   <td>完成（必需状态）</td> 
   <td> <p> 项目已完成：</p> 
     <p>如果项目的“完成模式”设置为“手动”，则项目经理会手动选择此状态，以通知项目团队中的用户停止处理项目。</p> 
    <p>如果项目的完成模式设置为自动，则当项目中的所有任务和问题都标记为完成时，Workfront会自动将项目标记为完成。 
    <p><b>重要</b> </p>
    <p>仅当项目中的所有任务、问题和审批均已解决时，您才可以将项目标记为完成。</p> </td> 
   <td>
    <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题不会填充他们的工作请求或工作列表。 </p>
    <p>与项目相关的所有通知（状态更改通知除外）停止发送给项目团队中的用户。</p>
    <p>系统不再计算项目的时间表。 </p>
    <p>无法复制项目。</p>
    <p>您可以将项目标记为完成时阻止用户执行其他操作。 </p><p>有关如何限制对标记为完成的项目执行操作的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p></td> 
  </tr> 
  <tr> 
   <td>废弃</td> 
   <td>项目尚未完成，但由于障碍或范围变化，项目无法继续进行，已被放弃。 项目经理将状态更改为“停止”，以提醒项目团队中的用户，此项目将永远不会完成，并且他们不应再处理此项目。</td> 
   <td> <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题从他们的工作列表中消失。</p> <p>批准决策无法授予任务或问题。</p> <p>不会将有关时间表更改、分配、所需操作、审批的通知发送给项目团队中的用户。</p> <p>系统不会自动计算项目的时间表，因为该项目被视为已完成。</p> <p>您可以将项目标记为废弃时阻止用户执行某些操作。 有关如何限制对Dead项目执行操作的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>保持</td> 
   <td>项目尚未完成，但由于一些延误，项目需要暂时停止。 项目经理选择使用此状态来提醒项目团队中的用户在当前时间停止处理项目。</td> 
   <td> <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题从他们的工作列表中消失。 </p> <p>批准决策无法授予任务或问题。</p> <p>不会将有关时间表更改、分配、所需操作、审批的通知发送给项目团队中的用户。</p> <p> <p><b>注意</b>：将项目置于暂停状态时，项目的时间表未停止。 即使没有人在积极处理该项目，该项目仍可显示为“处于风险中”或“存在问题”。 再次将项目返回到当前状态时，可能需要手动调整剩余未完成任务的日期，以便项目可以显示更新的进度。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>请求时间</td> 
   <td>当项目请求中的业务案例完成并提交审批时，系统会自动将项目状态标记为已请求。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题未填充其工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）都不会发送给任何用户。</p> <p>系统不会自动计算项目的时间表。</p> </td> 
  </tr> 
  <tr> 
   <td>已批准</td> 
   <td>当项目请求中的业务案例获得批准时，项目状态自动标记为已批准。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队中的用户可在其“项目”列表（没有自定义过滤器）的Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题未填充他们的工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）都不会发送给任何用户。</p> <p>系统不会自动计算项目的时间表。 </p> </td> 
  </tr> 
  <tr> 
   <td>被拒绝</td> 
   <td>当项目请求的业务案例被拒绝时，项目状态自动标记为“已拒绝”。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题未填充他们的工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）都不会发送给任何用户。</p> <p>系统不会自动计算项目的时间表。</p> </td> 
  </tr> 
  <tr> 
   <td>想法</td> 
   <td>提交项目请求时，项目状态会自动标记为“想法”。 有关使用业务案例请求项目的更多信息，请参阅 <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">审核请求的项目</a>.</td> 
   <td> <p>默认情况下，项目团队中的用户在其“项目”列表中（没有自定义筛选条件）无法在Workfront的“项目”区域中查看项目。 项目上分配给他们的任务和问题未填充他们的工作列表。</p> <p>与项目相关的所有通知（状态更改通知除外）都不会发送给任何用户。</p> <p>系统不会自动计算项目的时间表。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>下列项目状态不能更改为“终止”、“暂挂”或“完成”状态：
>
>* 请求时间
>* 想法
>* 已批准
>* 已拒绝（或其等效项）
>
