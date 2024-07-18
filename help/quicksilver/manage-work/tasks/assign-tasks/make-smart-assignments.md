---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 进行智能分配
description: 您可以使用智能分配来确定谁是完成工作的最佳用户。 智能分配是指Adobe Workfront在您根据确定最适合工作的资源的算法将工作项分配给资源时向您提供的用户、角色或团队建议。 有关智能分配的信息，请参阅智能分配概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 进行智能分配

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

<span class="preview">有关当前版本的信息，请参阅[2024年第三季度版本概述](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md)。</span>

您可以使用智能分配来确定谁是完成工作的最佳用户。

智能分配是指Adobe Workfront在将工作项分配给资源时向您显示的用户、角色或团队的建议。 Workfront的建议基于确定最适合作业的资源的算法。

<span class="preview">Workfront中有两个单独的算法可计算在任务和问题中工作方式不同的智能分配。</span>

有关确定智能分配时使用的条件的详细信息，请参阅[智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 进行智能分配

智能分配适用于大多数您可以在Workfront中进行分配的位置。

1. 转到以下区域并单击&#x200B;**工作总揽**&#x200B;或&#x200B;**将此工作总揽分配给**&#x200B;字段：

   * 任务、问题列表或报告
   * 任务或问题标题
   * 任务或问题摘要面板
   * <span class="preview">新任务或新问题框，向项目添加新任务或问题</span>
   * “主页”区域中列出的项目的“工作总揽”字段
   * 工作负载均衡器中的任务或问题

1. 将光标置于Assignments字段中，并等待两秒钟。

   <div class="preview">
   将显示以下一个或多个包含智能分配建议的部分：

   * **建议的工作分配**：显示任务。<!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   列表标题显示&#x200B;**以下是生产环境中的一些推荐**&#x200B;而不是&#x200B;**建议分配**。
     >
   * **用户和团队**：显示任务和问题。
   * **工作角色**：显示任务和问题。
   * **为卡片工作角色评分**：显示任务。 有关详细信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)。<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   对于任务，智能分配会根据算法计算的哪个阶段标识了分配，显示在以下部分中：

   * **建议分配**：在任务智能分配算法计算的第一阶段中确定的分配。 <span class="preview">此分区不适用于问题。</span>
   * <span class="preview">**用户和团队**、**工作角色**&#x200B;或&#x200B;**评级卡片工作角色**：在任务智能分配算法计算的第二阶段中识别的分配。<!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   有关详细信息，请参阅[智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md)。

1. 单击推荐列表中的用户的名称，以选择该用户。

1. （可选）单击&#x200B;**分配给我**&#x200B;以将工作项分配给您自己。

   >[!TIP]
   >
   >如果没有建议，则不会打开建议列表。

1. （可选）如果不想使用智能分配列表中的推荐用户之一，请开始键入所需资源的名称，并在该名称出现在列表中时将其选定。
1. 单击&#x200B;**Enter**&#x200B;进行分配。

   选定的用户已分配给任务或问题。
