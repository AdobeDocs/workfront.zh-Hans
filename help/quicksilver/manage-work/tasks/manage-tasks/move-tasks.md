---
product-area: projects
navigation-topic: manage-tasks
title: 移动任务
description: 您可以在Adobe Workfront中将任务移动到其他项目或不同的父级任务。
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 2%

---

# 移动任务

<!--Audited: 12/2024-->


<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


您可以在Adobe Workfront中的以下对象之间移动任务：

* 项目的临时任务。
* 从项目到另一个项目的任务。
* 另一个项目中不同父级下的项目任务。
* 同一项目内不同父级下的任务。

您可以在任务级别移动任务，也可以从任务列表中移动任务。
您可以从任务列表中移动单个任务，也可以一次移动多个任务。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的操作：

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
   <td> <p>新计划：标准 </p> 
 <p>或</p>  
<p>当前计划：工作或更高 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>具有Contribute或更高权限的项目，且能够添加任务</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 移动任务的注意事项

移动任务时，请考虑以下事项：

* 当您将任务从一个项目移动到另一个项目时，可能会重新计算任务日期。 重新计算将考虑新项目使用的时间表和项目的时间表来源信息。

* 在移动过程中，您可以选择将一些与任务相关的项目移动到移动的任务。 但是，默认情况下，以下对象会传输到移动的任务：

   * 问题
   * 记录的小时数
   * 用户评论
   * 自定义表单和自定义字段信息
   * 子任务

默认情况下，以下项目不会随任务一起移动：

* 里程碑

<div class="preview">

* 您的系统或组管理员可能会阻止您移动具有记录小时数的任务，具体取决于他们如何在“设置”区域中配置“允许用户移动具有记录小时数的任务和问题”首选项。 有关信息，请参阅[配置系统范围的任务和问题首选项](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。

</div>


## 在列表中移动任务

1. 转到包含要移动的一个或多个任务的项目。
1. 单击左侧面板中的&#x200B;**任务**&#x200B;以显示任务列表。
1. 单击&#x200B;**计划模式**&#x200B;图标![](assets/plan-mode-icon.png)并确保启用&#x200B;**自动保存**&#x200B;切换功能，然后选择要移动的一个或多个任务。

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >禁用&#x200B;**自动保存**&#x200B;切换后，您无法移动任务。

1. （可选，视情况而定）如果要在同一项目中移动选定任务，请单击选定任务，将其拖放到项目中要移动的位置。

   将任务拖放到项目的正确位置后，将立即保存对任务层次结构所做的更改。 与每个任务关联的所有信息都会随任务一起移动。

1. （视情况而定）选择要移动的一个或多个任务，然后执行以下操作之一：

   * 单击任务列表顶部的&#x200B;**更多**&#x200B;菜单![](assets/qs-more-menu.png)，然后单击&#x200B;**移至**。
   * 右键单击选定的任务，然后单击&#x200B;**移至**。
   * 选择一个任务时，单击列表中任务名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/more-icon-task-list.png)，然后单击&#x200B;**移至**。

   ![](assets/move-task-in-list-nwe-350x119.png)

   显示&#x200B;**移动任务**&#x200B;框

1. 继续移动任务，如本文中[在任务级别](#move-a-task-at-the-task-level)移动任务一节中所述，从步骤4开始。

   <!--
   is this still accurate?!
   -->

## 在任务级别移动任务 {#move-a-task-at-the-task-level}

除了从任务列表中移动任务外，在打开任务后，您还可以在任务级别移动任务。

1. 通过搜索在Workfront系统中查找任务。
1. 单击任务的名称以将其打开。
1. 单击任务名称旁边的&#x200B;**更多**&#x200B;下拉菜单![](assets/qs-more-menu.png)，然后单击&#x200B;**移至**。 此时将显示“移动任务”框。

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. （可选）更新&#x200B;**任务名称**。 该任务会以新名称移动到新位置。 Workfront不记录任务的原始名称。

   >[!TIP]
   >
   >选择在列表中移动多个任务时，“任务名称”字段会变暗且不可编辑。 您可以将鼠标悬停在“任务名称”字段上，此时将显示所有选定任务的列表。
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. 在&#x200B;**选择目标项目**&#x200B;字段中键入要将任务移动到的&#x200B;**目标项目**&#x200B;的名称。

   如果要在同一项目中移动任务，请键入当前项目的名称。

   >[!TIP]
   >
   >* 项目名称区分大小写。
   >* 您还可以开始键入参考号或输入项目的ID。 这可以帮助您区分具有相同名称的项目。
   >* 列表中仅显示100个项目。

1. （视情况而定）如果您没有所选项目的访问权限，请单击&#x200B;**请求访问权限**&#x200B;以请求对该项目的访问权限。
1. （视情况而定）如果您有权将任务添加到目标项目上的任务之一，请继续将任务移动到选定的目标项目，而不请求访问权限。

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >如果所选项目处于未决批准、已完成或终止状态，且Workfront管理员阻止将任务添加到这些项目，则会显示类似消息。 有关详细信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. （可选）单击左侧面板中的&#x200B;**选项**

   或

   向下滚动到“移动任务”框中的&#x200B;**选项**&#x200B;部分，然后取消选择下表中列出的任何项目，以将其从移动的任务中删除。 默认情况下，将选择所有选项。

   >[!IMPORTANT]
   >
   >取消选择“选项”列表中的项目会导致数据丢失。 现有任务中的信息将被删除并且无法恢复。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td>取消选择此选项可在将任务移动到其新位置时从任务中删除所有信息。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">约束</td> 
      <td> <p>任务限制被设置为“尽可能早”或“尽可能晚”，基于项目计划模式设置。</p> <p> 选中后，任务的当前限制将随任务转移。 </p> 
      <p><b>注释</b>

   当将具有日期特定限制的任务移动或复制到另一个项目，并且该任务的限制日期在新项目的日期之外时，任务限制会更改为尽可能早或尽可能晚或者调整项目的计划起始日期或计划完成日期。

   以下是特定于日期的约束示例：
   <ul>
      <li> 开始于</li>
      <li> 必须完成时间</li>
      <li> 开始时间不早于</li>
      <li> 开始时间不晚于</li>
      </ul>

   有关任务限制以及任务限制或项目日期如何受到影响的信息，请参阅<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务限制概述</a>并查找特定限制。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">任务</td> 
      <td> <p>将从任务中删除所有分配。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td>所有审批流程都将从任务中删除。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>任务状态为“新建”。 否则，将保留现有任务状态。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">财务信息</td> 
      <td>删除任务的财务信息，Workfront将任务成本类型更新为无成本，任务收入类型更新为不可记帐。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>选中后，当您将任务移动到另一个项目时，依赖关系会变为跨项目前置任务。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>附加到任务的文档不会转移到已移动的任务。 这包括版本、验证和链接文档。</p> <p>这不包括文档审批。 移动任务时绝不能移动文档审批。</p> 
      <b>注释</b>

   如果您选择不随任务移动文档，则文档将被删除并放入回收站30天。 管理员可以恢复它们，它们将在移动的任务上恢复。

   如果任务在移动后被删除，则恢复文档将放置在恢复它们的管理员用户页面的“文档”区域中。

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td>任务提醒未传输到已移动的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>任务记录的费用未转移到已移动的任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td> <p>Workfront会删除任务的“共享”列表中显示的所有实体的名称。 </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. （可选）单击左侧面板中的&#x200B;**选择父项**

   或

   滚动到&#x200B;**选择父项**&#x200B;部分，然后在目标项目中选择要成为所移动任务的父项的任务。

   >[!TIP]
   >
   >当选择在列表中移动多个任务时，所有选定任务都会成为选定父级的子级。

   通过执行以下操作之一选择父级：

   * 在任务列表中，选择项目计划中的父项之一。
   * 单击搜索图标![搜索图标](assets/search-icon.png)并按名称搜索父任务。

   任务将显示在列表中。

   ![移动具有搜索功能的任务时选择父任务](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. 找到父项后，选择该父项的单选按钮。

   如果不选择父任务，则任务将作为主任务而不是子任务移动，并放置在目标项目的任务列表的末尾。

1. 单击&#x200B;**移动任务**

   或

   在列表中选择多个任务时，单击&#x200B;**移动任务**。

   所移动的任务现在位于指定项目中，并且为父任务的子任务或项目中的最后一个任务。
