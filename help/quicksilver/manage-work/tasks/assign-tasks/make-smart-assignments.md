---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 进行智能分配
description: 您可以使用智能分配来确定谁是完成工作的最佳用户。 智能分配是指Adobe Workfront在您根据确定最适合工作的资源的算法将工作项分配给资源时向您提供的用户、角色或团队建议。 有关智能分配的信息，请参阅智能分配概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# 进行智能分配

<!--Audited: 02/2024-->

{{preview-and-fast-release}}

您可以使用智能分配来确定谁是完成工作的最佳用户。

智能分配是指Adobe Workfront在将工作项分配给资源时向您显示的用户、角色或团队的建议。 Workfront的建议基于确定最适合作业的资源的算法。

<span class="preview">Workfront中有两种单独的算法用于处理任务和问题。 </span>

有关确定智能分配时使用的标准的更多信息，请参阅 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

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
   <td> <p>Contribute或更高权限，能够分配任务和问题</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 进行智能分配

智能分配适用于大多数您可以在Workfront中进行分配的位置。

1. 转到以下区域，然后单击 **指定任务** 或 **将此分派至** 字段：

   * 任务、问题列表或报告
   * 任务或问题标题
   * 任务或问题摘要面板
   * <span class="preview">“新任务”或“新问题”框</span>
   * “主页”区域中列出的项目的“工作总揽”字段
   * 工作负载均衡器中的任务或问题

1. 将光标置于任务字段中，并等待两秒钟。

   <span class="preview">此 **建议的工作分配** 列表随即显示。</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   此时将显示列表标题 **以下是一些建议** 而不是 **建议的工作分配** 在问题列表中。

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   对于问题，智能分配建议显示在 **建议的分配** 区域。

   对于任务，智能分配会根据算法计算的哪个阶段标识了分配，显示在以下部分中：

   * **建议的分配**：在任务智能分配算法计算的第一阶段中识别的分配。
   * <span class="preview">**其他分配**：在任务智能分配算法计算的第二阶段中识别的分配。 此部分不适用于问题。 </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   有关更多信息，请参阅 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. 单击推荐列表中的用户的名称，以选择该用户。

1. （可选）单击 **分配给我** 以将工作项分配给您自己。

   >[!TIP]
   >
   >如果没有建议，则不会打开建议列表。

1. （可选）如果不想使用智能分配列表中的推荐用户之一，请开始键入所需资源的名称，并在该名称出现在列表中时将其选定。
1. 单击 **输入** 进行分配。

   选定的用户已分配给任务或问题。
