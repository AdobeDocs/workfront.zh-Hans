---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新问题状态
description: 您可以更新问题的状态，以通知其他人该问题的位置及其进展情况。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 2%

---

# 更新问题状态

<!--Audited: 01/2024-->

您可以更新问题的状态，以通知其他人该问题的位置及其进展情况。

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
   <td> <p>新许可证：参与者或更高版本</p>
   或
   <p>当前许可证：请求或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 问题状态

以下是Workfront中问题的默认状态：

* 新
* 进行中
* 等待反馈
* 暂停
* 不会解决
* 重新打开
* 已关闭
* 已解决

Adobe Workfront管理员可以为您的组织添加问题的自定义状态。 他们还可以使状态变得可用，具体取决于问题类型。

有关自定义状态和问题类型的更多信息，请参阅以下文章：

* [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [创建问题](../../../manage-work/issues/manage-issues/create-issues.md)

您可以手动更新问题状态，也可以让Workfront在某些操作发生时自动更新问题。

## 手动更新问题状态

您可以在Workfront的以下区域中更新问题状态：

* 任务页面上的问题标题。
* 编辑问题框（编辑问题时）。
* 问题页面上的详细信息部分。
* 在问题列表或报告中，当“状态”字段在视图中可见时。
* 在问题的“摘要”面板中。

要在问题标题中手动更新问题状态，请执行以下操作：

1. 转到要更新其状态的问题。
1. 单击 **状态** 字段，然后选择新状态。
1. 要提供问题完成的可视指示，请拖动或双击下的气泡 **完成百分比** （在问题的标题中）

   或

   在问题标题中的气泡内单击以输入百分比。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （可选）执行以下任一操作以提供有关更新的其他信息：

   * 要添加有关更新的注释，请转到 **更新** 部分并单击 **新建评论**，然后键入注释。

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 要通知特定用户有关更新，请在 **标记人员或团队** 键入评论时显示的字段。 有关更多信息，请参阅 [为其他人标记更新](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 要更新问题的提交日期，请单击 **问题详细信息**，然后编辑 **提交日期** 字段。 有关信息，请参阅 [编辑问题](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  只有问题被分配者才能更新提交日期。



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## 自动更新问题状态

当下表列出的操作发生时，Workfront会自动将问题的现有状态更新为其他状态。

>[!NOTE]
>
>下表中的状态是默认的系统状态。 您的Workfront管理员或组管理员可以重命名Workfront实例中的状态。 有关在Workfront中创建和管理状态的信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>操作</b></td> 
   <td><b>原始状态</b></td> 
   <td><b>新建状态</b></td> 
  </tr> 
  <tr> 
   <td>将问题完成百分比更新为100%</td> 
   <td>新建或进行中</td> 
   <td>已关闭</td> 
  </tr> 
  <tr> 
   <td>将问题完成百分比从100%更新为较低数字</td> 
   <td>已关闭 </td> 
   <td>进行中</td> 
  </tr> 
  <tr> 
   <td>更新附加到问题的解析对象的状态</td> 
   <td>各种状态</td> 
   <td> <p>各种状态</p> <p>有关解析对象以及它们如何影响问题状态的信息，请参阅文章中的“将可解析对象的状态与解析对象的状态同步”部分 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>单击“开始问题”按钮接受处理分配给您的问题</span> </td> 
   <td><span>新建</span> </td> 
   <td> <p>与主团队设置中的开始问题按钮关联的任何状态。 </p> <p>有关将“处理此项工作”按钮替换为“开始问题”按钮的信息，请参阅 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“处理此项工作”按钮替换为“开始”按钮</a></span><span>.</span> </p> <p>提示：单击 <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">“撤消”按钮</span> 单击“开始问题”后，状态将恢复为“新建”。 </p> </td> 
  </tr> 
 </tbody> 
</table>
