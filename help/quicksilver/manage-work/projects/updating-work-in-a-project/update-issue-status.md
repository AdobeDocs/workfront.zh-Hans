---
product-area: projects
navigation-topic: update-work-in-a-project
title: 更新问题状态
description: 您可以更新问题的状态，以告知其他人问题的位置及其进展情况。
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# 更新问题状态

您可以更新问题的状态，以告知其他人问题的位置及其进展情况。

## 访问要求

<!--drafted for P&P;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 问题状态

以下是Workfront中问题的默认状态：

* 新
* 进行中
* 等待反馈
* 保持
* 不会解决
* 重新打开
* 已关闭
* 已解决

您的Adobe Workfront管理员可以为贵组织的问题添加自定义状态。 它们还可以根据问题类型使状态可用。

有关自定义状态和问题类型的更多信息，请参阅以下文章：

* [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [创建问题](../../../manage-work/issues/manage-issues/create-issues.md)

您可以手动更新问题状态，也可以让Workfront在执行某些操作时自动更新它们。

## 手动更新问题状态

在更新问题状态时，您还可以添加有关新状态的说明，并更改其他问题信息，如提交日期。

1. 转到分配给您并要更新其状态的问题。
1. 单击 **状态** 字段，然后选择新状态。

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. 要直观地指示问题已完成，请拖动或双击下方的气泡 **完成百分比** 中。

   或

   在问题标题的气泡内单击以输入百分比。

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. （可选）执行以下任一操作以提供有关更新的其他信息，然后单击 **更新** 或者，如果问题的状态等于“完成”，请单击 **完成：**

   * 要添加有关更新的注释，请转到 **更新** 部分，单击 **开始新更新**，然后键入您的注释。

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * 要通知某些用户有关更新的信息，请在 **通知** 框。 有关更多信息，请参阅 [更新时标记其他人](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * 要更新问题的条件，请单击 **条件**，然后选择最能反映问题当前条件的条件。 从以下选项中进行选择：

      * 进展顺利
      * 一些问题
      * 主要障碍
   * 要更新问题的提交日期，请展开 **提交日期** 下拉日历，然后选择新日期。


## 自动更新问题状态

当发生下表中列出的操作时，Workfront会自动将问题的现有状态更新为其他状态。

>[!NOTE]
>
>下表中的状态是默认的系统状态。 您的Workfront管理员或组管理员可以重命名Workfront实例中的状态。 有关在Workfront中创建和管理状态的信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>操作</td> 
   <td>原始状态</td> 
   <td>新状态</td> 
  </tr> 
  <tr> 
   <td>将问题完成百分比更新为100%</td> 
   <td>新建或正在进行中</td> 
   <td>已关闭</td> 
  </tr> 
  <tr> 
   <td>将问题完成百分比从100%更新为较低的数字</td> 
   <td>已关闭 </td> 
   <td>进行中</td> 
  </tr> 
  <tr> 
   <td>更新附加到问题的解析对象的状态</td> 
   <td>各种状态</td> 
   <td> <p>各种状态</p> <p>有关解析对象以及这些对象如何影响问题状态的信息，请参阅文章中的“将可解析对象的状态与解析对象的状态同步”一节 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>单击开始问题按钮以接受处理分配给您的问题</span> </td> 
   <td><span>新</span> </td> 
   <td> <p>与“主团队”设置中的“开始问题”按钮关联的任何状态。 </p> <p>有关将“Work On It（处理）”按钮替换为“Start Issue（开始问题）”按钮的信息，请参阅 <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“Work On It（处理它）”按钮替换为“Start（开始）”按钮</a></span><span>.</span> </p> <p>提示：单击 <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">“撤消”按钮</span> 单击“开始问题”后，状态将还原为“新建”。 </p> </td> 
  </tr> 
 </tbody> 
</table>
