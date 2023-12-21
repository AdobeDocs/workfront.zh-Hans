---
product-area: projects;user-management
navigation-topic: assign-tasks
title: 进行智能分配
description: 您可以使用智能分配来确定谁是完成工作的最佳用户。 智能分配是在您根据确定最适合作业的资源的算法将工作项分配给资源时，Adobe Workfront向您提供的用户建议。 有关智能分配的信息，请参阅智能分配概述。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 94d3fc1715d32531962a1b7405850c0b2944c776
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# 进行智能分配

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它仅在“预览”环境中对所有客户可用。</span>

<span class="preview">有关当前发行计划的信息，请参阅 [2024年第一季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

您可以使用智能分配来确定谁是完成工作的最佳用户。 智能分配是在您根据确定最适合作业的资源的算法将工作项分配给资源时，Adobe Workfront向您提供的用户建议。 有关智能分配的信息，请参见 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p>
      或
      <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和问题的访问权限</p> <p>查看项目或授予更高的项目访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>Contribute或更高权限，能够分配任务和问题</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 进行智能分配

智能分配适用于大多数您可以在Workfront中进行分配的位置。

1. 转到以下区域，然后单击 **指定任务** 或 **将此分派至** 字段：

   * 任务、问题列表或报告
   * 任务或问题标题
   * 任务或问题摘要面板
   * “主页”区域中列出的项目的“工作总揽”字段
   * 工作负载均衡器中的任务或问题

1. 将光标置于任务字段中，并等待两秒钟。

   <span class="preview">此 **建议的工作分配** 列表随即显示。</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   此时将显示列表标题 **以下是一些建议** 而不是 **建议的工作分配** 在问题列表中。

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   此列表中显示的用户是任务或问题的智能分配建议。

   有关智能分配显示位置的更多信息，请参阅文章中的“查找智能分配建议”部分 [智能分配概述](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. 单击推荐列表中的用户的名称，以选择该用户。

1. （可选）单击 **分配给我** 以将工作项分配给您自己。

   >[!TIP]
   >
   >如果没有建议，则不会打开建议列表。

1. （可选）如果不想使用智能分配列表中的推荐用户之一，请开始键入所需用户的名称，并在该名称出现在列表中时将其选定。
1. 单击 **输入** 进行分配。

   选定的用户已分配给任务或问题。
