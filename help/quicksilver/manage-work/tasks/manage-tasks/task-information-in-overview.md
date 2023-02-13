---
product-area: projects
navigation-topic: manage-tasks
title: 在“任务详细信息概览”区域中管理任务信息
description: 在“任务详细信息概览”区域中管理任务信息
author: Alina
feature: Work Management
exl-id: 4980b28f-914d-4cf9-813f-14983aac660b
source-git-commit: 7e591a8eb801da463f05b574c091f68278974ad7
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 5%

---

# 在“任务详细信息概览”区域中管理任务信息

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, do it in both articles)</p>
-->

您可以通过访问“任务详细信息”部分的“概述”区域来查看或编辑任务的信息。 在此区域中，可以查看或编辑的字段数量有限。 有关编辑任务所有信息的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

本文介绍了如何在“任务详细信息”的“概述”区域查看或编辑信息。 有关更新任务详细信息其他区域的信息，请参阅以下文章：

* [在“任务详细信息”部分中管理任务财务](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)
* [将自定义表单添加到对象](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)
* [管理附加到对象的自定义表单](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
   *要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> 计划*</b> </p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> 许可证*</b> </p> </td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>查看或更高权限访问项目和任务</p> <p>如果您具有正确的访问级别，但仍无法编辑任务的“详细信息”部分，请咨询您的Adobe Workfront是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>为项目提供或更高权限</p> <p>查看任务的权限，以在详细信息部分中查看信息。 </p> <p>管理任务的权限以更新详细信息部分中的信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 在“任务详细信息概述”部分中编辑任务信息

1. 转到要查看或编辑的任务。
1. 单击 **任务详细信息** 中。
1. 转到 **概述** 以查看有关任务的更多信息。

   默认情况下，“概述”是“任务详细信息”部分的第一个区域，该区域已展开。

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员设置布局模板的方式，任务详细信息部分中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 在“详细信息”部分的右上角，单击 **概述**.

   >[!TIP]
   >
   >您无法编辑由Workfront自动生成或您无权编辑的字段。

1. 通过单击字段或单击，编辑任何可编辑的字段 **+添加** 向空字段添加信息。
1. 查看或编辑下列任一字段。

   并非所有字段都可编辑。  

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td> <p>有关任务的其他信息</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">参考号</td> 
      <td>这是Workfront为系统中所有对象生成的任务的唯一值。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>具有任务管理权限的用户可以在此字段中指定指向内部或外部页面的链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>选择任务的状态，以指示任务处于开发的哪个阶段。</p> <p>提示：您可以更新任务标题中的任务状态。 </p> </td> 
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
     <tr> 
      <td role="rowheader">持续时间</td> 
      <td> 
       <div> 
        <div> 
         <p>这是您允许任务在完成前保持打开状态的时间。 </p> 
         <p>重要信息：由于任务持续时间通常是计划起始日期与计划完成日期之间的时间长度，因此它会影响项目的时间表。</p> 
         <p>要指示任务的持续时间和时间单位，请执行以下操作：</p> 
         <ul> 
          <li> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">键入时间长度，然后从下拉菜单的可用时间单位中选择。</p> </li> </ul>

   <p><strong>笔尖</strong></p> <p> 在任务列表中更新任务的持续时间时，可以使用时间单位的缩写。 </p>      <p> 您可以从下表的常规时间或经过的时间选项中进行选择： </p> 
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
         <p><strong>注释</strong> </p>
         <p> 已用时间是任务持续时间的单位。 任务的“计划起始日期”和“计划完成日期”之间的时间（包括假日、周末和休假时间）。 换言之，已用时间即为日历日的过去。 常规时间考虑节假日、周末和休假时间，并从任务的“持续时间”中排除这些时间。 有关任务持续时间的详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>. </p> 
         <p> 
         <!--You cannot specify the Duration of a task when the Duration Type of the task is Simple, or when the Task Constraint is Fixed Dates. (NOTE: Anna said this is now possible for all duration types in the Assignments area. It's not here, but to clear confusion, I am drafting this out of here.)--></p> 
        </div> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预计持续时间</td> 
      <td> <p>预计起始日期与预计完成日期之间的天数差。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际持续时间</td> 
      <td> <p>实际开始日期与实际完成日期之间的天数差。 这是完成这项工作实际花了多长时间。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划小时数</td> 
      <td> <p>指定任务的计划小时数（以小时为单位）。 这是任务的受分配者完成任务所需的实际时间。 当持续时间类型设置为“计算分配”时，您只能为任务指定计划小时数。 有关持续时间类型的更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际小时数</td> 
      <td>用户在任务上记录的小时数。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">工作投入 </td> 
      <td> 
       <div> 
        <p>完成任务所需的工作量。 您的项目经理可能会决定使用此字段而不是“计划小时数”来估算完成任务所需的工作量。 仅当满足以下条件时，此字段才可见：</p> 
        <ul> 
         <li> <p>任务具有简单持续时间类型。 </p> <p>提示：如果更改任务“持续时间类型”，此字段将变灰。 </p> </li> 
         <li>您的项目经理已启用使用工作量以自动计算项目上的任务计划小时数字段。 </li> 
        </ul> 
        <p>从以下选项中进行选择：</p> 
        <ul> 
         <li>小</li> 
         <li>中 <span style="font-weight: normal;">（这是新任务的默认值）</span></li> 
         <li>大</li> 
        </ul> 
        <p><strong>注释</strong></p> 
        <p> 更新工作量可以更新“计划时数”任务。 如果项目“更新类型”为“自动”，则更新会立即进行。 当项目更新类型为“手动”时，您必须重新计算时间轴才能查看更新的计划时间。 </p> 
        <p>有关使用工作量而不是计划小时来估计任务工作量的信息，请参阅 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>. </p> 
       </div> </td> 
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
      <td role="rowheader">计划开始日期</td> 
      <td> <p>计划开始任务时。 任务的计划起始日期会设置并受多种因素的影响：</p> 
       <ul> 
        <li>根据任务计划起始日期的全系统首选项，项目上新任务的开始日期可以是今天，也可以是项目的开始日期（默认情况下）。 <span>与项目关联的组的组管理员也可以为组设置此首选项。</span> 有关系统级别或组级别任务首选项的详细信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">配置系统范围的任务和问题首选项</a>.</li> 
        <li>根据任务的前置任务，Workfront会选择计划的开始日期作为前置任务完成后的下一个可用日期，或根据前置任务关系开始。 有关前身关系的更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任务前置任务概述</a>.</li> 
        <li>当任务约束为“固定日期”或“必须开始”时，项目经理或任务责任人可以人工设置计划的起始日期。 有关任务约束的详细信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预计开始日期</td> 
      <td> <p>根据先前任务的进度和完成情况开始任务的“实际生活”日期。 这是一个计算字段，您无法手动编辑它。</p> <p> 在首次计划项目时，预计起始日期和计划起始日期通过相同的方式开始。 如果项目演变并且任务尚未开始，则预计起始日期可能会从计划起始日期移开。 有关预计开始日期的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-start-date.md" class="MCXref xref">项目预计起始日期概览</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际开始日期</td> 
      <td> <p>指定任务的实际开始日期。 当将任务的状态更改为“进行中”时，通常会自动填充默认值。 项目经理或任务责任人也可以手动修改实际起始日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期</td> 
      <td> <p>计划任务时显示的预期完成日期。 计划完成日期可通过多种因素进行设置：</p> 
       <ul> 
        <li>通过将任务的持续时间添加到计划起始日期，从计划起始日期计算计划完成日期。 当项目经理或Workfront指定任务的持续时间时，这会触发对计划完成日期的更新。 如果计划日期发生更改，则通常是因为的持续时间已更新。</li> 
        <li>当任务约束为“固定日期”或“必须完成”时，项目经理或任务责任人可以人工设置计划完成日期。 有关任务约束的详细信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">任务约束概述</a>.</li> 
        <li>如果任务的持续时间类型发生更改，并且任务上的资源数量同时发生更改，则计划完成日期也将发生更改。 有关持续时间类型的更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务持续时间和持续时间类型概述</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预计完成日期</td> 
      <td> <p>根据先前任务的进度和被分派人对任务进行的进度更新，完成任务的“实际生命”日期。 这是一个计算字段，您无法手动编辑它。</p> <p> 在项目首次计划时，预计完成日期和计划完成日期的起始日期是相同的。 如果项目演变，并且任务尚未开始，则预计完成日期可能会从计划完成日期移开。 有关预计完成日期的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的预计完成日期概览</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际完成日期</td> 
      <td> <p>指定任务完成的实际日期和时间。 任务完成的默认日期和时间始终与状态变为“完成”时的实际时间一致。 项目经理或任务责任人也可以手动修改实际完成日期。 </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">提交日期</td> 
      <td> <p>这是分配给任务的用户提交完成任务的日期。 这可能与计划完成日期不同。 只有被分配者才能编辑此字段。有关Workfront中提交日期的信息，请参阅 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">提交日期概述</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">输入日期</td> 
      <td>创建任务的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">输入者</td> 
      <td>创建任务的人员。</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">上次更新日期</td> 
      <td> <p>上次更新任务的日期。 </p> <p>提示：每次有人编辑并保存任务时，Workfront都会记录“更新日期”。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">上次更新者</td> 
      <td> <p>上次更新任务的人员。</p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">循环频率</td> 
      <td> <p>此操作仅在定期任务的父项上显示。 定期中的任务发生的频率。 有关创建定期任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建定期任务</a>. </p> </td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader">每次发生的持续时间</td> 
      <td> <p>此操作仅在定期任务的父项上显示。 它显示每个定期任务的持续时间。 有关创建定期任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建定期任务</a>. </p> <p><strong>注释</strong></p> <p> 在单个定期任务中修改的持续时间不会显示此字段中指示的值。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted, to keep it focused JUST on the Overview section and not others.) </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Custom Forms</strong> to add or forms or edit information on the existing custom forms.&nbsp;</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand any of the existing custom forms to edit them, or start typing in the <strong>Add custom form</strong> box in the upper-right corner to add a new form. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding or editing custom forms, see the following articles:</p>
   -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md" class="MCXref xref">Add a custom form to an object</a> </li>   
     -->

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md" class="MCXref xref">Manage custom forms attached to objects</a> </li>   
     -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click&nbsp;<strong>Finance</strong>, then <strong>Edit Finance</strong> to view or edit financial information for the task. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Expand the <strong>Finance</strong> area in the Details section, then double-click any editable field to update it. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about editing financial information for a task, see <a href="../../../manage-work/tasks/manage-tasks/task-finances-in-details.md" class="MCXref xref">Manage task finances in the Task Details section</a>. </p>
   -->

1. 单击 **保存更改**.
