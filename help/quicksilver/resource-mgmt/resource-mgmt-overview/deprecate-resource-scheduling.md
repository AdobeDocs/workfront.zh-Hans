---
content-type: reference
product-area: resource-management
keywords: 工作负载，平衡器
navigation-topic: resource-management-overview
title: 弃用Adobe Workfront中的资源计划工具
description: 我们当前正在弃用Adobe Workfront中的所有计划工具，并用工作负载平衡器替换它们。
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# 弃用Adobe Workfront中的资源计划工具

>[!IMPORTANT]
>  
><span class="preview">自2023年1月的23.1版本开始，本文中描述的计划功能已弃用并从Adobe Workfront中删除。   </span>
>  
> <span class="preview"> 2023年初23.1版发布后不久，也将删除本文。 此时，我们建议您相应地更新任何书签。 </span>
> 
><span class="preview"> 您现在可以使用负载平衡器来计划资源的工作。 </span>
>  
> <span class="preview">有关使用工作负载平衡器计划资源的信息，请参阅一节 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## 您应如何准备

有关如何准备在调度和负载平衡器之间进行过渡的详细信息，请参阅 [从资源计划迁移到负载平衡器](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

如果您当前使用计划工具，我们建议您停用这些工具并开始使用工作负载平衡器。

![全局资源计划区域](assets/resource-scheduler-global-350x127.png)

几乎所有以前在计划区域中可用的功能现在都在负载平衡器中可用。 有关信息，请参阅 [功能可用性](#feature-availability) 在本文中。 您可以继续安排资源在工作负载平衡器中专门工作。

![全局工作负载平衡器区域](assets/workload-balancer-pti-350x111.png)

## 不会传输到工作负载平衡器的信息

以下信息不会从计划工具传输到工作负载平衡器：

* **用户的每日分配**:您不应同时使用计划和负载平衡器来调整相同的用户分配。 如果您在“计划”工具中管理了用户分配，则调整后的每日分配不会转移到工作负载平衡器。 同样，如果已在负载平衡器中调整了用户分配，则它们不会转移到计划工具。 我们强烈建议您确保工作负载平衡器中的每日分配准确，以便为此过渡做好准备。 有关信息，请参阅 [在工作负载平衡器中管理用户分配](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **过滤器**:如果已在“计划”区域中保存过滤器，则它们不会传输到工作负载平衡器。 必须在工作负载平衡器中重新创建过滤器。 有关信息，请参阅 [在工作负载平衡器中筛选信息](../workload-balancer/filter-information-workload-balancer.md).

## 弃用时间线亮点

>[!IMPORTANT]
>
>阅读本文，了解弃用计划工具的最新时间轴。 本文和公告中心报文中将提供对此时间表的任何更新。

以下是资源计划工具弃用过程的时间表：

* [2020.4版（2020年11月）](#2020-4-release-november-2020)
* [2021.4版本（2021年10月）](#2021-4-release-october-2021)
* [2022.4 - 2023.1版（2022年10月 — 2023年1月）](#2022-4-2023-1-releases)

### 2020.4版（2020年11月） {#2020-4-release-november-2020}

* 计划解决方案不再实施新功能
* 只有高严重性和严重性缺陷才能优先进行修复
* 向Workfront添加了新的工作负载平衡器功能

### 2021.4版本（2021年10月） {#2021-4-release-october-2021}

* 对于任何首次使用Workfront的用户，工作负载平衡器都设置为默认值
* 可共享并包含其他字段的增强过滤器

### 2022.4 - 2023.1版（2022年10月 — 2023年1月） {#2022-4-2023-1-releases}

* 在2022.4或2023.1版本发行期间和之后，对于修复的缺陷，不会优先考虑任何缺陷
* 所有计划区域都将从预览环境(**2022年10月20日**)
* 所有计划区域都将从生产环境中删除(**2023年1月**)
* 工作负载平衡器是Workfront中唯一可用的资源调度工具(在 **2023年1月**)

## 功能可用性 {#feature-availability}

除非另有指定，否则所有资源计划功能已在负载平衡器中可用或将可用。 有关工作负载平衡器的信息，请参阅 [工作负载平衡器概述](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

除了现有功能外，负载平衡器还具有或将具有资源计划工具中不存在的新功能，如下表所示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>功能</b></span> </td> 
   <td rowspan="2"> <b>资源计划工具功能可用性</b></td> 
   <td colspan="3"><b>工作负载平衡器功能可用性</b></td> 
  </tr> 
  <tr> 
   <td><b>现已可用</b></td> 
   <td><b>即将推出</b></td> 
   <td><b>未计划</b></td> 
  </tr> 
  <tr> 
   <td> <p>从“资源”区域访问工具</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>为未分配和已分配的工作分开区域</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>为未分配和已分配的工作应用和创建过滤器</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>直接从工具访问工作项</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>手动分配或取消分配任务和问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>调整单个分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>包括发布时间</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>显示预计日期 </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>显示已完成的工作</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>显示用户休息时间、周末和计划例外</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>根据角色快速分配用户*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>快速更换用户*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>快速取消分配用户*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>团队中的访问工具</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>从项目访问工具</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>工作许可证用户在从项目访问工作负载平衡器时可以调整用户分配 </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>在“未分配的工作”区域中显示问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>通过拖放来分配和取消分配任务和问题*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>对所有计划用户都可见，而未在项目中指定资源管理器。</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>按项目分组信息</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>与无法访问资源区域的用户共享工作负载平衡器</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>按周显示和调整分配</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>直接从工具访问用户</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>使用“摘要”面板，无需导航即可访问有关工作项的更多信息*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>以百分比值显示和调整分配 </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>显示可用时间与已分配时间之差</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在图表中显示用户可用性</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>按项目状态对工作项和项目进行颜色代码</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>在调整用户分配时自动更新计划小时数（对于具有简单持续时间类型的任务）</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>根据用户的分配模式、现有角色或团队分配建议分配</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>可共享并包含其他字段的增强过滤器</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>进行高级分配</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>按项目和项目状态对工作项进行颜色编码</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>将用户添加到项目团队(已调整到 <b>人员</b> 选项卡) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>自动分配任务和问题</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*这些功能仅在新的Adobe Workfront体验中可用。
