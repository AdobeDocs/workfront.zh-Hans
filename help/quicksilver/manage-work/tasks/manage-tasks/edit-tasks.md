---
product-area: projects
navigation-topic: manage-tasks
title: 编辑任务
description: 您可以编辑有关已创建、拥有Contribute或“管理”权限的任务的信息。 本文介绍了如何搜索、查找和编辑任务（如果您有相应的权限）。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '3681'
ht-degree: 3%

---

# 编辑任务

<!--Audited: 07/2024-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a field, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


您可以编辑有关已创建、拥有Contribute或“管理”权限的任务的信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新增：标准</p>
   <p>当前：工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>编辑对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <ul> 
     <li> <p>Contribute对任务的权限，以便在任务详细信息区域编辑以下信息： </p>
     <ul>
     <li>描述</li>
     <li>状态</li>
     </ul>  
      </li> 
     <li> <p>管理任务的权限以编辑详细信息区域和编辑任务框中的所有信息</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Contribute或项目的更高权限</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 编辑任务的限制

有一些限制可能会阻止您编辑任务。

编辑任务时，请考虑以下事项：

* 更新任务会触发处于当前状态的项目的通知。 为避免分配给任务的用户混淆，当项目处于当前状态时，应尽可能限制编辑任务。
* 您无法编辑批准流程中的任务。 您只能为批准流程中的任务记录时间或更新状态。

  ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* 只有当Workfront管理员或组管理员在项目偏好设置区域中启用此功能时，您才能编辑文档并将其添加到状态为“完成”、“废弃”或“未决批准”的项目中的任务。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 当项目被标记为“完成”、“终止”或处于批准流程中时，您始终可以编辑任务的以下信息：

   * 记录时间
   * 编辑现有费用
   * 附加自定义表单

* 其他用户必须先刷新其页面，然后才能查看您对任务所做的更新。

## 编辑列表中的任务

通过内联编辑列表视图中显示的字段，可以编辑任务列表中的任务信息。

有关编辑列表中的任务的信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)。

## 使用摘要编辑列表中的任务

您可以使用“摘要”面板编辑列表中的任务。 有关在“摘要”面板中编辑任务的信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)文章中的“编辑摘要中的任务”部分。

## 在“编辑任务”框中编辑任务

您可以使用“编辑任务”或“任务详细信息”区域编辑任务。 以下步骤描述了如何在“编辑任务”框中编辑任务。

{{step1-click-main-menu}}

1. 单击&#x200B;**项目**，然后单击项目名称以将其打开。
1. 单击左侧面板中的&#x200B;**任务**。
1. 单击要编辑的任务。
1. （视情况而定）要编辑有关任务的有限信息，请单击左侧面板中的&#x200B;**任务详细信息**。

   ![](assets/nwe-task-details-expanded-350x273.png)

   请考虑编辑“任务详细信息”部分中以下区域的信息：

   * **概述**

     默认情况下，此区域处于扩展状态。

   * **自定义表单**

     只有当对象附加了自定义表单时，才会显示自定义表单的名称。

   * **财务**

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，任务详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   有关“任务详细信息”部分中可见的字段的信息，请继续编辑“编辑任务”框中的任务，如下所述。

   要编辑“详细信息”部分中的信息，请执行以下操作：

   1. （可选）单击右上角的&#x200B;**全部折叠**&#x200B;图标![](assets/collapse-all-icon.png)以折叠所有区域。
   1. （可选且有条件）折叠区域时，单击每个区域旁边的&#x200B;**向右箭头** ![](assets/right-pointing-arrow.png)以展开要编辑的区域。
   1. 有关在“任务详细信息”选项卡中编辑信息的详细信息，请参阅以下文章：

      * [在任务详细信息概述区域管理任务信息](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [在“任务详细信息”部分管理任务财务](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

   1. （可选）如果没有自定义表单附加到任务，请在&#x200B;**添加自定义表单**&#x200B;字段中开始键入表单的名称，然后在表单显示在列表中时将其选定，然后单击&#x200B;**保存更改**。
   1. （可选）单击&#x200B;**导出**&#x200B;图标![](assets/export.png)以将概述和自定义表单信息导出到PDF文件，然后单击&#x200B;**导出**。 从以下项中选择：

      * 选择全部（仅在至少附加一个自定义表单时显示）
      * 概述
      * 一个或多个自定义表单的名称

      PDF文件将下载到您的计算机。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      有关详细信息，请参阅[导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)。

1. （视情况而定）要编辑有关任务的所有信息，请以具有任务管理权限的用户身份，单击任务名称旁边的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑**。

   或

   从任务列表中选择任务，然后单击列表顶部的&#x200B;**编辑**&#x200B;图标![](assets/edit-icon.png)。

   将打开“编辑任务”框。

   >[!IMPORTANT]
   >
   >您必须具有任务的“管理”权限才能看到“编辑”选项。

   所有任务字段在“编辑任务”框中均可用，并按左侧面板中列出的区域分组。

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，任务详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   请考虑在以下任意部分中指定信息：

   * [任务名称](#task-name)
   * [概述](#overview)
   * [分配](#assignments)
   * [自定义表单](#Custom%C2%A0F)
   * [财务](#finance)
   * [设置](#settings)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员设置布局模板的方式，编辑任务框中的字段可能会重新排列或不显示。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

### 任务名称 {#task-name}

1. 按如上所述开始编辑任务。
1. 单击左侧面板中的&#x200B;**任务名称**。

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. 更新任务的名称。

1. 单击&#x200B;**保存**&#x200B;或继续以下部分。

### 概述 {#overview}

1. 按如上所述开始编辑任务。
1. 单击左侧面板中的&#x200B;**概述**。

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. 更新关于任务的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>添加有关任务的其他信息。 </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">基本信息部分</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>选择任务的状态，以指示任务处于哪个开发阶段。</p> <p><b>提示</b>

   您可以在任务标题中更新任务状态。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">优先级</td> 
      <td> <p>这是一个可视标志，可用于安排任务的优先级。 </p> <p>从以下选项中选择： </p> 
       <ul> 
      <li> <p> 无</p> </li> 
      <li> <p> 低 </p> </li> 
      <li> <p>正常 </p> </li> 
      <li> <p>高 </p> </li> 
      <li> <p> 紧急 </p> </li> 
       </ul> <p>根据您的Workfront管理员选择的项目偏好设置，优先级名称可能有所不同。 有关任务优先级的信息，请参阅<a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">更新任务优先级</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">任务日期和约束部分</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任务限制</td> 
      <td> <p>通过指定任务限制来确定何时必须完成任务。 </p> <p>从以下选项中选择： </p> 
       <ul> 
      <li> <p><span>固定日期</span> </p> <p>指定<strong>计划开始</strong>和<strong>计划完成日期</strong>。 </p> </li> 
      <li> <p><span>必须在</span>开始 </p> <p>指定<strong>计划开始日期</strong>。 </p> </li> 
      <li> <p><span>必须在</span>完成 </p> <p>指定<strong>计划完成日期</strong>。 </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>尽快</span></p> </li> 
      <li> <p><span>尽可能迟</span></p> </li> 
      <li> <p><span>最早可用时间</span></p> </li> 
      <li> <p> <span>最新可用时间</span></p> </li> 
      <li> <p><span>开始时间不晚于</span> </p> </li> 
      <li> <p>指定计划的开始日期</p> </li> 
      <li> <p><span>开始时间不早于</span> </p> <p>指定<strong>计划开始日期</strong>。 </p> </li> 
      <li> <p> 完成<span>的时间不晚于</span></p> <p>指定<strong>计划完成日期</strong>。 </p> </li> 
      <li> <p> 完成<span>的时间不早于</span></p> <p>指定<strong>计划完成日期</strong></p> </li> 
       </ul> <p>有关任务限制的详细信息，请参阅<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务限制概述</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提交日期和时间</td> 
      <td> <p>这是分配给任务的用户承诺完成任务的日期。 这可能与计划的完成日期不同。 只有被分配者才能编辑此字段。 有关Workfront中提交日期的信息，请参阅<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划开始日期和时间</td> 
      <td> <p>任务计划开始的时间。 任务的计划开始日期受许多因素的影响和影响：</p> 
       <ul> 
      <li>根据系统范围对任务计划开始日期的偏好设置，项目上新任务的开始日期可以是今天，也可以是项目的开始日期（默认情况下）。 <span>与项目关联的组的组管理员也可以为该组设置此首选项。</span>有关系统级别或组级别任务首选项的详细信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">配置系统范围的任务和问题首选项</a>。</li> 
      <li>根据任务的前置任务，Workfront会将计划开始日期选为前置任务完成后下一个可用日期，或选择开始日期，具体取决于前置任务关系。 有关前置任务关系的详细信息，请参阅<a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">前置任务概述</a>。</li> 
      <li>当任务限制为固定日期或必须开始日期时，项目经理或任务所有者可以手动设置计划开始日期。 有关任务限制的更多信息，请参阅<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务限制概述</a>。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期和时间</td> 
      <td> <p>计划的任务时显示的预计完成日期。 Workfront使用下列因素设置计划完成日期：</p> 
       <ul> 
      <li>从计划开始日期通过将任务的持续时间添加到计划开始日期来计算计划完成日期。 当项目经理或Workfront指定任务的持续时间时，将触发对计划完成日期的更新。 如果计划日期发生更改，通常是因为任务的持续时间已更新。</li> 
      <li>当任务限制为“固定日期”或“必须完成日期”时，项目经理或任务所有者可以手动设置计划完成日期。 有关任务限制的更多信息，请参阅<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务限制概述</a>。</li> 
      <li>如果任务的持续时间类型发生更改，并且任务上的资源数量同时发生更改，则计划完成日期也会发生更改。 有关持续时间类型的详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型的概述</a>。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际开始日期和时间</td> 
      <td> <p>指定任务的实际开始日期。 当您将任务的状态更改为进行中时，通常会自动填充默认值。 项目经理或任务所有者也可以手动修改实际开始日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际完成日期和时间</td> 
      <td> <p>指定任务完成的实际日期和时间。 任务完成时的默认日期和时间始终与状态变为“已完成”时的实际时间一致。 项目经理或任务所有者也可以手动修改实际完成日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>工作时间部分</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作投入 </td> 
      <td>

   <p>完成任务所需的工作量。 您的项目经理可能会决定使用此字段而不是计划小时数来估计完成任务所需的工作量。 仅当满足以下条件时，此字段才可见：</p> 
      <ul> 
      <li> <p>任务的持续时间类型很简单。 </p> <p><b>提示</b>

   如果更改任务的持续时间类型，此字段将变暗。 </p> </li>
   <li>您的项目经理已启用使用工作投入以自动计算项目上的任务已计划小时数字段。 </li> 
      </ul> 
      <p>从以下选项中选择：</p> 
      <ul> 
      <li>小</li> 
      <li>Medium <span style="font-weight: normal;">（这是新任务的默认值）</span></li> 
      <li>大</li> 
      </ul> 
      <p><b>注释</b>

   更新工作量可能会更新任务计划小时数。 如果项目更新类型为“自动”，则立即进行更新。 当项目更新类型为手动时，必须重新计算时间线以查看更新的计划小时数。 </p>

   <p>有关使用工作投入而不是计划小时数来估计任务投入的信息，请参阅<a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>。 </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**&#x200B;或继续以下部分。

### 分配 {#assignments}

1. 按如上所述开始编辑任务。
1. 单击左侧面板中的&#x200B;**工作**。

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. 单击&#x200B;**搜索人员、角色和团队**，然后开始键入要分配给任务的用户、角色或团队的名称，然后单击该名称，或当该名称显示在列表中时按Enter键。

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则它们仍会分配给工作项。 在这种情况下，我们建议执行以下操作：
   >
   >* 将工作项重新分配给活动资源。
   >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

1. （可选）通过选择任务负责人名称旁边的&#x200B;**所有者**&#x200B;单选按钮，指明任务负责人是否为任务的主要任务负责人。 团队不能是任务的主要被分配人。
1. （有条件和可选）更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">持续时间类型</td> 
      <td> <p>这确定了以下各项之间的关系： </p> 
       <ul> 
      <li> <p>分配给任务的资源数 </p> </li> 
      <li> <p>完成任务所需的总工作量 </p> </li> 
      <li> <p> 任务的总持续时间。 </p> </li> 
       </ul> <p>您的Workfront管理员或组管理员为您的系统或组中的任务选择默认持续时间类型设置。 有关设置项目默认设置的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。 </p> <p>持续时间类型使您能够根据任务的需要设置一致的资源分配。 有关任务的持续时间类型的详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概览</a>。 </p> <p>从以下选项中选择： </p> 
       <ul> 
      <li> <p>计算的分配量 </p> </li> 
      <li> <p> 计算的工作量 </p> </li> 
      <li> <p>投入比导向 </p> </li> 
      <li> <p>简单</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">每次发生的持续时间</td> 
      <td> <p>这仅在周期性任务的父级上显示。 它显示每个周期性任务的持续时间，如创建任务时定义。 有关创建周期性任务的信息，请参阅<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建周期性任务</a>。 </p> <p> <b>注释</b>

   在单个周期性任务中修改的持续时间不显示此字段中指示的值。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td> 
      <div> 
      <div> 
      <p>这是在任务完成之前您允许任务保持打开状态的时长。 </p> 
      <p><b>重要</b>

   由于任务持续时间通常是计划开始日期和计划完成日期之间的时间量，因此它会影响项目的时间表。</p>

   <p>要指明任务的持续时间和时间单位，请执行以下操作：</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">键入时间长度，并从下拉菜单中的可用时间单位中选择。</p> <p><b>提示</b></p>
      更新任务列表中的任务持续时间时，可以使用时间单位的缩写。 </p> </li> 
      </ul> 
      <p> 您可以从下表中的常规时间或占用时间选项中进行选择： </p> 
      <table style="table-layout:auto"> 
      <col> 
      <col data-mc-conditions=""> 
      <tbody> 
      <tr> 
      <td>时间单位</td> 
      <td>缩写</td> 
      </tr> 
      <tr> 
      <td>分钟</td> 
      <td>一</td> 
      </tr> 
      <tr> 
      <td>小时</td> 
      <td>H</td> 
      </tr> 
      <tr> 
      <td>天。 这是默认设置。 </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>周</td> 
      <td>星期-</td> 
      </tr> 
      <tr> 
      <td>月</td> 
      <td>T</td> 
      </tr> 
      <tr> 
      <td>经过的分钟数</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>经过的小时数</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>经过的天数</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>经过的周数</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>经过的月数</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>注释</b>

   <p>占用时间是任务持续时间的时间单位。 该时间是任务的计划开始日期与计划完成日期之间的时间，包括假日、周末和休息时间。 换言之，经过的时间就是行事历的日数。

   常规时间会考虑假日、周末和休息时间，并将它们排除在任务的持续时间之外。 有关任务持续时间的详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>。 </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">规划小时数</td> 
   <td> <p>指定任务的计划小时数（以小时为单位）。 这是任务被分派人完成任务所花费的实际时间。 当“持续时间类型”设置为“计算的工作分配”时，您只能指定任务的已计划小时数。 有关持续时间类型的详细信息，请参阅<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型的概述</a>。</p> 
   <b>注释</b>
   <p>
   创建周期性任务时，计划小时数是每个事件的小时数。 父任务的计划小时数是所有发生的所有计划小时数的总和。 有关创建周期性任务的信息，请参阅<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建周期性任务</a>。
   </p>

   </td> 
   </tr> 
   <tr> 
   <td role="rowheader">分配</td> 
   <td> <p>如果您的任务限制是计算的工作或投入比导向，请为每个被分派人指定<strong>分配%</strong>（分配百分比）。 这是指从被分派人计划起他们可在此任务上花费的时间。 更改被分配人的分配百分比将更改任务的已计划小时数。 </p> <p>当“任务约束”为“简单”时，可以指定以下内容：</p> 
      <ul> 
      <li> <p>每个被分配人的分配小时数。</p> </li> 
      <li> <p>任务的已计划小时数</p> </li> 
      <li> <p>任务持续时间</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">受让人的角色</td> 
   <td> <p>选择人员作为被分派人时，请从<strong>被分派人的角色</strong>下拉菜单中选择一个角色。 这是被分派人可以在这项任务上履行的职责。 </p> <p><b>提示</b>

   下拉菜单中仅显示与其配置文件中每个被分配人关联的工作角色。</p> </td>
   </tr> 
      </tbody> 
      </table>

1. 单击&#x200B;**保存**&#x200B;或继续以下部分。

### 自定义表单

可定义在将任务添加到项目时自动附加到任务的默认自定义表单。 有关设置项目以包含所有新任务的默认任务自定义表单的信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)一文中的“任务”一节。

1. 按如上所述开始编辑任务。
1. 单击左侧面板中的&#x200B;**自定义Forms**，或者单击已附加的自定义表单的名称。

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 单击&#x200B;**添加自定义表单**，然后选择要与任务关联的一个或多个自定义表单。 您必须先构建自定义表单，然后才可在此字段中选择它们。 列表中仅显示活动的自定义表单。

   有关生成自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。您最多可以向一个任务添加十个自定义表单

1. （视情况而定）如果您将自定义表单附加到任务，请编辑表单上的任何字段。 在保存任务之前，必须指定所有必填字段。

   >[!NOTE]
   >
   >根据Workfront管理员为自定义表单中的分区设置权限的方式，并非每个人都可以查看或编辑给定自定义表单上的相同字段。 在自定义表单的部分中编辑字段的权限取决于您对任务本身的权限。 有关设置任务权限的信息，请参阅[共享任务](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)。

1. 单击&#x200B;**保存**&#x200B;或继续以下部分。

### 财务 {#finance}

1. 开始编辑您的任务，如本文的[编辑任务](#Edit2)部分所述。
1. 单击左侧面板中的&#x200B;**财务**。

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>指定任务的成本类型。 这将根据任务的小时数确定如何计算任务成本。 </p> <p>从以下选项中选择： </p> 
       <ul> 
        <li> <p>无成本</p> </li> 
        <li> <p>固定每小时 </p> </li> 
        <li> <p> 用户每小时 </p> </li> 
        <li> <p> 角色每小时</p> </li> 
       </ul> <p>有关跟踪成本的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a> 。 您的Workfront管理员或组管理员为您的系统或组中的任务选择默认成本类型设置。 有关设置项目默认设置的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a> 。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>指定任务的收入类型。 这将根据任务的小时数确定如何计算任务收入。 </p> <p>从以下选项中选择： </p> 
       <ul> 
      <li> <p> 不可计费 </p> </li> 
      <li> <p>用户每小时 </p> </li> 
      <li> <p>角色每小时 </p> </li> 
      <li> <p>固定每小时 </p> </li> 
      <li> <p>受限用户小时 </p> </li> 
      <li> <p>受限角色小时 </p> </li> 
      <li> <p>用户小时加固定 </p> </li> 
      <li> <p>角色小时加固定 </p> </li> 
      <li> <p>固定收入 </p> </li> 
       </ul> <p>有关跟踪收入的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a> 。 </p> <p>您的Workfront管理员或组管理员为您的系统或组中的任务选择默认收入类型设置。 有关设置项目默认设置的信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**&#x200B;或继续下面的部分。

### 设置 {#settings}

1. 开始编辑您的任务，如本文的[编辑任务](#Edit2)部分所述。
1. 单击左侧面板中的&#x200B;**设置**。

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. 更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">跟踪模式</td> 
      <td> <p>指定如何跟踪任务的进度状态。 </p> <p>从以下选项中选择： </p> 
       <ul> 
      <li> <p> 用户必须更新 </p> </li> 
      <li> <p>假设准时 </p> </li> 
      <li> <p>忽略迟到警告</p> </li> 
      <li> <p> 自动完成 </p> </li> 
      <li> <p>前置任务 </p> </li> 
       </ul> <p>有关任务跟踪模式的详细信息，请参阅<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任务跟踪模式概述</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源均衡</td> 
      <td> <p>如果希望从资源均衡中排除分配给任务的资源，请选择<strong>从资源均衡中排除</strong>字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">均衡延迟</td> 
      <td> <p>以小时为单位指定均衡延迟。 </p> <p> 有关调配延迟的详细信息，请参阅<a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">更新任务调配延迟</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td> <p>选择要与任务关联的审批流程。 您的Workfront管理员必须定义系统级别的批准流程，然后才能将其与任务关联。 对审批流程具有管理权限的用户也可以创建特定于组的审批流程。 </p> <p>有关创建审批流程的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">为工作项创建审批流程</a>。 添加审批流程时，请考虑以下事项： </p> 
       <ul>

   <li> <p>列表中仅显示有效的审批流程。 </p> </li>

   <li> <p>系统范围及组特定的批准流程会显示在列表中。 与项目组以外的组关联的审批流程不会显示在列表中。 </p>

   <p><b>重要</b>

   如果项目组发生更改，则以前附加的组特定审批流程会变成一次性审批流程。 有关对项目组的更改或审批流程中的更改如何影响审批设置的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">组和审批流程更改如何影响分配的审批流程</a>。 </p>

   </li>

   <li> <p>您可以定义在任务添加到项目时自动附加到任务的默认审批流程。 有关设置项目以包含默认任务审批流程的信息，请参阅<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">编辑项目</a>一文中的“任务”一节。 </p> </li>

   <li> <p>批量编辑任务时，存在以下情况： </p> 
      <ul> 
      <li> <p>从同一组中选择多个任务时，系统级别和组级别审批流程都会显示在此字段中。 </p> </li> 
      <li> <p>从不同的组中选择多个任务时，此字段仅显示系统级别的审批流程。 </p> </li> 
      <li> <p>当任何任务附加一次性审批流程时，它将被您选择的系统级别或组级别审批流程替换。 </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. 单击&#x200B;**保存**。

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## 在任务标题中编辑任务（受限）

您可以在任务标题中编辑有限数量的信息。

您的系统或组管理员可以自定义您在任务标题中看到的字段。 有关详细信息，请参阅[使用布局模板自定义对象标头](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

默认情况下，任务标题中包含以下字段：

* 任务名称
* 完成百分比
* 分配
* 规划完成日期

  >[!CAUTION]
  >
  >某些任务约束和其他依赖关系可能会阻止您编辑此字段。 有关任务限制的信息，请参阅[任务限制概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)。

* 状态
* 如果在当前审批流程中将您设置为审批者，则做出审批决策

## 批量编辑任务

您可以选择自动保存对列表中的任务所做的更改时，在列表中批量编辑任务并同时更新其所有信息。

有关批量保存任务的信息，请参阅文章[在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)中的“批量编辑任务”部分。
