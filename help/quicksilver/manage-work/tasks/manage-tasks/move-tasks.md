---
product-area: projects
navigation-topic: manage-tasks
title: 移动任务
description: 您可以在Adobe Workfront中将任务移动到不同的项目或不同的父任务。
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 23a08c929b0a227c7a555af70ff731ef2df7a179
workflow-type: tm+mt
source-wordcount: '1360'
ht-degree: 2%

---

# 移动任务

您可以在Adobe Workfront中的以下对象之间移动任务：

* 项目的临时任务。
* 从项目到其他项目的任务。
* 另一个项目中不同父项下的项目任务。
* 同一项目中不同父项下的任务。

您可以在任务级别移动任务，也可以从任务列表中移动任务。

## 访问要求

您必须具有以下访问权限才能执行本文中的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>能够添加任务的项目的参与者或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在列表中移动任务

要移动任务列表中显示的任务，请执行以下操作：

1. 转到包含要移动的任务或任务的项目。
1. 单击 **任务** 显示任务列表。
1. 确保 **自动保存** 切换已启用，然后选择要移动的任务。

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >当 **自动保存** 切换处于禁用状态。

1. （可选和视情况而定）如果要在同一项目中移动选定的任务，请单击选定的任务，然后将其拖动到您希望在项目中移动到的位置。

   将任务放置到项目的正确位置后，您对任务层次结构所做的更改会立即保存。 与每个任务关联的所有信息都随任务一起移动。

1. （视情况而定）选择要移动的任务或任务，然后执行以下操作之一：

   * 单击 **更多** 菜单 ![](assets/qs-more-menu.png) 在任务列表顶部，单击 **移动到**.
   * 右键单击选定的任务，然后单击 **移动到**.
   * 选择一项任务时，单击 **更多** 菜单 ![](assets/more-icon-task-list.png) 在列表中任务名称旁边，单击 **移动到**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   此时将显示“移动任务”框

1. 继续移动任务，如一节中所述 [在任务级别移动任务](#move-a-task-at-the-task-level) 在本文中，从步骤4开始。

   <!--
   is this still accurate?!
   -->

## 在任务级别移动任务 {#move-a-task-at-the-task-level}

除了从任务列表移动任务外，在打开任务后，您还可以在任务级别移动任务。 

1. 通过搜索在Workfront系统中查找任务。
1. 单击任务的名称以将其打开。
1. 单击 **更多** 下拉菜单 ![](assets/qs-more-menu.png) 在任务名称旁边，单击 **移动到**. 此时将显示“移动任务”框。

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. （可选）更新 **任务名称**. 任务将在新位置中使用新名称移动。 Workfront不记录任务的原始名称。

   >[!TIP]
   >
   >选择在列表中移动多个任务时，此字段会变暗且不可编辑。 您可以将鼠标悬停在“任务名称”字段上，并显示所有选定任务的列表。
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. 键入 **目标项目** 任务在 **选择目标项目** 字段。

   如果要在同一项目中移动任务，请键入当前项目的名称。

   >[!TIP]
   >
   >* 项目名称区分大小写。
   >* 您还可以开始键入参考编号或输入项目的ID。 这可能有助于您区分名称相同的项目。
   >* 列表中仅显示100个项目。


1. （视情况而定）单击 **请求访问** 如果您无权访问所选项目，请求获得对该项目的访问权限。
1. （视情况而定）如果您有权向目标项目上的任务之一添加任务，则继续将任务移动到选定的目标项目，而不请求访问权限。

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >如果选定的项目处于待批准、已完成或已停止状态，则当Workfront管理员阻止向这些项目添加任务时，会显示类似的消息。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. （可选）单击 **选项** 在左侧面板中

   或

   向下滚动到 **选项** ，然后取消选择下表中列出的任意项目，以将其从已移动的任务中删除。 默认情况下，将选择所有选项。

   >[!IMPORTANT]
   取消选择“选项”列表中的项目会导致数据丢失。 将删除现有任务中的信息，且无法恢复。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td>取消选中此选项可在将任务移动到新位置时从任务中删除所有信息。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">约束</td> 
      <td> <p>根据项目计划模式设置，任务约束将设置为“尽快”或“尽快”。</p> <p> 选择后，任务的当前约束将随任务一起转移。 </p> 
      <p><b>注释</b>

   在将具有特定日期限制的任务移动或复制到另一个项目，并且任务的约束日期在新项目的日期之外时，任务约束会变为“尽快”或“尽可能晚”，或调整项目的“计划起始日期”或“计划完成日期”。

   以下是特定于日期的限制示例：
   <ul>
      <li> 开始于</li>
      <li> 必须完成时间</li>
      <li> 开始时间不早于</li>
      <li> 开始时间不晚于</li>
      </ul>

   有关任务约束以及任务约束或项目日期如何受到影响的信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a> 并寻找一个特定的约束。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">分配</td> 
      <td> <p>所有分配都将从任务中删除。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">批准流程</td> 
      <td>所有审批流程都将从任务中删除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>任务状态为“新建”。 否则，将保留现有任务状态。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">财务信息</td> 
      <td>任务的财务信息将被删除，Workfront会将任务成本类型更新为“无成本”，将任务收入类型更新为“不可开单”。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>选中此选项后，当您将任务移动到其他项目时，依赖项将成为跨项目的上一个任务。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>附加到任务的文档不会转移到移动的任务。 这包括版本、校样和链接的文档。</p> <p>这不包括文档批准。 移动任务后，文档批准将永远无法移动。</p> 
      <b>注释</b>

   如果您选择不随任务移动文档，则文档将被删除并放入回收站30天。 管理员可以恢复它们，并且它们将在移动的任务中恢复。

   如果任务在移动后被删除，则还原的文档将放置在恢复任务的管理员用户页面的“文档”区域。

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任务提醒不会转移到已移动的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>已记录任务的费用不会转移到已移动的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td> <p>Workfront会删除任务“共享”列表中显示的所有实体的名称。 </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. （可选）单击 **选择父项** 在左侧面板中

   或

   滚动到 **选择父项** 部分，然后在目标项目中选择要成为已移动任务父项的任务。

   >[!TIP]
   选择在列表中移动多个任务时，所有选定任务都将成为选定父项的子项。

   通过执行以下操作之一来选择父项：

   * 在任务列表中，选择项目计划中的父项之一。
   * 单击搜索图标 ![“搜索”图标](assets/search-icon.png) 和按名称搜索父任务。

   任务应显示在列表中。

   ![使用搜索功能移动任务时选择父任务 ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父项后，为其选择单选按钮。

   如果未选择父任务，则这些任务将作为主任务而不是子任务进行移动，并且它们将放在目标项目的任务列表末尾。

1. 单击 **移动任务**

   或

   单击 **移动任务** 在列表中选择多个任务时。
移动的任务现在位于指定的项目上，并且是父任务的子任务，或是项目上的最后一个任务。
