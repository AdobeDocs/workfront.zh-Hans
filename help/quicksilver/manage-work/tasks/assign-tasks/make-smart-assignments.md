---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 进行智能分配
description: 您可以使用智能分配来确定谁是完成工作的最佳用户。 智能分配是指Adobe Workfront在您根据确定最适合工作的资源的算法将工作项分配给资源时向您提供的用户、角色或团队建议。 有关智能分配的信息，请参阅智能分配概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 进行智能分配

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">此页面上高亮显示的信息指的是“生产”环境中仅供启用快速版本的客户使用的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">对于在2025年1月通过25.1版本启用快速发布的客户，此功能将从生产环境中删除。 有关25.1版本的信息，请参阅[2025年第一季度版本概述](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md)。

您可以使用智能分配来确定谁是完成工作的最佳用户。

智能分配是指Adobe Workfront在将工作项分配给资源时向您显示的用户、角色或团队的建议。 Workfront的建议基于确定最适合作业的资源的算法。

<span class="preview">Workfront中有两个单独的算法可计算在任务和问题中工作方式不同的智能分配。</span>

有关确定智能分配时使用的条件的详细信息，请参阅[智能分配概述](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md)。

## 访问要求

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
   <td> <p>新增：标准</p>
      或
      <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和问题的访问权限</p> <p>查看项目或授予更高的项目访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或更高权限，能够进行任务和问题分配</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 进行智能分配

智能分配适用于大多数您可以在Workfront中进行分配的位置。

1. 转到以下区域并单击&#x200B;**工作总揽**&#x200B;或&#x200B;**将此工作总揽分配给**&#x200B;字段：

   * 任务、问题列表或报告
   * 任务或问题标题
   * 任务或问题摘要面板
   * <span class="preview">新任务</span>或新问题框，因为您向项目中添加了<span class="preview">新任务</span>或问题
   * 工作负载均衡器中的任务或问题

1. 将光标置于Assignments字段中，并等待两秒钟。

   对于问题，智能分配会显示在以下部分中：

   * **用户和团队**
   * **职位角色**

   ![](assets/smart-assignments-issue-header.png)

   对于任务，智能分配会根据算法计算的哪个阶段标识了分配，显示在以下部分中：

   * <span class="preview">**建议的分配**：显示任务智能分配算法第一阶段中识别的分配。</span>
   * **用户和团队**、**工作角色**&#x200B;或&#x200B;<span class="preview">**评级卡片工作角色**</span>：在任务智能分配算法计算的第二阶段中识别的分配。

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   有关详细信息，请参阅[智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

1. 在推荐列表中选择资源，方法是单击资源的名称。

1. （可选）单击&#x200B;**分配给我**&#x200B;以将工作项分配给您自己。

   >[!TIP]
   >
   >如果没有建议，则不会打开建议列表。

1. （可选）如果不想使用智能分配列表中的推荐用户之一，请开始键入所需资源的名称，并在该名称出现在列表中时将其选定。
1. 单击&#x200B;**Enter**&#x200B;进行分配。

   选定的用户已分配给任务或问题。
