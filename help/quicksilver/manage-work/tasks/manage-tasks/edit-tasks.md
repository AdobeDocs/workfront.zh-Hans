---
product-area: projects
navigation-topic: manage-tasks
title: 编辑任务
description: 编辑任务
author: Alina
feature: Work Management
exl-id: 572c6008-3a67-47ae-8f5d-6b871ef1f37b
source-git-commit: 9c7af82b02649f33728d05126587fb5035e9e110
workflow-type: tm+mt
source-wordcount: '3627'
ht-degree: 4%

---

# 编辑任务

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: some information in this area is repeated in the following articles. If you need to update a fied, update it in both:</p>
<p>** Task finances in details</p>
<p>** Task information in overview)</p>
</div>
-->


您可以编辑有关已创建、或您具有“Contribute”或“管理”权限的任务的信息。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <ul> 
     <li> <p>向任务贡献权限以在“任务详细信息”区域中编辑该任务 </p> </li> 
     <li> <p>在“编辑任务”框中管理任务的权限以对其进行编辑</p> </li> 
    </ul> 
    <ul> 
     <li> <p>对项目拥有或更高权限</p> </li> 
    </ul> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑任务的限制

有些限制可能会阻止您编辑任务。

编辑任务时请考虑以下事项：

* 更新任务会触发“当前”状态项目的通知。 为避免为分配了任务的用户造成混淆，在项目处于“当前”状态时，请尽可能限制编辑任务。
* 您无法编辑审批流程中的任务。 您只能记录批准流程中某项任务的“状态”时间或更新“状态”。

   ![](assets/edit-task-in-approval-process-nwe-350x148.png)

* 仅当您的Workfront管理员或组管理员在“项目首选项”区域中启用此功能时，您才能编辑文档并将其添加到项目中状态为“完成”、“无效”或“待批准”的任务。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 当项目被标记为“完成”、“已停用”或处于“审批流程”中时，您始终可以编辑任务的以下信息：

   * 日志时间
   * 编辑现有费用
   * 附加自定义表单

## 编辑列表中的任务

您可以通过列表视图中显示的内嵌编辑字段，编辑任务列表中的任务信息。

有关在列表中编辑任务的信息，请参阅 [在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

## 使用“摘要”编辑列表中的任务

您可以使用“摘要”面板编辑列表中的任务。 有关在“摘要”面板中编辑任务的信息，请参阅 [在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md) 文章。

## 在“编辑任务”框中编辑任务

您可以使用“编辑任务”或“任务详细信息”区域编辑任务。 以下步骤介绍了如何在“编辑任务”框中编辑任务。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **项目**，然后单击项目名称以将其打开。
1. 单击 **任务** 中。
1. 单击要编辑的任务。
1. （可选）要编辑有关任务的有限信息，请单击 **任务详细信息** 中。

   ![](assets/nwe-task-details-expanded-350x273.png)

   请考虑在“任务详细信息”部分的以下区域编辑信息：

   * **概述**

      默认情况下，此区域会展开。

   * **自定义表单**

      只有在对象附有自定义表单时，海关表单的名称才会显示。

   * **财务**
   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，任务详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   有关“任务详细信息”部分中显示的字段的信息，

   继续编辑“编辑任务”框中的任务，如下所述。

   要编辑详细信息部分中的信息，请执行以下操作：

   1. （可选）单击 **全部折叠** 图标 ![](assets/collapse-all-icon.png) 来折叠所有区域。
   1. （可选和视情况而定）折叠区域后，单击 **向右箭头** ![](assets/right-pointing-arrow.png) 展开要编辑的区域。
   1. 有关编辑“任务详细信息”选项卡中信息的详细信息，请参阅以下文章：

      * [在“任务详细信息概览”区域中管理任务信息](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)
      * [在“任务详细信息”部分中管理任务财务](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
   1. （可选）如果任务中没有附加自定义表单，请在 **添加自定义表单** 字段，然后在列表中显示时将其选中，然后单击 **保存更改**.
   1. （可选）单击 **导出** 图标 ![](assets/export.png) 要将概述和自定义表单信息导出到PDF文件，请单击 **导出**. 从以下选项中进行选择：

      * 全选（仅当至少附加了一个自定义表单时才显示）
      * 概述
      * 一个或多个自定义表单的名称

      PDF文件将下载到您的计算机。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      有关更多信息，请参阅 [导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).




1. 要编辑有关任务的所有信息，请单击 **更多** 菜单 ![](assets/more-icon.png) 在任务名称旁边，单击 **编辑**.

   或

   从任务列表中，选择一个任务，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 列表顶部。

   “编辑任务”(Edit Task)框打开。

   >[!IMPORTANT]
   >
   >您必须具有任务的“管理”权限，才能看到“编辑”选项。

   “编辑任务”框中提供了所有任务字段，并按左侧面板中列出的区域进行分组。

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，任务详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   请考虑在以下任一部分中指定信息：

   * [任务名称](#task-name)
   * [概述](#overview)
   * [分配](#assignments)
   * [自定义表单](#Custom%C2%A0F)
   * [财务](#finance)
   * [设置](#settings)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员设置布局模板的方式，“编辑任务”框中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 任务名称 {#task-name}

1. 开始按如上所述编辑任务。
1. 单击 **任务名称** 中。

   ![](assets/nwe-task-name-section-edit-task-box-350x122.png)

1. 更新任务的名称。

1. 单击 **保存** 或继续以下部分。

### 概述 {#overview}

1. 开始按如上所述编辑任务。
1. 单击 **概述** 中。

   ![](assets/nwe-overview-section-edit-task-box-350x257.png)

1. 更新有关任务的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>添加有关该任务的其他信息。 </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">基本信息部分</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>选择任务的状态，以指示任务处于开发的哪个阶段。</p> <p><b>笔尖</b>

   您可以更新任务标题中的任务状态。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">优先级</td> 
      <td> <p>这是一个可视标记，用于确定任务的优先级。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
      <li> <p> 无</p> </li> 
      <li> <p> 低 </p> </li> 
      <li> <p>正常 </p> </li> 
      <li> <p>高 </p> </li> 
      <li> <p> 紧急 </p> </li> 
       </ul> <p>根据Workfront管理员选择的项目首选项，优先级名称可能会因您而异。 有关任务优先级的信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-priority.md" class="MCXref xref">更新任务优先级</a>. </p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"><span style="font-weight: bold;">任务日期和约束部分</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任务限制</td> 
      <td> <p>通过指定任务约束确定任务何时必须完成。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
      <li> <p><span>固定日期</span> </p> <p>指定 <strong>计划开始</strong> 和 <strong>计划完成日期</strong>. </p> </li> 
      <li> <p><span>必须开始时间</span> </p> <p>指定 <strong>计划开始日期</strong>. </p> </li> 
      <li> <p><span>必须完成时间</span> </p> <p>指定 <strong>计划完成日期</strong>. </p> </li> 
       </ul> 
       <ul> 
      <li> <p><span>尽快</span></p> </li> 
      <li> <p><span>尽可能晚</span></p> </li> 
      <li> <p><span>最早可用时间</span></p> </li> 
      <li> <p> <span>最晚可用时间</span></p> </li> 
      <li> <p><span>开始时间不晚于</span> </p> </li> 
      <li> <p>指定计划的开始日期</p> </li> 
      <li> <p><span>开始时间不早于</span> </p> <p>指定 <strong>计划开始日期</strong>. </p> </li> 
      <li> <p> 完成 <span>不迟于</span></p> <p>指定 <strong>计划完成日期</strong>. </p> </li> 
      <li> <p> 完成 <span>不早于</span></p> <p>指定 <strong>计划完成日期</strong></p> </li> 
       </ul> <p>有关任务约束的详细信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提交日期和时间</td> 
      <td> <p>这是分配给任务的用户提交完成任务的日期。 这可能与计划完成日期不同。 只有被分配者才能编辑此字段。有关Workfront中提交日期的信息，请参阅 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划开始日期和时间</td> 
      <td> <p>计划开始任务时。 任务的计划起始日期会设置并受多种因素的影响：</p> 
       <ul> 
      <li>根据任务计划起始日期的全系统首选项，项目上新任务的开始日期可以是今天，也可以是项目的开始日期（默认情况下）。 <span>与项目关联的组的组管理员也可以为组设置此首选项。</span> 有关系统级别或组级别任务首选项的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">配置系统范围的任务和问题首选项</a>.</li> 
      <li>根据任务的前置任务，Workfront会选择计划的开始日期作为前置任务完成后的下一个可用日期，或根据前置任务关系开始。 有关前身关系的更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任务前置任务概述</a>.</li> 
      <li>当任务约束为“固定日期”或“必须开始”时，项目经理或任务责任人可以人工设置计划的起始日期。 有关任务约束的详细信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期和时间</td> 
      <td> <p>计划任务时显示的预期完成日期。 计划完成日期可通过多种因素进行设置：</p> 
       <ul> 
      <li>通过将任务的持续时间添加到计划起始日期，从计划起始日期计算计划完成日期。 当项目经理或Workfront指定任务的持续时间时，这会触发对计划完成日期的更新。 如果计划日期发生更改，则通常是因为的持续时间已更新。</li> 
      <li>当任务约束为“固定日期”或“必须完成”时，项目经理或任务责任人可以人工设置计划完成日期。 有关任务约束的详细信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>.</li> 
      <li>如果任务的持续时间类型发生更改，并且任务上的资源数量同时发生更改，则计划完成日期也将发生更改。 有关持续时间类型的更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际开始日期和时间</td> 
      <td> <p>指定任务的实际开始日期。 当将任务的状态更改为“进行中”时，通常会自动填充默认值。 项目经理或任务责任人也可以手动修改实际起始日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际完成日期和时间</td> 
      <td> <p>指定任务完成的实际日期和时间。 任务完成的默认日期和时间始终与状态变为“完成”时的实际时间一致。 项目经理或任务责任人也可以手动修改实际完成日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><b>工作时间部分</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">工作投入 </td> 
      <td>

   <p>完成任务所需的工作量。 您的项目经理可能会决定使用此字段而不是“计划小时数”来估算完成任务所需的工作量。 仅当满足以下条件时，此字段才可见：</p> 
      <ul> 
      <li> <p>任务具有简单持续时间类型。 </p> <p><b>笔尖</b>

   如果更改任务“持续时间类型”，此字段将变灰。 </p> </li>
   <li>您的项目经理已启用使用工作量以自动计算项目上的任务计划小时数字段。 </li> 
      </ul> 
      <p>从以下选项中进行选择：</p> 
      <ul> 
      <li>小</li> 
      <li>中 <span style="font-weight: normal;">（这是新任务的默认值）</span></li> 
      <li>大</li> 
      </ul> 
      <p><b>注释</b>

   更新工作量可以更新“计划时数”任务。 如果项目“更新类型”为“自动”，则更新会立即进行。 当项目更新类型为“手动”时，您必须重新计算时间轴才能查看更新的计划时间。 </p>

   <p>有关使用工作量而不是计划小时来估计任务工作量的信息，请参阅 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>. </p> 
    </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 或继续以下部分。

### 分配 {#assignments}

1. 开始按如上所述编辑任务。
1. 单击 **分配** 中。

   ![](assets/nwe-assignments-section-edit-task-box-350x217.png)

1. 单击 **搜索人员、角色和团队** 然后，开始键入要分配给该任务的用户、角色或团队的名称，然后单击该名称或在该名称显示在列表中时按Enter键。

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
   >
   >* 将工作项重新分配给活动资源。
   >* 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


1. （可选）通过选择 **所有者** 单选按钮。 团队不能是任务的主要受分配人。
1. （视情况而定）更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">持续时间类型</td> 
      <td> <p>这标识了以下各项之间的关系： </p> 
       <ul> 
      <li> <p>分配给任务的资源数 </p> </li> 
      <li> <p>完成任务所需的总工作量 </p> </li> 
      <li> <p> 任务的总持续时间。 </p> </li> 
       </ul> <p>您的Workfront管理员 <span> 或组管理员</span> 为系统或组中的任务选择默认的持续时间类型设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>. </p> <p>持续时间类型允许您根据任务需求设置一致的资源分配。 有关任务的持续时间类型的详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>. </p> <p>从以下选项中进行选择： </p> 
       <ul> 
      <li> <p>计算的分配量 </p> </li> 
      <li> <p> 计算的工作量 </p> </li> 
      <li> <p>投入比导向 </p> </li> 
      <li> <p>简单</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">每次发生的持续时间</td> 
      <td> <p>此操作仅在定期任务的父项上显示。 它显示每个定期任务的持续时间。 有关创建定期任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建定期任务</a>. </p> <p> <b>注释</b>

   在单个定期任务中修改的持续时间不会显示此字段中指示的值。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td> 
      <div> 
      <div> 
      <p>这是您允许任务在完成前保持打开状态的时间。 </p> 
      <p><b>重要信息</b>

   由于任务持续时间通常是计划起始日期与计划完成日期之间的时间长度，因此它会影响项目的时间表。</p>

   <p>要指示任务的持续时间和时间单位，请执行以下操作：</p> 
      <ul> 
      <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">键入时间长度，然后从下拉菜单的可用时间单位中选择。</p> <p><b>笔尖</b></p>
      在任务列表中更新任务的持续时间时，可以使用时间单位的缩写。 </p> </li> 
      </ul> 
      <p> 您可以从下表的常规时间或经过的时间选项中进行选择： </p> 
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
      <td>天数. 这是默认设置。 </td> 
      <td>D</td> 
      </tr> 
      <tr> 
      <td>周</td> 
      <td>三</td> 
      </tr> 
      <tr> 
      <td>月</td> 
      <td>二</td> 
      </tr> 
      <tr> 
      <td>占用分钟数</td> 
      <td>EM</td> 
      </tr> 
      <tr> 
      <td>占用小时数</td> 
      <td>EH</td> 
      </tr> 
      <tr> 
      <td>占用天数</td> 
      <td>ED</td> 
      </tr> 
      <tr> 
      <td>占用周数</td> 
      <td>EW</td> 
      </tr> 
      <tr> 
      <td>占用月数</td> 
      <td>ET</td> 
      </tr> 
      </tbody> 
   </table>

   <p><b>注释</b>

   <p>已用时间是任务持续时间的单位。 任务的“计划起始日期”和“计划完成日期”之间的时间（包括假日、周末和休假时间）。 换言之，已用时间即为日历日的过去。

   常规时间考虑节假日、周末和休假时间，并从任务的“持续时间”中排除这些时间。 有关任务持续时间的详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>. </p>
   </div> 
   </div> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">计划小时</td> 
   <td> <p>指定任务的计划小时数（以小时为单位）。 这是任务的受分配者完成任务所需的实际时间。 当持续时间类型设置为“计算分配”时，您只能为任务指定计划小时数。 有关持续时间类型的更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">分配</td> 
   <td> <p>如果任务约束是计算工作或工作驱动，请指定 <strong>分配%</strong> （分配百分比）。 这是从受让人的计划开始他们可以在此任务上花费的时间。 更改任务分配百分比将更改任务的计划时数。 </p> <p>当“任务约束”为“简单”时，您可以指定以下内容：</p> 
      <ul> 
      <li> <p>每个受分派人的分配小时数。</p> </li> 
      <li> <p>任务的计划小时数</p> </li> 
      <li> <p>任务的持续时间</p> </li> 
      </ul> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">受让人的角色</td> 
   <td> <p>从 <strong>被分派人的角色</strong> 下拉菜单。 这是受分配人可以在此任务中履行的角色。 </p> <p><b>笔尖</b>

   只有与其配置文件中的每个代理人关联的作业角色才会显示在下拉菜单中。</p> </td>
   </tr> 
      </tbody> 
      </table>

1. 单击 **保存** 或继续以下部分。

### 自定义表单

您可以定义默认的自定义表单，在将任务添加到项目时，将其自动附加到任务。 有关设置项目以包含所有新任务的默认任务自定义表单的信息，请参阅文章中的“任务”部分 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 开始编辑上述任务。
1. 单击 **自定义Forms** 在左侧面板中，或单击自定义表单的名称（如果已附加）。

   ![](assets/nwe-custom-forms-section-edit-task-box-350x127.png)

1. 单击 **添加自定义表单** 并选择要与任务关联的自定义表单。 您必须先构建自定义表单，然后才能在此字段中进行选择。 列表中仅显示活动的自定义表单。

   有关构建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。您最多可以在任务中添加10个自定义表单。

1. （视情况而定）如果您将自定义表单附加到任务，请编辑表单上的任何字段。 在保存任务之前，必须指定所有必填字段。

   >[!NOTE]
   >
   >根据Workfront管理员为自定义表单中各个部分设置权限的方式，并非每个人都可以查看或编辑给定自定义表单中的相同字段。 在自定义表单的某个部分中编辑字段的权限取决于您对任务本身拥有的权限。 有关设置任务权限的信息，请参阅 [共享任务](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

1. 单击 **保存** 或继续以下部分。

### 财务 {#finance}

1. 开始编辑任务，如 [编辑任务](#Edit2) 章节。
1. 单击 **金融** 中。

   ![](assets/nwe-finance-section-edit-task-box-350x298.png)

1. 更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">成本类型</td> 
      <td> <p>指定任务的成本类型。 这将根据任务的小时数确定如何计算任务的成本。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
        <li> <p>无成本</p> </li> 
        <li> <p>固定小时 </p> </li> 
        <li> <p> 用户小时 </p> </li> 
        <li> <p> 角色小时</p> </li> 
       </ul> <p>有关跟踪成本的更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a> . 您的Workfront管理员或组管理员为系统或组中的任务选择默认的成本类型设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">收入类型</td> 
      <td> <p>为任务指定收入类型。 这将根据任务上的小时数确定如何计算任务的收入。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
      <li> <p> 不可记帐 </p> </li> 
      <li> <p>用户小时 </p> </li> 
      <li> <p>角色小时 </p> </li> 
      <li> <p>固定小时 </p> </li> 
      <li> <p>受限用户小时 </p> </li> 
      <li> <p>受限角色小时 </p> </li> 
      <li> <p>用户小时加固定 </p> </li> 
      <li> <p>角色小时加固定 </p> </li> 
      <li> <p>固定收入 </p> </li> 
       </ul> <p>有关跟踪收入的更多信息，请参阅<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a> . </p> <p>您的Workfront管理员或组管理员为系统或组中的任务选择默认的收入类型设置。 有关设置项目默认值的信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 或继续使用以下部分。

### 设置 {#settings}

1. 开始编辑任务，如 [编辑任务](#Edit2) 章节。
1. 单击 **设置** 中。

   ![](assets/nwe-settings-section-edit-task-box-350x304.png)

1. 更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">跟踪模式</td> 
      <td> <p>指定如何跟踪任务的进度状态。 </p> <p>从以下选项中进行选择： </p> 
       <ul> 
      <li> <p> 用户必须更新 </p> </li> 
      <li> <p>假设按时 </p> </li> 
      <li> <p>忽略迟到警告</p> </li> 
      <li> <p> 自动完成 </p> </li> 
      <li> <p>前置任务 </p> </li> 
       </ul> <p>有关任务的跟踪模式的更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任务跟踪模式概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源均衡</td> 
      <td> <p>选择 <strong>从资源平衡中排除</strong> 字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">均衡延迟</td> 
      <td> <p>指定调平延迟（以小时为单位）。 </p> <p> 有关调平延迟的更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-leveling-delay.md" class="MCXref xref">更新任务调平延迟</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td> <p>选择要与任务关联的审批流程。 您的Workfront管理员必须定义系统级别的审批流程，然后才能将它们与任务关联。 对审批流程具有管理访问权限的用户也可以创建特定于组的审批流程。 </p> <p>有关创建审批流程的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md">为工作项创建审批流程</a>. 添加审批流程时，请考虑以下事项： </p> 
       <ul>

   <li> <p>列表中仅显示活动的批准流程。 </p> </li>

   <li> <p>系统范围和特定于组的审批流程将显示在列表中。 与项目组以外的组关联的批准流程不会显示在列表中。 </p>

   <p><b>重要信息</b>

   如果项目组发生更改，则之前附加的特定于组的审批流程将变成一次性审批流程。 有关项目组更改或审批流程更改如何影响审批设置的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">组和审批流程更改如何影响分配的审批流程</a>. </p>

   </li>

   <li> <p>您可以定义默认的审批流程，在将任务添加到项目时自动附加到任务。 有关将项目设置为包含默认任务审批流程的信息，请参阅文章中的“任务”部分 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">编辑项目</a>. </p> </li>

   <li> <p>批量编辑任务时，存在以下情况： </p> 
      <ul> 
      <li> <p>从同一组中选择多个任务时，系统级别和组级别审批流程都会显示在此字段中。 </p> </li> 
      <li> <p>当您从不同的组中选择多个任务时，此字段中只显示系统级别的审批流程。 </p> </li> 
      <li> <p>如果任何任务附加了一次性审批流程，则将由您选择的系统级别或组级别审批流程来替代。 </p> </li>

   </ul> </li> 
      </ul> </td> 
     </tr> 
    </tbody> 
   </table>
    </li>

1. 单击&#x200B;**保存**。

<!--notes from the table: <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)</p>       -->

## 在任务标题中编辑任务（受限）

您可以在任务标题中编辑有限量的信息。

系统或组管理员可以自定义您在任务标题中看到的字段。 有关更多信息，请参阅 [使用布局模板自定义对象标头](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


![](assets/qs-task-header-without-approvals-and-with-dependecies-350x17.png)

默认情况下，项目标题中包含以下字段：

* 任务名称
* 完成百分比
* 分配
* 计划完成日期和时间

   >[!CAUTION]
   >
   >某些任务约束和其他依赖关系可能会阻止您编辑此字段。 有关任务约束的信息，请参阅 [任务约束概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* 状态
* 如果您在当前审批流程中设置为审批者，则应做出审批决策

## 批量编辑任务

您可以选择自动保存对列表中的任务所做的更改，同时在列表中批量编辑任务并更新其所有信息。

有关批量保存任务的信息，请参阅文章中的“批量编辑任务”部分 [在列表中编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).
