---
content-type: reference
navigation-topic: workfront-navigation
title: 术语表 [!DNL Adobe Workfront] 术语
description: 此 [!DNL Adobe Workfront] 词汇表列出了Adobe Workfront中的常用术语。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '19138'
ht-degree: 0%

---

# 术语表 [!DNL Adobe Workfront] 术语

>[!IMPORTANT]
>
>本文可用作参考，便于您了解可能遇到的术语 [!DNL Adobe Workfront] 应用程序，在 [!DNL Workfront] 文档，或者在通常情况下谈论规划和管理工作时。 我们当前正在更新此信息，因此，此表可能不完整。 当我们认为此信息详尽无遗时，我们将删除此免责声明。

下表列出了Adobe Workfront中的常用术语：

## A - C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>对象名称</strong></th> 
   <th><strong>描述</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL访问级别]</td> 
   <td>确定用户如何与Workfront中的不同对象和工具交互的用户配置文件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL活动任务]</td> 
   <td>当前项目中的未完成任务，未阻止前置任务处理该任务，并且没有具有未来计划开始日期的任务限制。 换言之，它可以在今天发挥作用。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL活动]</td> 
   <td>In [!DNL Workfront Goals]，活动是目标的进度指示器。 它可以是您手动更新的进度条，也可以是与目标关联的项目。 您不能在报表中显示活动，也不能通过 [!DNL Workfront] API。 有关活动的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront目标中的结果和活动入门</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL实际成本]</td> 
   <td> <p>对于任务和问题，这是与记录的实际小时数关联的成本，与分配给任务或问题的资源的每小时成本费率相关。 对于项目，这是项目任务和问题中所有[！UICONTROL实际成本]的总和。 有关信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL实际费用成本]</td> 
   <td> <p>为项目或任务记录的所有费用的[！UICONTROL实际金额]的总和。</p> <b>示例 </b>
   <p>如果您为任务1创建费用并在[！UICONTROL实际金额]字段中输入$600.00，则此任务的[！UICONTROL实际费用成本]为$600.00。 </p> 
   <p>对于项目， [!DNL Workfront] 使用以下公式计算[！UICONTROL实际费用成本]：</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs)</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL实际小时数]</td> 
   <td> <p>在项目、任务或问题报告中，[！UICONTROL实际小时数]是在项目、任务或问题上记录的所有小时数的总和。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span> 如果在任务1的[！UICONTROL更新]选项卡中，单击“记录时间”并输入25小时，则任务1的实际小时数= 25小时。 </p> <p>[!DNL Workfront] 使用以下公式计算父任务或项目的[！UICONTROL实际小时数]：</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL实际劳力成本]</td> 
   <td> <p>与投资于任务或项目的人工相关的[！UICONTROL实际成本]。 </p> <p>对于任务， [!DNL Workfront] 使用以下公式计算[！UICONTROL实际劳力成本]：</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>如果任务的[！UICONTROL成本类型]为[！UICONTROL用户小时]， [!DNL Workfront] 使用用户率。 如果任务的[！UICONTROL成本类型]为[！UICONTROL角色小时]， [!DNL Workfront] 使用工作角色费率计算[！UICONTROL实际劳力成本]。 </p> <p>对于项目， [!DNL Workfront] 使用以下公式计算[！UICONTROL实际劳力成本]：</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>例如，如果用户为具有[！UICONTROL用户每小时] [！UICONTROL成本类型]的任务记录5小时，并且其小时费率为$100，则[！UICONTROL实际劳力成本]为$500。</p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL实际收入] </td> 
   <td> <p>项目或任务的[！UICONTROL实际收入]是与项目或任务的[！UICONTROL实际小时数]关联的货币金额。 </p> <p>有关在中跟踪收入的信息 [!DNL Workfront]，请参见 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL实际开始]</td> 
   <td>用户更改分配给他们的工作的进行中的对象时的时间戳。</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[！UICONTROL Agile]方法</td> 
   <td>一种基于跨职能团队的需求和解决方案的协作演变的一种方法。 它鼓励基于固定时间表的灵活性和变化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Agile团队]</td> 
   <td>与传统团队不同，他们从积压工作中获取潜在工作，并在称为[！UICONTROL迭代]的指定时间段内处理该工作。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL All Teams]</td> 
   <td> <p>当在[！UICONTROL筛选器]中引用此字段时，此字段显示属于登录用户所属任何团队的用户，或分配给登录用户所属任何团队的工作项。 </p> <p>我们建议在筛选器中使用此字段，以使报告在与其他用户共享时更加通用。 这样，您只能构建一个报告，该报告将根据查看信息的登录者显示不同的信息，因为始终为登录用户自定义信息。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配日期]</td> 
   <td> <p>您可以在以下类型的报表中找到此字段：</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[！UICONTROL项目]（财务数据）</li> 
     <li>[！UICONTROL预算小时]</li> 
    </ul> <p>对于<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[！UICONTROL项目（财务数据）]报表： </p> 
    <ul> 
     <li>在尝试了解时生成此报告 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 分配给您资源的[！UICONTROL计划小时数]数量。</li> 
     <li> <p>[！UICONTROL分配日期]是开始向任务分配[！UICONTROL工作角色]的一周的第一天（星期日）。 资源（[！UICONTROL工作角色]）可以具有的[！UICONTROL分配日期与分配给它的任务的[！UICONTROL持续时间]期间的周数相同。 如果任务跨越多个月，则当月的第一天也可能成为[！UICONTROL分配日期]（如果其在任务的[！UICONTROL持续时间]之内）。</p> <p>例如，您可以将[！UICONTROL工作角色]分配给跨越3周且有90个[！UICONTROL计划小时数的任务。 这些小时数在任务持续时间内平均分布，这使得每天都将6 [！UICONTROL已计划小时数]分配给您的工作角色：</p> <p><em> [！UICONTROL每日计划小时数] = [！UICONTROL总计划小时数]/[！UICONTROL工作天数]在任务的[！UICONTROL持续时间] </em> </p> <p>因此，该任务包含三个[！UICONTROL分配日期]，在任务的[！UICONTROL持续时间]期间，每个星期日的分配日期各一个，每个分配日期具有特定数量的[！UICONTROL计划小时数]。<br>如果任务在一个月的最后一周中期开始，并在新月开始后两周结束，则该任务将有四个[！UICONTROL分配日期]：在任务的[！UICONTROL持续时间]期间，每个星期日的分配日期各一个，新月第一天分配日期各一个。</p> <p>为了充分利用此信息，我们建议您构建 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 项目（财务数据）报告并添加[！UICONTROL分配日期]的矩阵分组，然后每周、每月、每季度或每年对结果进行分组，以获得最准确的数据。<br>有关构建矩阵分组的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">创建矩阵报表</a>.</p> </li> 
    </ul> <p>仅当与财务信息关联的数据的年龄少于5岁时，财务信息才会填充在[！UICONTROL项目（财务数据）]报表中。 例如，如果某个工作角色在2015年1月分配到了任务，而今天是2021年9月，则工作角色的[！UICONTROL分配日期]等财务字段未填充到[！UICONTROL项目（财务数据）]报表中。 </p> 
    <div> 
     <p>对于[！UICONTROL预算小时数]报表：</p> 
     <ul> 
      <li>尝试了解在资源规划者中分配给您的资源或您的项目的[！UICONTROL预算小时数]时，请构建此报告。</li> 
      <li> <p>[！UICONTROL分配日期]是您在[！UICONTROL资源规划者]中为其预算小时数的一周的第一天（星期日）。 </p> <p>提示：   <p>如果一周持续两个月，它将在报告中生成两行：一行对应于一周的第一天（第一周的星期日，在第一个月内），第二行显示第二个月的第一天。 </p> <p>例如，如果您为用户预留6月30日（星期日）至7月6日（星期六）这周的8小时，则两行显示[！UICONTROL分配日期] 6月30日和7月1日。 </p> </p> <p>有关编制资源预算的信息，请参见 [!DNL Resource Planner]，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">预算中的资源 [!DNL Resource Planner] 使用[！UICONTROL项目]和[！UICONTROL角色]视图</a>.</p> <p>有关构建[！UICONTROL预算小时数]报表的信息，请参阅 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">报告：预算小时</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公告]</td> 
   <td> <p>在系统内向用户传递信息的方法。 此信息通常来自 [!DNL Workfront] 发送给管理员或从管理员发送给用户。 </p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">发送公告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL应用程序集成]</td> 
   <td>应用程序通常表示软件应用程序的连接器，但也可以表示处理数据的特殊功能。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL批准者决定]</td> 
   <td> <p>在[！UICONTROL验证审批]报告中，此字段显示不再活动的验证的验证审批决策。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL审批者阶段]</td> 
   <td>在[！UICONTROL验证审批报告]中，此字段显示有关当前阶段的验证的信息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL审批]</td> 
   <td> <p>给定工作项（如任务、文档或时间表）可能要求主管或其他用户签发该工作项。 此注销过程称为批准。 </p> <p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL批准日期]</td> 
   <td>在[！UICONTROL验证审批]报告中，此字段显示批准验证的日期。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL审批者]</td> 
   <td>必须注销给定工作项的用户或工作角色，或在时间表上批准小时条目的用户。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配给]</td> 
   <td> <p>在[！UICONTROL任务或问题]报告中，此字段显示任务或问题的所有者或[！UICONTROL主要被分配人]。 您也可以按此字段进行筛选或分组。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配]</td> 
   <td>分配给问题或任务的用户、工作角色或团队。 项目、项目组合或项目群不能具有分配。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配]</td> 
   <td> <p>在[！UICONTROL任务]或[！UICONTROL问题]报告中，此字段显示分配给任务或问题的所有实体（用户、工作角色、团队）的列表。 您可以使用字段[！UICONTROL任务用户]和[！UICONTROL任务角色]按此字段进行筛选。 您可以使用“团队”字段按分配给任务或问题的团队进行筛选。 您无法按此字段对报告进行分组。</p> <p>已放置在[！UICONTROL回收站]中的工作项将继续显示在引用了[！UICONTROL分配]对象的某些报表中，其中 [!DNL OR] 过滤器修饰符已使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配角色]</td> 
   <td>
   <p>在[！UICONTROL任务]或[！UICONTROL问题]报告中，此字段显示有关分配给任务或问题的工作角色的信息。 此字段显示[！UICONTROL主要所有者]，以及分配给任务或问题的其他工作角色。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分配状态]</td> 
   <td> <p>在工作、任务或问题报告中，[！UICONTROL工作状态]显示分配给工作项的用户是单击[！UICONTROL处理该工作]还是单击[！UICONTROL完成]按钮接受或完成该工作。 存在以下[！UICONTROL分配状态]：</p> 
    <ul> 
     <li><b>[！UICONTROL已请求]</b>：用户已被分配给任务或问题，但尚未单击[！UICONTROL处理它]按钮开始处理。</li> 
     <li><b>[！UICONTROL正在工作]</b>：用户已单击[！UICONTROL处理此项工作]按钮，并且当前正在处理该项目。 </li> 
     <li><b>[！UICONTROL完成]</b>：用户已单击[！UICONTROL完成]按钮并完成了对该项的工作。 </li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[！UICONTROL处理此工作]和[！UICONTROL完成]按钮概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任务团队]</td> 
   <td>
   <p>在[！UICONTROL任务]或[！UICONTROL问题]报告中，此字段显示有关分配给任务或问题的团队的信息。 字段显示[！UICONTROL主要所有者]，以及分配给任务或问题的其他团队。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任务用户]</td> 
   <td>
   <p>在[！UICONTROL任务]或[！UICONTROL问题]报告中，此字段显示有关分配给任务或问题的用户的信息。 此字段显示[！UICONTROL主要所有者]，以及分配给任务或问题的其他用户。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL属性]</td> 
   <td>属性是的特质 [!DNL Workfront] 对象。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL审核区域]</td> 
   <td> <p>审核是记录Workfront中发生操作的系统消息。 记录了以下审计类型：</p> 
    <ul> 
     <li>[！UICONTROL范围更改]</li> 
     <li>[！UICONTROL附件操作]</li> 
     <li>[！UICONTROL常规编辑]</li> 
     <li>[！UICONTROL状态更改]</li> 
     <li>[！UICONTROL注释]</li> 
     <li>[！UICONTROL组合条目]</li> 
     <li>[！UICONTROL错误条目]</li> 
     <li>[！UICONTROL状态更改]</li> 
     <li>[！UICONTROL订阅更改]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL审核记录]</td> 
   <td>由事件自动生成的注释集合，这些事件通过“记录的更改”（[！UICONTROL审核区域]）进行跟踪。 每条注释都记录操作者、操作者以及操作时间。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Automatic And On Change]</td> 
   <td> <p>[！UICONTROL项目更新]类型之一。 当夜间重新计算流程运行以及对项目或项目中的任务进行任何更新时，这将重新计算项目的预计和计划时间表。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>可用性</p></td> 
   <td> <p>此术语与“用户可用性”或“资源可用性”相关，它说明了资源（用户或工作角色）可用工作的时间。 </p> 
   <p>Workfront使用多个字段并根据系统中资源管理首选项的设置计算用户可用性。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>. </p>
   <p>有关资源可用性的详细信息，请参见 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">资源管理入门</a></p>
   另外，“容量”也用于表示资源可用性。 
   </td> 
  </tr>

<tr> 
   <td>[！UICONTROL Automatic Only]</td> 
   <td> <p>[！UICONTROL项目更新]类型之一。 当夜间重新计算流程运行时，这将重新计算预计时间表和计划时间线。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[！UICONTROL BAU]</td> 
   <td>有助于实现日常主要业务目标的“一切照常”工作。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL积压]</td> 
   <td>敏捷环境中的区域，新问题会保留到准备好处理时为止。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL基线]</td> 
   <td>在敏捷环境中测量迭代的数据源。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[！UICONTROL开票记录]</td> 
   <td> <p>记录可记帐的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">创建开票记录</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>开票记录状态</td> 
   <td> <p>在开票记录或小时报表中，开票记录的状态指示开票记录是已经开票还是未开票。 您无法删除项目或编辑与已记帐记帐记录关联的时间。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >创建开票记录</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[！UICONTROL品牌]</td> 
   <td>自定义的过程 [!DNL Workfront] 为界面提供使用您的颜色和徽标镜像您的公司的外观。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL痕迹导航]</td> 
   <td> <p>页面顶部的区域，显示用户在应用程序中的分层位置。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有关更多信息，请参阅 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预算状态]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与以下功能相关 [!DNL Workfront] 已删除，无法更新字段。 </p> <p>此字段显示项目是否已添加到[！UICONTROL Capacity Planner]，以及是否已为其完成预算计算。 [！UICONTROL Capacity Planner]已从删除 [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预算完成日期]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与以下功能相关 [!DNL Workfront] 已删除。 无法更新此字段。 </p>
   <p> 此字段在[！UICONTROL项目]和[！UICONTROL任务]报告和列表中仍然可见。</p>  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预算成本]</td>

<td> <p>这是与项目预算资源关联的成本。 </p>
   <p>该字段显示在以下区域 [!DNL Workfront] 名称下：</p>
   <ul>
   <li><strong>[！UICONTROL预算成本]</strong>：在[！UICONTROL业务案例摘要]面板中</li>
   <li><strong>[！UICONTROL成本]</strong>：在按[！UICONTROL成本]查看信息时，显示在[！UICONTROL利用率]区域</li>
   <li><strong>[！UICONTROL项目预算成本]</strong>：在列表和报告中</li>
   </ul>   
    <p>使用以下公式计算项目的[！UICONTROL预算成本]：</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>有关计算[！UICONTROL预算成本]的更多信息，并了解中此概念的各种名称 [!DNL Workfront]，请参见 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">计算项目预算成本</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL预算小时数]</td> 
   <td> <p>为完成项目所需的工作的资源预算小时数。 此字段是指在[！UICONTROL业务案例]的[！UICONTROL资源预算]区域（或[！UICONTROL资源规划者]）中为项目或项目资源预算的小时数。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的[！UICONTROL预算劳力成本]和[！UICONTROL预算小时数]</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 有关在中为用户编制预算的信息 [!DNL Resource Planner]，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">预算中的资源 [!DNL Resource Planner] 使用[！UICONTROL项目]和[！UICONTROL角色]视图</a>. </p> 
    <p>[！UICONTROL Business Case]或[！UICONTROL Resource Planner]的[！UICONTROL Resource Budgeting]区域中的预算小时数显示在以下区域中 [!DNL Workfront] 和下：</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[！UICONTROL预算小时数]显示名称</strong></td> 
        <td><strong>领域 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL小时]</td> 
        <td>[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]区域</td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL BDG]</td> 
        <td>由[！UICONTROL小时数]查看的[！UICONTROL资源规划者]</td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL预算小时数]</td> 
        <td> <p>利用率报表[！UICONTROL小时数]视图</p> <p>有关[！UICONTROL利用率]报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[！UICONTROL资源利用率]报告概述</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL花蕾。 小时]</td> 
        <td> <p>[！UICONTROL预算小时数]报告</p><p>预算小时数报表中的[！UICONTROL预算小时数]对象引用与已弃用的资源管理工具相关的信息。 仅“[！UICONTROL Bud. 此报表中的“小时数”字段是指在项目的[！UICONTROL Business Case]的[！UICONTROL Resource Planner]或[！UICONTROL Resource Budgeting]区域中预算的小时数。 </p> <p>有关创建报告的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[！UICONTROL资源规划者预算小时数] </td> 
        <td> <p>可在以下报表中找到：</p>
        <ul>
        <li>[！UICONTROL项目]报告
        <li>[！UICONTROL项目（财务数据）]报表
        <li>[！UICONTROL任务]报告
        <li>[！UICONTROL问题]报告
        <li>[！UICONTROL预算小时数]报告</li>
        </ul>
         <p>有关创建报告的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>中对[！UICONTROL预算小时数]的任何其他提及 [!DNL Adobe Workfront] 指使用已从Workfront中删除的已弃用功能进行预算的小时数。 这些是仅供查看的字段，在使用当前资源预算编制工具时，不会更新为当前信息。 </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预算劳力成本]</td> 
   <td> <p>这是与您作为资源经理为工作角色在项目上需要完成的工作进行预算关联的小时数。 </p> <p>使用以下公式计算项目报表中的[！UICONTROL预算劳力成本]：</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>此字段可能是指以下内容：</p> 
    <ul> 
     <li> <p>显示在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]区域或[！UICONTROL Resource Planner]中与项目工作角色成本关联的人工成本。 有关计算[！UICONTROL预算劳力成本]的信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[！UICONTROL了解项目的预算劳力成本]和[！UICONTROL预算小时数]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]区域中显示的人工成本，反映了从链接到项目的计划中所估算的[！UICONTROL人员成本] [!DNL Scenario Planner] 当您使用Scenario Planner来预算项目资源时。 有关计划的信息，请参阅 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">Scenario Planner中的计划概述</a>. </p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> </li> 
     <p>它显示在以下名称的以下区域：</p>
   <ul>
   <li><strong>[！UICONTROL预算劳力成本]</strong>：在[！UICONTROL Business Case]的[！UICONTROL Resource Budgeting]区域。
   <li><strong>[！UICONTROL预算成本]</strong>：在[！UICONTROL利用率]报表[！UICONTROL成本]视图中
   <p>有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用率信息 </a>.</p>
   <li><strong>[！UICONTROL BDG]</strong>：在 [!DNL Resource Planner] 项目或 [!DNL Role] 视图，按成本查看时
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>：在以下报表中： 
   <ul>
    <li>[！UICONTROL项目]报告</li>
    <li>[！UICONTROL项目（财务数据）]报表</li>
    <li>[！UICONTROL任务]报告</li>
    <li>[！UICONTROL问题]报告</li>
    <li>[！UICONTROL预算小时数]报告</li> 
    </ul>
    <p>有关创建报告的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[！UICONTROL预算开始日期]</td> 
  <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与以下功能相关 [!DNL Workfront] 已删除。 无法更新此字段。</p>
  <p>这些区域已从 [!DNL Workfront]. </p> 
  <p>该字段在[！UICONTROL项目]和[！UICONTROL任务]报告和列表中仍然可见。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL燃尽图]</td> 
   <td>折线图，提供已完成工作和剩余工作的可视化表示形式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL商业案例]</td> 
   <td> <p>用于评估项目是否应从[！UICONTROL Idea]状态前移到[！UICONTROL Planning]状态的工具。 换句话说，[！UICONTROL业务案例]可帮助组织确定启动和完成项目是否值得，尤其是在将项目与项目组合中的其他项目进行比较时。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">为项目创建[！UICONTROL业务案例] </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与以下功能相关 [!DNL Workfront] 已删除。 无法更新此字段。</p> <p>此字段在项目和[！UICONTROL任务]列表及报告中仍然可见。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计算分配]</td> 
   <td> <p>任务[！UICONTROL持续时间]类型之一。 这将根据任务的[！UICONTROL工期]和[！UICONTROL所需工作]计算分配到该任务的用户在8小时工作日中分配给该任务的百分比。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[！UICONTROL工期]和[！UICONTROL工期类型]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计算工作量]</td> 
   <td> <p>[！UICONTROL持续时间类型]任务之一。 考虑到[！UICONTROL持续时间]和用户[！UICONTROL分配]百分比（基于8小时工作日），这将计算任务的[！UICONTROL所需工时]。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[！UICONTROL工期]和[！UICONTROL工期类型]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL日历]</td> 
   <td> <p>有两种类型的日历 [!DNL Workfront]：[！UICONTROL主页日程表]和日程表报告。</p> <p>[！UICONTROL主页日程表]是一个个人日程表，允许用户根据以下时间内的可用小时数管理其工作量： [!DNL Workfront]. 用户还可以将其[！UICONTROL主日历]与 [!DNL Outlook] ([!DNL Google] 和 [!DNL Microsoft] 集成即将推出)。 </p> <p>有关[！UICONTROL主页日程表]的详细信息，请参阅 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[！UICONTROL主日历]视图</a>.</p> <p>日历报告是一种动态报告，用户可以在其中查看事件的日期和其他重要详细信息，包括到期日、工作状态以及事件被分配到的用户。</p> <p> 有关日历报表的详细信息，请参阅 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">日历报表概述</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[！UICONTROL可以启动]</td> 
   <td> <p>此字段指示任务是否准备好开始处理。 如果任务的[！UICONTROL可以开始]字段已准备好开始工作，则将任务设置为[！UICONTROL True]。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">任务的“[！UICONTROL可以开始]”概述</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>能力</p> </td> 
   <td> <p>资源的可用时间，当资源可以分配给工作时。 请参阅“可用性”。 </p></td> 
  </tr>

<tr> 
   <td> <p>[！UICONTROL类别]</p> </td> 
   <td> <p>类别是自定义表单。 您可以为此对象生成报告，也可以将其显示在其他对象报告中。 并非所有对象都具有自定义表单或类别。 以下对象可以具有自定义表单： <br></p> 
    <ul> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL任务]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL文档]</li> 
     <li>[！UICONTROL费用]</li> 
     <li>[！UICONTROL程序]</li> 
     <li>[！UICONTROL用户]</li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL迭代]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL类别名称]</td> 
   <td> <p>当作为列添加到以下任何对象的视图时，它会显示与这些对象关联的所有自定义表单的列表：</p> 
    <ul> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL任务]<br></li> 
     <li>[！UICONTROL问题]<br></li> 
     <li>[！UICONTROLPortfolio]<br></li> 
     <li>[！UICONTROL文档]<br></li> 
     <li>[！UICONTROL费用]<br></li> 
     <li>[！UICONTROL程序]<br></li> 
     <li>[！UICONTROL用户]<br></li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL更改管理]</td> 
   <td>一个实践领域，侧重于定义、理解和调整计划工作，以适应范围、时间表、成本和资源因素的变化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL更改顺序]</td> 
   <td>针对概述对商定范围的请求更改的项目提出的一种问题。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL仅更改]</td> 
   <td>[！UICONTROL更新类型]项目之一。 仅在对项目或任务进行任务更新或编辑时更新[！UICONTROL项目预计]和[！UICONTROL计划]时间表。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL更改顺序]</td> 
   <td> <p>[！UICONTROL Issue]类型之一，通常表示在完成项目之前必须完成计划外的工作量。</p> <p>有关[！UICONTROL问题]类型的更多信息，请参阅文章中的“默认问题类型”部分 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">自定义默认问题类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL子任务]</td> 
   <td>作为[！UICONTROL父任务] （[！UICONTROL摘要任务]）的[！UICONTROL子任务]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL子项]</td> 
   <td>[！UICONTROL子任务]到[！UICONTROL父任务] （[！UICONTROL摘要任务]）的集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Coaching]和[！UICONTROL Training]</td> 
   <td>学习模块、认证、标准或实践社区。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL提交]</td> 
   <td>一种通信工具，供用户设置对任务交付项的期望。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL提交日期]</td> 
   <td>一种通信工具，供用户设置对任务交付项的期望。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Communication]和[！UICONTROL Reporting]</td> 
   <td>用于审查项目、项目群或项目组合的例外情况和运行状况的标准</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公司]</td> 
   <td> <p>[！UICONTROL公司]是中的组织单位 [!DNL Workfront]. </p> 
   <p> 您可以将用户或项目与一个公司关联。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">创建和编辑公司</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成日期]</td> 
   <td> <p>设置完成项目、任务或问题的日期。 中有多种类型的[！UICONTROL完成日期] [!DNL Workfront]：</p> 
    <ul> 
     <li>[！UICONTROL实际完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">项目概述[！UICONTROL实际完成日期] </a>.</li> 
     <li>[！UICONTROL计划完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">设置项目[！UICONTROL计划完成日期]</a> 和 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务概述[！UICONTROL计划完成日期]</a>.</li> 
     <li>[！UICONTROL预计完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的[！UICONTROL预计完成日期]概述</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成日]</td> 
   <td>相对于[！UICONTROL模板]的开始日期，[！UICONTROL模板任务]或[！UICONTROL模板]应完成的日期。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成模式]</td> 
   <td> <p>这指示如何将项目标记为[！UICONTROL完成]。 它可以有两个值：</p> 
    <ul> 
     <li>[！UICONTROL手动]：用户必须将项目状态更改为[！UICONTROL完成]。</li> 
     <li>[！UICONTROL自动]：当项目中的所有任务全部完成并关闭所有问题时，项目状态将自动更改为[！UICONTROL完成]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL条件]</td> 
   <td> <p>这是任务、问题或项目进度的可视化表示形式。</p> <p>对于项目，条件可以由项目所有者手动设置，也可以由自动设置 [!DNL Workfront]，基于项目的进度状态。 </p> <p>项目条件的可能值包括：</p> 
    <ul> 
     <li>[！UICONTROL On Target]</li> 
     <li>[！UICONTROL处于风险中]</li> 
     <li>[！UICONTROL存在问题]</li> 
    </ul> <p>有关项目条件的更多信息，请参阅文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[！UICONTROL项目条件]和[！UICONTROL条件类型]概述</a>.</p>
     <p>您可以将任务和问题条件与可在报告中显示的数字相关联。 以下列表显示了任务和问题条件的默认名称和编号。 您的系统管理员可以更新条件的名称，并且可以添加具有不同编号的新条件。 将数字与条件关联后，便无法对其进行编辑。  </p> 
     <p>对于任务，条件由任务所有者手动设置。 任务条件的可能值包括：</p> 
    <ul> 
     <li>[！UICONTROL进展顺利] (0)<br></li> 
     <li> [！UICONTROL一些问题] (1)<br></li> 
     <li>[！UICONTROL主要障碍] (2)</li> 
    </ul> <p>有关任务条件的更多信息，请参阅文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任务和问题的[！UICONTROL条件]</a>.</p> <p>对于问题，条件由问题所有者手动设置。 问题条件的可能值包括：<br></p> 
    <ul> 
     <li>[！UICONTROL进展顺利] (0)<br></li> 
     <li>[！UICONTROL一些问题] (1)<br></li> 
     <li>[！UICONTROL主要障碍] (2)</li> 
    </ul> 
   <p><b>注释</b></p>
    <p>在[！UICONTROL Journal Entry]报表中跟踪[！UICONTROL Condition]字段时，[！UICONTROL New]和[！UICONTROL Old Number Values]会显示与条件关联的编号而不是其名称。 如果最初没有为任务或问题定义条件，而您稍后更新了该条件，则捕获更新的日志条目会将[！UICONTROL条件]字段的[！UICONTROL旧编号值]显示为 — 2,147,483,648。 另请参阅本文中的“[！UICONTROL新数字值]”、“[！UICONTROL旧数字值]”和“[！UICONTROL日志条目]”。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL条件更新]</td> 
   <td> <p>此字段显示任务、项目或问题的当前条件。 此选项显示任务、项目或问题的所有者在[！UICONTROL更新状态]字段中提供的最新更新以及新条件。</p> <p>对条件更新所做的注释不会显示在[！UICONTROL Condition Update]列中；只会显示主更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL约束日期]</td> 
   <td> <p>如果您使用的是绑定到特定日期的[！UICONTROL任务限制]，例如[！UICONTROL必须开始日期]，则该特定日期将成为任务的[！UICONTROL限制日期]。</p> <p>以下任务约束将更新[！UICONTROL约束日期]字段：</p> 
    <ul> 
     <li>[！UICONTROL必须开始于]</li> 
     <li>[！UICONTROL必须完成于]</li> 
     <li>[！UICONTROL开始时间不晚于]</li> 
     <li>[！UICONTROL开始时间不早于]</li> 
    </ul> <p>提示：   
     <ul> 
      <li> <p>具有[！UICONTROL约束日期]的任务没有[！UICONTROL约束日期]。 </p> </li> 
      <li> <p> [！UICONTROL约束日期]只能在报表或自定义视图中查看。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL约束日]</td> 
   <td> <p>如果在模板任务中使用与特定日期关联的任务限制日期，例如必须开始日期，则该特定日期将成为模板任务的限制日期。</p> <p>以下任务约束将更新[！UICONTROL约束日]字段：</p> 
    <ul> 
     <li>[！UICONTROL必须开始于]</li> 
     <li>[！UICONTROL必须完成于]</li> 
     <li>[！UICONTROL开始时间不晚于]</li> 
     <li>[！UICONTROL开始时间不早于]</li> 
    </ul> <p>提示：[！UICONTROL约束日]只能在报表或自定义视图中查看。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL约束类型]</td> 
   <td> <p>任务的计划趋势。 例如，[！UICONTROL将计划任务尽快开始，[！UICONTROL完成时间不晚于]将计划任务在[！UICONTROL约束日期]之前完成，并且不晚于。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[！UICONTROL任务约束]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上下文菜单]</td> 
   <td>位于屏幕左侧的菜单，在该菜单上，项目会更改为与活动内容相关联。 例如，当用户查看项目时，[！UICONTROL上下文菜单]将显示指向与项目相关的信息和工具的链接。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL转换的问题发起人]</td> 
   <td>项目或任务报告中的一个字段，当问题被转化为项目或任务时，该字段显示有关作为问题的[！UICONTROL主要联系人]的用户的信息。 该字段还显示在[！UICONTROL项目详细信息]部分中，其中显示已转换问题的[！UICONTROL主要联系人]的名称。 另请参阅本文中的“[！UICONTROL主要联系人]”。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL成本]</td> 
   <td> <p>完成项目、任务或问题时必须花费的货币金额。 </p> <p>您可以跟踪与项目相关的人力、费用和风险的各种成本类型。有关在中跟踪成本的信息， [!DNL Workfront] 参见 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟踪成本</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL成本类型]</td> 
   <td>对于任务，[！UICONTROL成本类型]确定该任务如何应计成本。 某些示例包括[！UICONTROL固定小时]、[！UICONTROL用户小时]和[！UICONTROL用户小时加固定]。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL跨项目依赖关系]</td> 
   <td> <p>一个项目的任务依赖于另一个项目的任务。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">创建跨项目前置任务</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL自定义数据]</td> 
   <td> <p>组织特有的数据。 组织可以自定义 [!DNL Workfront] 创建自定义表单和自定义字段以应用。 此自定义信息可推动KPI、审核和需求组合的报告。 </p> <p>[！UICONTROL自定义数据]可以链接到：</p> 
    <ul> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL任务]</li> 
     <li>[！UICONTROL用户]</li> 
     <li>[！UICONTROL公司]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL文档]</li> 
     <li>[！UICONTROL费用]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程序]</li> 
     <li>[！UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义数据类型]</td> 
   <td>用于指定[！UICONTROL自定义数据]字段是作为文本、日期、数字还是货币存储在数据库中的选项。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义显示类型]</td> 
   <td>自定义字段的字段显示类型。 示例包括[！UICONTROL下拉列表]、[！UICONTROL文本字段]、[！UICONTROL文本区域]、[！UICONTROL单选按钮]等。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义字段]</td> 
   <td>对于允许用户从多个选项中选择的自定义数据，这些是用户可以从中进行选择的值。 自定义选项仅在[！UICONTROL下拉列表]、[！UICONTROL多选下拉列表]、[！UICONTROL单选按钮]和[！UICONTROL复选框]中有效。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义表单标签]</td> 
   <td>使用带有自定义选项的自定义显示类型时，这是将在下拉菜单、复选框或该自定义选项的单选按钮中显示的用户界面文本。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义值]</td> 
   <td>将自定义字段与自定义选项一起使用时，该值将存储在数据库中供特定选项使用。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL自定义视图]</td> 
   <td>为列表中的每个对象显示的数据字段或列的定义。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL客户]</td> 
   <td>使用Workfront实例的组织。</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL功能板]</td> 
   <td> <p> 您可以将此字段添加到报表或报表对象列表，以显示报表在列表中列出的仪表板。 </p> <p> 您还可以使用此字段筛选特定功能板上列出的报表。 </p> <p> 有关在报表对象报表中包括仪表板信息的更多信息，请参阅文章中的“了解在仪表板中列出了哪些报表”部分 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">访问和组织报告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL数据类型]</td> 
   <td>请参阅“[！UICONTROL自定义数据类型]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL延迟天数]</td> 
   <td> <p>如果缺少[！UICONTROL实际完成日期]，则此字段显示[！UICONTROL规划开始]和[！UICONTROL今天]之间的日期差异。</p> <p>此外，还显示了当存在[！UICONTROL实际完成日期]时，[！UICONTROL实际完成日期]与[！UICONTROL规划完成日期]之间的日期差异。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL默认计划]</td> 
   <td> <p>可自定义的默认工作时数，可分配给组织内的用户和项目。 </p> <p>时间表用于计算分配给用户的任务的计划日期、开始日期和完成日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL可交付结果]</td> 
   <td>项目完成时必须提供的可量化的货物或服务。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL Demand Management]</td> 
   <td>摄取过程的评分和优先顺序。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL部门目标]</td> 
   <td>特定部门特有的目标，侧重于改善该部门内的运营指标。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL依赖关系]</td> 
   <td>两个任务之间的链接，需要先更改一个任务状态，然后另一个任务才能更改状态。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL依赖关系类型]</td> 
   <td> <p>任务与其前置任务之间的计划关系类型。 例如，[！UICONTROL Finish-Start]，它要求第一个任务必须完成，第二个任务才能开始。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">任务相关性类型概览</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文档]</td> 
   <td>任何附加到中对象的文件 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文档版本]</td> 
   <td> <p>每次将同一文档上载到同一对象时，都会为其分配一个版本号。 用户可以查看和更改文档的早期版本的多个选项。</p> <p>有关更多信息，请参阅 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">管理文档版本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL持续时间]</td> 
   <td> <p>为完成任务问题或项目分配的时间窗口（由[！UICONTROL规划开始]与规划完成之间的天数确定）。</p> 
    <ul> 
     <li>对于任务，如果任务的持续时间类型不简单，则持续时间为可编辑字段。 如果任务的工期类型为“简单”，或者如果任务约束为“固定日期”，则工期是由Workfront执行的计算。</li> 
     <li>对于问题，“持续时间”始终是一个可编辑的字段，它应表示需要解决该问题的预计天数。</li> 
     <li>对于项目，“持续时间”是按以下方式执行的计算 [!DNL Workfront] 它还表示最早任务的规划开始与项目中最新任务的[！UICONTROL规划完成]之间的天数差。</li> 
    </ul> <p>有关任务的[！UICONTROL持续时间]与[！UICONTROL计划持续时间]之间差异的更多信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">[！UICONTROL计划持续时间]与任务的[！UICONTROL持续时间]之间的差异</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL持续时间（分钟）]</td> 
   <td>此字段显示的信息与[！UICONTROL Duration]字段的信息相同（以分钟为单位，而不是以天为单位）。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL每次发生的持续时间]</td> 
   <td> <p>显示在周期性任务父级的[！UICONTROL任务详细信息]和[！UICONTROL编辑任务]框中。 它显示每个周期性任务的持续时间。 有关创建周期性任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建周期性任务</a>. </p> <p> <span>在单个周期性任务中修改的持续时间不显示此字段中指示的值。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL持续时间类型]</td> 
   <td> <p>一个任务字段，指明完成任务所需的工作如何在整个任务持续时间中分配给被分配人。 它表示任务的[！UICONTROL持续时间]、[！UICONTROL所需工作]与分配资源应花费在任务完成上的时间量（即[！UICONTROL分配]）之间的关系。 </p> <p>此字段显示在任务的[！UICONTROL详细信息]选项卡上。 </p> <p>选项包括：</p> 
    <ul> 
     <li>[！UICONTROL计算赋值]</li> 
     <li>[！UICONTROL计算工作量]</li> 
     <li>[！UICONTROL投入比导向]</li> 
     <li>[！UICONTROL Simple]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[！UICONTROL工期]和[！UICONTROL工期类型]概述</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[！UICONTROL持续时间单位]</td> 
   <td>功率搜索中用于测量时间的单位。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL投入比导向]</td> 
   <td>用户数量与任务完成时间之间的关系。 当添加更多用户时，为任务完成安排的总时间会减少，但任务的持续时间保持不变。 例如，如果一项任务正在炮制一桶花生，则添加更多人会缩短计划时间，但以人 — 日为单位的持续时间将保持不变。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL占用时间]</td> 
   <td> <p>[！UICONTROL占用时间]是任务的[！UICONTROL持续时间]的时间单位。 它是包含假日、周末和休息时间的任务的[！UICONTROL计划开始日期]到[！UICONTROL计划完成日期]之间的时间。 换言之，经过的时间就是日历天的流逝。 </p> <p>[!DNL Workfront] 支持以下任务持续时间的占用时间单位：</p> 
    <ul> 
     <li> <p>[！UICONTROL占用分钟数]</p> </li> 
     <li> <p>[！UICONTROL占用小时数]</p> </li> 
     <li> <p>[！UICONTROL占用天数]</p> </li> 
     <li> <p>[！UICONTROL占用周数]</p> </li> 
     <li> <p>[！UICONTROL占用月数]</p> </li> 
    </ul> <p>有关任务持续时间（包括占用时间）的详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[！UICONTROL工期]和[！UICONTROL工期类型]概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL结束日期]</td> 
   <td> <p> 在[！UICONTROL费率]报表中，这是项目级别工作角色的新计费率结束的日期。 在此日期之前与项目关联的小时数乘以该记帐费率来计算项目收入。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL参与度]</td> 
   <td>[！UICONTROL工作绩效指标] (WPI)，指示对任务、项目、团队或组织的承诺和信念何时减弱。 这表明，您需要采取行动，恢复这一信念和承诺。 WPI的衡量标准是问一个简单的问题：“您是否了解对您有何期望？ 您分配到的工作对该组织是否有影响？ 你干得好吗？”</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL企业目标]</td> 
   <td>有助于实现公司目标指标的跨职能目标。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件]</td> 
   <td>项目或任务中的任何更改。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件处理程序]</td> 
   <td>发生事件时发生的自动任务。 一个常见示例是自动电子邮件通知。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL事件通知]</td> 
   <td>从事件处理程序生成的电子邮件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL费用]</td> 
   <td>任务或项目的非劳力成本。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL External]</td> 
   <td> <p>通常为许可证类型或具有此类许可证的用户，此类用户只能查看系统中的信息。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL外部系统]</td> 
   <td>在指定的记录系统之外存储和管理的任何服务或软件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL筛选器]</td> 
   <td> <p>定义屏幕上显示的信息的报告或列表元素的主要构建块之一。 有关报表元素的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报表元素：筛选器、视图和分组</a>.</p> <p>该过滤器可确定在报告中或页面上显示的结果 [!DNL Workfront] 面板列表，如项目、任务或问题。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL Financial Work Management]</td> 
   <td>在中管理人工成本、费用和收入数据的流程 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL固定成本]</td> 
   <td>您可以为项目定义固定成本额。 这是项目的[！UICONTROL计划成本]的一部分，它表示完成项目所需的金额。 有关成本的信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL固定收入]</td> 
   <td>您可以为项目定义固定收入额。 这是项目的[！UICONTROL计划收入]的一部分，它表示在完成项目时可能获得的金额。 有关收入的信息，请参见 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL标志]</td> 
   <td> <p> 该字段与[！UICONTROL状态图标]的字段相同，但它仅适用于以下视图： </p> 
    <ul> 
     <li> [！UICONTROL模板] </li> 
     <li> [！UICONTROL费用] </li> 
    </ul> <p> 有关更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹]</td> 
   <td>文件夹用于组织与对象关联的文档或报告。</td> </tr>
  <tr>
  <td>[！UICONTROL FTE]（相当于全职）</td> 
   <td>这是相当于全职的时间，指示资源可用于工作的时间。 
   [！UICONTROL FTE]字段显示在以下区域中： 
  <ul>
   <li> 用户配置文件，在编辑或创建用户时 </li>
   <li> [！UICONTROL资源规划者] </li>
   <li> [！UICONTROL Scenario Planner](需要Workfront Scenario Planner的附加许可证) </li>
   <li> 用户列表和报告 </li> </ul>

<p>[！UICONTROL FTE]必须是最多为1的小数，并且不能为0。 </p>
   <p> [！UICONTROL FTE]为1（这是用户的[！UICONTROL FTE]字段的默认值，如其配置文件中所定义）表示资源（用户或角色）根据计算其可用性的计划工作整个小时数。 </p>
   <p>由您的Workfront管理员决定在确定用户可用性时使用的计划。  </p>
   <ul>
   <li> 当使用[！UICONTROL默认计划]时，Workfront会使用在其配置文件中找到的用户的[！UICONTROL FTE]来计算可用性。 </li>
   <li> 使用用户的计划时，Workfront将使用用户的休息时间、[！UICONTROL工作时间]值和[！UICONTROL默认计划]的小时数来计算用户的[！UICONTROL FTE]。 </li> </ul>

<p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.  </p>
   <p>有关在中创建计划的详细信息 [!DNL Workfront]，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>. </p>

<p><b>注释</b></p>
   <p>对于[！UICONTROL Scenario Planner]中的所有计算，Workfront使用以下值： 1 [！UICONTROL FTE] = 8小时。</p>
   <p>有关更多信息，请参阅 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">[！UICONTROL Scenario Planner]入门</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL甘特图]</td> 
   <td> <p>日历视图中项目日期的可视时间线，基于当前计划的项目任务中的计划或预计日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目标]</td> 
   <td><p>中的目标有两个概念 [!DNL Workfront]： </p> 
    <ul> 
     <li> <p><b>项目目标</b>：项目相关利益相关者同意的一组业务目标。 项目目标属于项目的业务案例。 </p> <p>您无法在列表或报告中显示项目目标，但可以通过API访问它们。 </p> <p>有关业务案例项目目标的信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">创建业务案例目标 </a>. </p> </li> 
     <li> <p><b>战略目标</b>：策略目标是指您创建的一个目标，用于规划特定时间段的工作策略。 您可以使用创建这些类型的目标 [!DNL Workfront Goals]. 您的组织必须购买额外的许可证，并且您必须拥有此功能的访问权限，才能创建战略目标。 [!DNL Workfront Goals] 仅在获得额外许可证后才能使用。</p> 
     <p>有关更多信息，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </p> 
     <p>您可以在目标或项目报告中显示战略目标，并通过API访问它们。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目标层次结构]</td> 
   <td> <p>在[！UICONTROL目标]和[！UICONTROL项目]报表中，这是一个收集字段，当战略目标与其他目标对齐时，该字段会在层次结构中显示战略目标所属的目标。 目标由▸分界符分隔。 </p> <p>只有目标和目标的父级会显示在此字段中。 子目标不显示。 </p> <p>有关在中对齐目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">中的目标对齐概述 [!DNL Workfront Goals]</a>. </p> 
   <p>仅当您的组织购买了 [!DNL Workfront Goals]. 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL目标成功分数]</td> 
   <td> 在[！UICONTROL项目报告]中，此字段用于引用与[！UICONTROL业务]案例相关的项目级目标。 目前，这是一个已弃用的字段，与任何功能都无关联。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL目标] </td> 
   <td> <p>在[！UICONTROL项目]报表中，这是一个收集字段，它显示与项目关联的所有战略目标。 目标用逗号分隔。</p> <p>仅当您的组织购买了 [!DNL Workfront Goals]. 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. 有关中的战略目标和项目目标的更多信息 [!DNL Workfront]，请参阅本文中的“[！UICONTROL目标]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL全局界面首选项]</td> 
   <td>影响所有用户的界面设置。 [！UICONTROL全局界面首选项]可被[！UICONTROL用户界面首选项]覆盖。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL组]</td> 
   <td> <p>有权访问相同对象的用户（可能来自同一部门或业务部门）的集合。 除了用户之外，组还可以与项目组合、项目群、项目群、<span> 项目模板，</span> 公司、团队、时间表、布局模板和时间表配置文件。</p> <p>您还可以按组向对象授予权限。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">组概述</a>.</p> <p>在下列类型之一的对象列表或报表中，可以使用[！UICONTROL组]字段列出与特定组相关联的该类型对象：用户、项目组合、项目群、 <span>项目模板</span>、公司、团队、计划、布局模板或时间表配置文件。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL组管理员]</td> 
   <td> <p>管理指定用户组的对象、访问权限和用户的用户。</p> <p> 在[！UICONTROL组]报表中，此字段显示组中指定为[！UICONTROL组管理员]的用户名称。 有关组管理员的详细信息，请参见 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>具有管理访问权限的[！UICONTROL组]</td> 
   <td> <p> 在[！UICONTROL布局模板]、[！UICONTROL时间表配置文件]或[！UICONTROL计划报告]中，此字段显示组管理员有权修改模板的组。 您还可以按此字段筛选此报告。 </p> <p> 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL分组]</td> 
   <td> <p>用于按通用标准对列表中的信息进行分类的报表元素。</p> <p>有关更多信息，请参阅文章中的“[！UICONTROL分组]”部分 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报表元素：筛选器、视图和分组</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL移交日期]</td> 
   <td> <p>任务可供工作的日期。 [！UICONTROL移交日期]是一个计算日期，无法手动设置。 <br>有关[！UICONTROL移交日期]的更多信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[！UICONTROL任务移交日期]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL技术支持]</td> 
   <td>部分 [!DNL Workfront] 保留所有问题队列的服务器。 [！UICONTROL技术支持]可用于处理客户支持工单、项目请求、技术支持工单等。 此区域与[！UICONTROL Requests]区域相同。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL所有者]</td> 
   <td>在[！UICONTROL小时]报表中，[！UICONTROL所有者]是小时所归因的用户。 这与实际记录时间的用户不同。 这两个实体有时可能是两个不同的用户。 <br>有关记录另一个用户的时间的详细信息，请参阅文章 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">记录时间</a>.</td> 
  </tr>

<tr> 
   <td>小时状态</td> 
   <td> <p>Workfront为任务、问题或项目记录的实际小时数设置的属性。 </p>

小时条目在Workfront中可以具有以下状态之一：
<ul>
   <li><b>已提交</b>：小时数已记录到项目、任务或问题中。 它们是开票记录的一部分，或者尚未添加到开票记录。</li>
   <li><b>已批准</b>：小时数已记录并且已由项目所有者批准。 它们是开票记录的一部分，或者尚未添加到开票记录。</li> 
   <li><b>未批准</b>：小时数已被项目所有者记录并拒绝。 它们是开票记录的一部分，或者尚未添加到开票记录。</li>
   <li><b>已记帐</b>：小时数已记录，已添加到记帐记录，并且记帐记录状态已标记为已记帐。 它们不需要项目所有者的批准。</li>
   <li><b>已记帐和已批准</b>：小时数已被记录、项目所有者批准，并且开票记录状态已标记为已开票。</li>
   </ul>


<p>当小时数是记帐记录的一部分时，小时状态指示小时数是否已批准，或者小时数所属记帐记录是否已记帐。 小时条目的小时状态仅在小时列表或报告中可见。 </p>

<p>有关向开票记录添加小时数的更多信息，请参阅文章中的“向开票记录添加小时数”部分 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >创建开票记录</a>.</p>

<p>有关批准项目时间的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >项目需要批准时间</a>.</p>

<p><b>笔尖</b></p>

<p>未直接在工作项上记录的常规小时数不显示小时状态。 </p> </td> 
  </tr>



<tr> 
   <td>[！UICONTROL小时类型]</td> 
   <td> <p>可以为用户为任务、问题或项目记录的实际小时数设置的属性。 这也是未直接链接到工作的已记录小时数的属性，如[！UICONTROL Vacation]和[！UICONTROL Time Off]。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">管理小时类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL ID]</td> 
   <td> <p>ID是与中的每个对象关联的字母数字指示器 [!DNL Workfront]. 它唯一标识 [!DNL Workfront] 数据库。 您可以查看报表中任何对象的ID或每个对象的列表。 </p> <p>提示：   <p>您还可以在对象页面的URL中查看ID。 例如，当您访问[！UICONTROL项目详细信息]页面时，项目的ID可能类似于以下URL中列出的数字：</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL个人目标]</td> 
   <td>对团队目标的量度有贡献的个人目标，但与个人或职业发展无关。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL继承访问权限]</td> 
   <td>共享函数，允许访问从对象传播到另一个对象。 例如，项目和项目组合记录中定义的项目用户的继承访问权限。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL计划]</td> 
   <td> <p>在 [!DNL Workfront Scenario Planner]，您可以将计划划分为多个计划，以便更轻松地管理计划。 <span>您可以构建[！UICONTROL计划]报表，并可以访问[！UICONTROL项目]报表中的[！UICONTROL计划]信息。</span></p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> <p>此 [!DNL Initiative] 报告在您的 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。 您无法通过API访问[！UICONTROL Initiatives]。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL计划工作角色]</span> </td> 
   <td> <p><span>[！UICONTROL计划工作角色]报告类型显示与计划计划计划相关的工作角色的信息。 [!DNL Workfront Scenario Planner].</span> </p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p><span>此报表类型在中不可见 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL计划工作角色小时数]</span> </td> 
   <td> <p><span> 在[！UICONTROL计划工作角色]报表中，它显示与计划中的工作角色关联的小时数。</span> </p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p>此字段和[！UICONTROL Initiative Job Role]报告类型在您的 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划工作角色计数]</td> 
   <td> <p>在[！UICONTROL计划工作角色]报表中，它显示与计划关联的特定工作角色的数量。</p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p>此字段和[！UICONTROL Initiative Job Role]报告类型在您的 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划上次发布日期]</td> 
   <td> <p>[！UICONTROL Initiative]、[！UICONTROL Initiative Job Role]和[！UICONTROL Project]报表中的一个字段，它显示上次将计划计划计划发布到项目的日期。 您可以发布计划以创建项目或更新链接到计划的项目。</p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> <p><span>有关发布计划的信息，请参阅</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">发布方案以在中创建和更新项目 [!DNL Workfront Scenario Planner]</a>. 此字段在您的中不可见 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL内联搜索]</td> 
   <td>在完成表单的过程中执行的搜索，以查找某个特定字段的可能条目。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL接口设置]</td> 
   <td>应用程序允许定义自定义视图、筛选器、分组、列表控件等的区域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL是公司目标]</p></td> 
   <td> <p>In [!DNL goal reports]，则为每个策略目标显示一个“[！UICONTROL True]/ [！UICONTROL False]”值，以指示您的组织是否已作为所有者分配给目标。 </p> 
   <p>仅当您的组织购买了 [!DNL Workfront Goals]. 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL问题]</td> 
   <td> <p>计划外工作项，通常表示存在妨碍完成任务或项目的问题。 它会进行测试和评估，以便进一步考虑工作量</p> <p>[！UICONTROL问题]也可以是[！UICONTROL技术支持]请求。 [！UICONTROL更改单]、[！UICONTROL请求]和[！UICONTROL错误]也是[！UICONTROL问题]。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL问题管理]</td> 
   <td> <p>管理问题类型定义的流程和规则，以及与每种类型关联的路由、分类或流量流程。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL问题所有者]</td> 
   <td>负责分类和完成问题的团队或用户。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL迭代]</td> 
   <td>团队生成一组预定义交付项的时间段。</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL工作角色]</td> 
   <td> <p>用于标识用户的日常工作职能和职责。 可以将工作角色分配给工作项，以确定完成工作流程所需的技能，而无需将其分配给特定用户。 </p> <p>一个用户可以有多个角色。 示例包括图形设计器或顾问。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL日志条目]</p> </td> 
   <td> <p>一个可报告对象，可为项目、任务、问题和其他对象的[！UICONTROL更新]区域中所显示的跟踪字段说明系统更新信息。</p> <p>要了解更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[！UICONTROL更新]区域报告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Kanban标志]</td> 
   <td> <p>在[！UICONTROL Task]报告或[！UICONTROL Issue]报告中，[！UICONTROL Kanban Flag]字段显示在[！UICONTROL Kanban Board]上的文章中设置的标志状态。 可能的值包括[！UICONTROL On Track]、[！UICONTROL Ready To Pull]和[！UICONTROL Is Blocked]。</p> <p>有关在[！UICONTROL Kanban故事板上的故事上设置标记状态的更多信息，请参阅文章 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">对[！UICONTROL Kanban展示板上的故事使用标记</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>可衡量的价值，表明公司在多大程度上有效地实现了关键业务目标。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL滞后]</td> 
   <td>前置任务的[！UICONTROL规划完成日期]之后必须经过的时间，直到相关任务可以开始。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL滞后类型]</td> 
   <td> <p>[！UICONTROL滞后时间]的计算方法。 它可以是：</p> 
    <ul> 
     <li>[！UICONTROL天数]（工作日）</li> 
     <li>[！UICONTROL日历日]（忽略假日）</li> 
     <li>[！UICONTROL百分比]</li> 
     <li>[！UICONTROL每周日期]</li> 
    </ul> <p>有关更多信息，请参阅中的“[！UICONTROL滞后类型概述]”部分 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">滞后类型概述</a></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL大缩略图]</td> 
   <td> <p> 在[！UICONTROL Document]列表或报表中，它以缩略图显示文档的预览。 </p> <p>选择 <strong>[！UICONTROL大缩略图]</strong> 查看报表中400像素范围的缩略图。</p> <p>当您修改列表或报表中的列宽时，缩略图的大小会进行调整。</p> <p>另请参阅本文中的“[！UICONTROL缩略图]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最近10位查看者]</td> 
   <td> <p>在报表列表中，此字段显示最近查看过报表的最多10个用户的名称。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次条件注释]</td> 
   <td> <p>此字段显示对象所有者上次在对象上输入的更新。这是所有者最近对对象执行的活动或交互。</p> <p>此 [!DNL Last Condition Note] 如果删除了某个对象的最后一个注释的注释文本，则该列为空。 在对象上输入新注解后，它将变成最后一个注解，并再次显示在列中。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次财务更新日期]</td> 
   <td>在[！UICONTROL项目]报表中，此字段捕获上次计算和更新项目财务的日期和时间。 有关项目财务的信息，请参见 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">项目财务概述</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上一注释]</td> 
   <td> <p>此字段显示任何用户上次在对象上输入的更新。 这是对象上的最新活动或交互。</p> <p>如果对象的最后一个注释的文本已被删除，[！UICONTROL Last Note]列为空。 在对象上输入新注解后，它将变成最后一个注解，并再次显示在列中。</p>
   <p>将此字段添加到[！UICONTROL任务]报告时，子对象上剩余的任何更新 — 如问题、子任务、文档等。  — 不显示在此列中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次查看者]</td> 
   <td> <p>在报告列表中，此字段显示有关上次查看报告的用户的信息。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上次查看日期]</td> 
   <td> <p>在报告列表中，此字段显示上次显示报告的日期。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL布局模板]</td> 
   <td>由系统管理员或组管理员定义，用于标识在给定用户的工作区中显示的选项卡和报告。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL布局类型]</td> 
   <td>结合[！UICONTROL自定义视图]，[！UICONTROL布局类型]指定[！UICONTROL自定义视图]的类型。 目前，仅列表可用。 将来，[！UICONTROL详细信息]（对象的[！UICONTROL详细信息]视图）可能会变得可用。</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL库任务]</td> 
   <td>单个任务的模板，用于为整个应用程序中的[！UICONTROL任务]和[！UICONTROL模板任务]提供一致的命名。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL许可证类型]</td> 
   <td>分配给[！UICONTROL访问级别]的许可证类型。 它是[！UICONTROL Full User]、[！UICONTROL Limited User]或[！UICONTROL Requester]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL许可证限制计划]</td> 
   <td> <p>在[！UICONTROL组]视图或报表中，此字段显示可分配给用户的最大[！UICONTROL计划]许可证数，这些用户具有指定为其[！UICONTROL主组]的相应组。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL许可证限制工作]</td> 
   <td> <p>在[！UICONTROL组]视图或报表中，此字段显示可分配给用户的最大[！UICONTROL工作]许可证数，这些用户具有指定为其[！UICONTROL主组]的相应组。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL受限用户]</td> 
   <td>允许创建 [!DNL Access Level] 包含仅查看权限，能够提交问题、输入注释和上传文档。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL列表控件]</td> 
   <td> <p>[！UICONTROL界面设置]的一部分，允许将自定义筛选器、视图和分组链接到单个用户或全局链接到所有用户。</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL手册]</td> 
   <td> <p>[！UICONTROL项目]的[！UICONTROL更新类型]之一。 此设置允许仅在单击“[！UICONTROL重新计算的时间线]”时更新[！UICONTROL项目预计]和[！UICONTROL已计划]的时间线。 在轻微重新计算过程中以及更新项目中的项目或任务时，将忽略通过此方式设置的项目。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目[！UICONTROL更新类型] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL我]</td> 
   <td> <p>指当前登录的用户。 </p> <p>我们建议在筛选器中使用此字段，以使报告在与其他用户共享时更加通用。 这样，您只能构建一个报告，该报告将根据查看信息的登录者显示不同的信息，因为始终为登录用户自定义信息。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL最大用户数]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与以下功能相关 [!DNL Workfront] 已删除，无法更新字段。 </p> <p>在早期版本中 [!DNL Workfront]中，您可以在创建或编辑工作角色时更新此字段。 它显示可与每个项目中的角色相关联的用户总数。 值为零，表示可在项目上分配无限数量的用户。 </p>字段在一些报告和列表中仍然可见，但显示的信息无法更新。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL里程碑]</td> 
   <td> <p>与任务关联的标记，用于指示任务完成时已实现项目中的关键点。 您通常可以使用里程碑来显示重要事件，例如项目某个阶段的完成或一组关键活动。 [！UICONTROL里程碑]通常与父任务相关联。 必须先创建里程碑，然后才能将其附加到任务。 有关里程碑的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">创建里程碑路径</a> 和 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">将里程碑与任务关联</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL里程碑路径]</td> 
   <td>[！UICONTROL里程碑]的集合。 [！UICONTROL里程碑路径]用于项目，以将具有特定类型的[！UICONTROL里程碑]的项目与具有一组不同的[！UICONTROL里程碑]的项目区分开。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL里程碑任务]</td> 
   <td>标记以指示要测量的可报告事件的任务。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL模块]</td> 
   <td>中的方案中的单个步骤 [!DNL Workfront Fusion] 会根据关联的应用程序执行某些功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL My Primary Role]</td> 
   <td> <p>当在筛选条件中引用此选项时，将显示与登录用户具有相同[！UICONTROL主角色]的用户，或分配给登录用户的[！UICONTROL主角色]的工作项。</p> <p>我们建议在筛选器中使用此字段，以使报告在与其他用户共享时更加通用。 这样，您只能构建一个报告，该报告将根据查看信息的登录者显示不同的信息，因为始终为登录用户自定义信息。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL My Home Team]</td> 
   <td> <p>当在筛选器中引用此字段时，此字段显示属于登录用户的[！UICONTROL主团队]的用户，或分配给登录用户的[！UICONTROL主团队]的工作项。 </p> <p>我们建议在筛选器中使用此字段，以使报告在与其他用户共享时更加通用。 这样，您只能构建一个报告，该报告将根据查看信息的登录者显示不同的信息，因为始终为登录用户自定义信息。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL命名约定]</td> 
   <td>组织范围的一组规则，使用数据创建项目、任务和交付项的名称。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL本机集成]</td> 
   <td>无需手动编码或API配置的集成。 也称为“开箱即用”集成。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL导航菜单]</td> 
   <td>应用程序的顶部中央面板，其中包含指向[！UICONTROL Workfront]主区域的链接。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[！UICONTROL新数值]</td> 
   <td>在[！UICONTROL Journal Entry]报表中，这将显示替换[！UICONTROL旧数字值]的字段的更新值。
   有关更多信息，请参阅本文中的“[！UICONTROL旧数字值]”。</td> 
  </tr>
  <tr> 
   <td>[！UICONTROL非工作日]</td> 
   <td>未分配给完成任何分配的日期。 这通常是假日、假期或周末。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL注释]</td> 
   <td>对所做的评论或更新 [!DNL Workfront] 对象。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL注释文本]</td> 
   <td> <p>这会显示用户在任何对象上输入的更新文本。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL链接目标的数量]</td> 
   <td> <p>在[！UICONTROL项目]报表中，这是与项目关联的策略目标的数量。 有关将项目与战略目标关联的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">将项目添加到中的目标  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>有关战略目标的信息，另请参阅本文中的“[！UICONTROL目标]”。</p> 
   <p>仅当您的组织购买了 [!DNL Workfront Goals]. 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">将项目添加到[！UICONTROL Adobe Workfront目标]中的目标</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL对象]</td> 
   <td> <p>组织的工作项和报告，以及在[！UICONTROL Workfront]中管理这些工作项和报告的用户组。 对象可以是：</p> 
    <ul> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程序]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL任务]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL文档]</li> 
     <li>[！UICONTROL功能板]</li> 
     <li>[！UICONTROL报表]</li> 
     <li>[！UICONTROL组]</li> 
     <li>[！UICONTROL团队]</li> 
     <li>[！UICONTROL用户]</li> 
     <li>[！UICONTROL公司]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解[！UICONTROL Adobe Workfront]中的对象</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL对象类型]</td> 
   <td>如果创建包含所有自定义表单的报表或列表，可将此字段用作视图或过滤器，以查看与每个表单关联的对象类型。 </td> 
  </tr> 
 <tr> 
   <td>[！UICONTROL旧数值]</td> 
   <td>在[！UICONTROL Journal Entry]报表中，这会显示字段在更新前的原始值。 字段值更新后，将在[！UICONTROL Journal Entry]报表中显示为[！UICONTROL New Number Value]。 有关更多信息，另请参阅“[！UICONTROL新数值]”。</td> 
  </tr>
  <tr> 
   <td>[！UICONTROL On Change Only]</td> 
   <td> <p>[！UICONTROL项目更新]类型之一。 如果选择此项，则[！UICONTROL项目预计]和[！UICONTROL已计划]时间表仅在更新或更改项目或项目中的任务时更新。 它不会每晚更新项目。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL操作任务]</td> 
   <td> <p>中的[！UICONTROL Issue]名称 [!DNL Workfront] 数据库，用于文本模式报表或计算的自定义数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL打开]</td> 
   <td>未完成但正在处理的问题或任务。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL组织结构图]</td> 
   <td>组织结构图的简称。 这是一个显示组织层次结构的图表。 它还位于[！UICONTROL用户]详细信息屏幕上的选项卡上，该屏幕显示并允许设置[！UICONTROL用户]的[！UICONTROL公司]和[！UICONTROL报表]关系。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL组织设置]</td> 
   <td>这会为您的组织定义[！UICONTROL公司]、[！UICONTROL组]和[！UICONTROL安全配置文件]。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL其他组]</td> 
   <td> <p>在列出用户的报表或视图中，此字段显示每个用户所属的所有组。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL替代货币]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]报表中，这是与工作角色关联的货币。 它是由[！UICONTROL设置]区域建立的[！UICONTROL基本货币]的覆盖 [!DNL Workfront] 管理员。 </p> 
     <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL覆盖货币计费/小时]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]报表中，这是使用所选工作角色的[！UICONTROL覆盖货币]的工作角色的每小时记帐费率。</p> 
     <p> 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL覆盖货币成本/小时]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL工作角色]报表中，这是工作角色使用所选工作角色的[！UICONTROL覆盖货币]每小时成本费率。 </p> 
     <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理职位角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL所有者]</td> 
   <td>负责完成指定对象的用户。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL所有者类型]</span> </td> 
   <td> 
    <div> 
     <p>在[！UICONTROL目标]报表中，这会显示分配给策略目标的所有者类型。 以下是目标所有者类型：</p> 
     <ul> 
      <li> <p>[！UICONTROL用户]</p> </li> 
      <li> <p>[！UICONTROL团队] </p> </li> 
      <li> <p>[！UICONTROL组]</p> </li> 
     </ul> 
     <p>当目标所有者是您的组织时，此字段中未显示任何值。 </p> 
     <p>这需要额外的许可证。 有关信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概述</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL参数]</td> 
   <td> <p>[！UICONTROL参数]是一个自定义字段。 您可以为系统中的所有参数或自定义字段构建报告。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Parent]</td> 
   <td>在报表中，此字段显示有关对象父项的信息。 例如，在[！UICONTROL问题]报告中，它可能会显示问题登录所属的任务或项目的信息；在任务报告中，它可能会显示有关直接父级任务或项目的信息。 有关哪些对象中可能有父对象的详细信息 [!DNL Workfront]，请参阅文章中的“对象的相互依赖性和层次结构”部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解中的对象 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父级滞后时间]</td> 
   <td>从[！UICONTROL父任务]开始到[！UICONTROL子任务]开始必须经过的时间。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL父任务]</td> 
   <td>也称为[！UICONTROL摘要任务]。 此任务具有子任务（也称为[！UICONTROL子任务]）。 父任务的[！UICONTROL持续时间]、[！UICONTROL所需工时]和[！UICONTROL完成百分比]是根据子任务计算的。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL兼职资源]</td> 
   <td>容量小于系统中定义的默认计划的授权用户。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL完成百分比]</td> 
   <td> <p>项目、任务或问题字段，显示与任务、项目或问题关联的工作的完成百分比。</p> <p>您可以为问题和工作任务手动更新此字段。 </p> <p>对于项目和父任务，此字段是从所有工作任务汇总而来，您无法手动更新。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">项目[！UICONTROL完成百分比]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL权限]</td> 
   <td> <p>授予用户对某个对象的权限，通常是为了让用户可以完成对该项目的工作或查看该项目而授予这些权限。 您可以将权限授予：</p> 
    <ul> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL任务]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROLPortfolio]</li> 
     <li>[！UICONTROL程序]</li> 
     <li>[！UICONTROL报表]</li> 
     <li>[！UICONTROL功能板]</li> 
     <li>[！UICONTROL文档]</li> 
     <li>[！UICONTROL自定义Forms]</li> 
     <li>[！UICONTROL视图]</li> 
     <li>[！UICONTROL筛选器]</li> 
     <li>[！UICONTROL分组]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划]</td> 
   <td> <p>这是中的完整许可证类型 [!DNL Workfront] 系统。 用户必须拥有此项才能访问中的所有功能 [!DNL Workfront].</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划](在 [!DNL Scenario Planner])</td> 
   <td> <p>使用时，计划是主要对象 [!DNL Workfront] 场景规划器。 您可以概述公司的近期和长期未来战略，确定每个高级别成果并将其作为计划添加到 [!DNL Workfront] 场景规划器。 </p> <p>无法显示 [!DNL Scenario Planner] 计划，但无法通过 [!DNL Workfront] API。 </p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划]</td> 
   <td> <p>某些内容计划发生的时间范围。 在中创建项目、任务或问题时 [!DNL Workfront]，即可确定计划的开始和结束日期，以及开始和结束日期的计划时间范围。 这些值表示您最初的意图或完成项目所需时间的估计。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划收益]</td> 
   <td>这是一个手动输入项，供项目经理评估完成一个项目是否会给组织带来任何经济利益。 指定此值可包含在为项目组合[！UICONTROL业务案例]中。 您必须对项目具有[！UICONTROL管理]权限才能更新此值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL计划预算小时数]</td> 
   <td> <p>在[！UICONTROL预算小时数]报表中，显示在[！UICONTROL资源规划者]中为项目或[！UICONTROL工作角色]预算的小时数。 </p> <p>有关在[！UICONTROL资源规划者]中预算项目或角色的信息，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">使用[！UICONTROL项目]和[！UICONTROL角色]视图的[！UICONTROL资源规划者]中的预算资源</a>. 有关[！UICONTROL预算小时数]报表的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">报告：预算小时</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划完成日期]</td> 
   <td> <p>您可以手动将[！UICONTROL规划完成日期]设置为您选择的日期。 如果不设置[！UICONTROL规划完成日期]， [!DNL Workfront] 自动设置。 自动设置后，[！UICONTROL计划完成日期]为：[！UICONTROL计划开始日期] + [！UICONTROL持续时间]</p> <p>有关更多信息，请参阅以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务概述[！UICONTROL计划完成日期]</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">设置项目[！UICONTROL计划完成日期]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划成本]</td> 
   <td> <p>项目的[！UICONTROL计划劳力成本]和[！UICONTROL计划费用成本]的总和。 这不包括项目中的[！UICONTROL计划风险成本]。  </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划持续时间]</td> 
   <td> <p>任务的[！UICONTROL计划持续时间]通常与任务的[！UICONTROL持续时间]相同。 它表示任务的[！UICONTROL规划开始]与[！UICONTROL规划完成日期]之间的天数差。 </p> <p>当任务的[！UICONTROL工期]类型为[！UICONTROL投入比导向]时，根据分配给该任务的资源数量，[！UICONTROL计划工期]可能与任务的[！UICONTROL工期]不同。 </p> <p>例如，如果[！UICONTROL工期]类型为[！UICONTROL投入比导向]的任务的[！UICONTROL工期]为3天，并且您为该任务分配了一个具有完整时间计划的资源，则[！UICONTROL计划工期]也为3天。 如果将具有完整时间计划的三个资源分配给同一任务，则[！UICONTROL持续时间]将保留3天，而[！UICONTROL计划持续时间]将变为1天。 [！UICONTROL计划持续时间]还更改任务的[！UICONTROL计划开始]和[！UICONTROL计划完成]日期，以反映新的[！UICONTROL计划持续时间]。 因此，项目的时间表也受到影响。 </p> <p>有关任务的[！UICONTROL持续时间]与[！UICONTROL计划持续时间]之间差异的更多信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">[！UICONTROL计划持续时间]与任务的[！UICONTROL持续时间]之间的差异</a>.</p> <p>项目和问题没有[！UICONTROL计划持续时间]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划持续时间分钟]</td> 
   <td> <p>项目或问题的[！UICONTROL计划持续时间分钟]是以分钟为单位的项目或问题的[！UICONTROL持续时间]。 </p> <p>任务没有[！UICONTROL计划持续时间分钟]字段。 </p> <p>[！UICONTROL模板任务]有一个[！UICONTROL计划持续时间分钟]字段，该字段以分钟为单位显示任务的[！UICONTROL计划持续时间]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划费用成本]</td> 
   <td> <p>为项目或任务记录的所有费用的[！UICONTROL计划金额]的总和。</p> <p><b>示例</b></p>
   <p>如果您为任务1创建费用并在[！UICONTROL计划金额]字段中输入$600.00，则此任务的[！UICONTROL计划费用成本]为$600.00。 </p> 
   <p>对于项目， [!DNL Workfront] 使用以下公式计算[！UICONTROL计划费用成本]：</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划小时数]</td> 
   <td> <p>此字段显示在[！UICONTROL项目]、[！UICONTROL任务]和问题区域、项目、任务或问题的报告以及资源管理工具中，如[！UICONTROL资源规划器]、[！UICONTROL工作负载均衡器]和[！UICONTROL利用率]报告。 </p> <p>它显示项目所有者预计完成每个任务或问题所需的小时数。 对于项目，它通常是项目任务中[！UICONTROL计划小时数]的汇总。 </p> <p>根据您查看信息的位置，[！UICONTROL规划小时数]字段可能会显示不同的信息。 有关计划小时数的信息，请参见 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划小时数概述</a>.</p> <p>计划小时数以分钟为单位存储在 [!DNL Workfront] 数据库。 使用此字段编写计算时，请确保将小时数显示为分钟这一事实考虑在内。<br></p> <p>默认情况下，计划小时数平均分配给工作项持续时间内的所有天，对于分配给任务的所有资源也是如此。 用户可以更新工作项的每日计划小时数或每个被分配人的单个计划小时数。</p> <p>项目、任务和问题的此字段更新有所不同： </p> 
    <ul> 
     <li> <p>对于问题，您可以手动更新此字段。 问题已计划小时数未添加到项目已计划小时数。 </p> <p>提示：在问题报告中，[！UICONTROL已计划小时数]字段之一已替换为[！UICONTROL工作]字段。 字段显示问题的已计划小时数。 有关更多信息，请参阅此表中的“工作”或“[！UICONTROL工作]”字段。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>对于任务，当任务的[！UICONTROL持续时间类型]为[！UICONTROL计算的工作分配]或[！UICONTROL简单]时，您可以手动更新此字段。 此字段的计算方式 [!DNL Workfront] 当任务的[！UICONTROL持续时间类型]为[！UICONTROL计算的工作量]或[！UICONTROL投入比驱动]时。<br>有关[！UICONTROL任务持续时间]的信息，请参阅文章 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[！UICONTROL工期]和[！UICONTROL工期类型]概述</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>对于项目， [!DNL Workfront] 通过添加项目中所有任务的所有已计划小时数来计算已计划小时数。 </p> </li> 
    </ul> <p><b>笔尖</b></p> <p>此外，您还可以通过使用文本模式并引用其他字段，在[！UICONTROL项目]、[！UICONTROL任务]或[！UICONTROL问题]报表中显示[！UICONTROL已计划小时数]。 有关更多信息，请参阅“<code>work</code>“”、“[！UICONTROL Work]”和“”<code>workRequiredExpression</code>”字段。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划劳力成本]</td> 
   <td> 
    <p>对于任务，用户或角色的每小时费率乘以分配给用户或角色的小时数。</p> <p>对于项目，它是所有任务的所有[！UICONTROL计划劳力成本]的总和。</p> <p>是否使用用户或角色的费率取决于为给定任务选择的成本类型。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划收入]</td> 
   <td> <p>任务和项目可以在中显示[！UICONTROL计划收入]的值 [!DNL Workfront]. [！UICONTROL计划收入]表示与项目中的任务的[！UICONTROL计划小时数]关联的资金量。 对于项目，它还可以包含项目的[！UICONTROL固定收入]。 </p> <p>对于任务，这是与任务的[！UICONTROL已计划小时数]关联的收入。 所有任务的计划小时数累计到项目的计划小时数，有助于计算项目[！UICONTROL计划小时数]。 </p> 
   <p>[!DNL Workfront] 使用以下公式为任务和项目计算[！UICONTROL计划收入]：</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>显示在[！UICONTROL项目详细信息]区域和项目报表中的项目[！UICONTROL计划收入]与[！UICONTROL利用率]报表中显示的计划收入不同。 </p> <p>[！UICONTROL项目详细信息]区域中的[！UICONTROL计划收入]反映了任务收入以及项目的固定收入。 [！UICONTROL利用率报告]中的[！UICONTROL计划收入]仅显示与项目中的任务关联的[！UICONTROL计划收入]。 </p> 
     <p><b>示例</b></p>  
      <p>如果项目具有1个时长10小时的任务，分配给一名顾问，每小时费率为$20，并且项目有$100 [！UICONTROL固定收入]，则[！UICONTROL利用率]报表显示$200 [！UICONTROL计划收入]（与任务小时数关联的[！UICONTROL计划收入]）。 [！UICONTROL项目详细信息]部分显示$300（来自任务的[！UICONTROL计划收入]和项目的固定收入）。 </p> 
    <p>有关在中跟踪收入的信息 [!DNL Workfront] 参见 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">开单和收入概览</a>. </p> 
    <p>有关[！UICONTROL利用率报表]中[！UICONTROL计划收入]计算的信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看资源利用率信息 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划风险成本]</td> 
   <td> <p>项目上所有风险的[！UICONTROL潜在成本]的总和，考虑其发生概率。 此金额不包括在项目的[！UICONTROL计划成本中。</p> <p>项目的[！UICONTROL计划风险成本]按以下公式计算：</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL门户配置文件]</td> 
   <td>管理员定义的选项卡和门户部分集合，该集合显示在 [!DNL Workfront] 应用程序[！UICONTROL主页]和其他仪表板。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL门户分区]</td> 
   <td>功能板或门户页面上选项卡的一个组件。 通常是单个报告、图表、日历或关键信息列表。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL门户选项卡]</td> 
   <td>门户或功能板上的选项卡，最多包含三个门户部分。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROLPortfolio]</td> 
   <td> <p>具有统一特性的项目集合。 这些项目通常会争夺相同的资源、预算或时限。 您可以将Portfolio划分为项目群，并在将项目添加到Portfolio之前将其与项目群关联。</p> <p>有关项目组合的详细信息，请参阅 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">中的Portfolio概述 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio管理]</td> 
   <td>一个实践领域，侧重于管理收藏集或相关方案和项目工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio优化器]</td> 
   <td>A [!DNL Workfront] 工具，以帮助评估项目组合中的项目并确定其优先次序。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROLPortfolio所有者]</td> 
   <td>负责项目组合优先级和预算的利益相关者。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL潜在风险成本]</td> 
   <td>这是一个项目字段，您可以在列表和报告中找到它。 它显示了项目相关风险的潜在成本（如果发生）。 有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL前置任务]</td> 
   <td> <p>必须在从属任务完成之前完成的任务。 此外，还有标记为另一个任务的[！UICONTROL依赖关系]的任务。 前置任务允许计划员设置序列依赖关系逻辑，如在另一个任务完成后启动任务。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">前置任务概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主要公司]</td> 
   <td>用户所属的公司（在其用户设置中指定）。 公司还可以与项目关联。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主要联系人]</td> 
   <td><p>[！UICONTROL主要联系人]是问题的创建者，由以下人员自动指定 [!DNL Workfront] 当有人创建问题时。 如果您具有，则可以手动更新此字段 [!DNL Manage] 问题的权限。 问题只能有一个主要联系人。</p> 
   <p>如果更改了主要联系人，则最初指定为主要联系人的用户仍拥有该问题的[！UICONTROL管理]访问权限。</p>
   <p>将问题转化为任务或项目时，被指定为的[！UICONTROL主要联系人]的用户会成为该项目或任务的[！UICONTROL转换的问题发起人]。 如果在问题转化后更新了问题的[！UICONTROL主要联系人]，则转化后的[！UICONTROL问题发起人]将保留为转化发生时问题所在的[！UICONTROL主要联系人]。 另请参阅本文中的“[！UICONTROL转换的问题创建者]”。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL优先级]</td> 
   <td>可分配给任务、问题或项目的值，用于指定其重要性。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL专用]</td> 
   <td>在[！UICONTROL注释]或[！UICONTROL文档]上，此选项会将该对象隐藏给大多数查看者。 对于专用技术支持队列，只有队列团队中的用户可以通过[！UICONTROL技术支持]区域将问题提交到该队列。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL配置文件]</td> 
   <td>有关用户帐户的所有信息。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL程序]</td> 
   <td> <p>项目组合中的子集，可将相似的项目组合在一起，以实现明确定义的收益。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL程序管理]</td> 
   <td>管理跨项目的依赖项、风险、问题、要求和解决方案，保持项目正常运行，并实现确定的项目收益。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL项目所有者]</td> 
   <td>负责监督和组织活动的利益相关者，以确保项目目标与公司目标一致。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[！UICONTROL进度]</span> </td> 
   <td> <p>在[！UICONTROL目标]报表中，它显示战略目标完成时间的百分比。 进度百分比显示为数字。 有关战略目标的信息，另请参阅此表中的“[！UICONTROL目标]”。</p> <p>仅当您的组织购买了 [!DNL Workfront] 目标。 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 将项目添加到中的目标 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL进度状态]</td> 
   <td> <p>在项目、任务和目标报告中，此字段显示项目、任务或战略目标的进度状态。 有关更多信息，请参阅以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">项目进度状态概述</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任务进度状态概述</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">中的目标进度和条件概述 [!DNL Adobe Workfront Goals]</a> </p>
     <p>的[！UICONTROL目标]报表和[！UICONTROL进度状态] [!DNL goals] 字段仅在您的组织购买后才可见 [!DNL Workfront Goals]. 有关中的战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[！UICONTROL项目]</td> 
   <td> <p>必须在特定时间范围内完成的大量工作，且必须使用特定的预算和资源数量。 为了使项目易于管理，您需要将项目分成一系列任务。 完成所有任务即完成项目。 有关计划项目的信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">计划项目概述</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目分配计划小时数]</td> 
   <td> <p>在[！UICONTROL计划工作角色]报表中，它显示与分配给项目中任务或问题的工作角色关联的[！UICONTROL计划小时数]。 此字段和[！UICONTROL Initiative Job Role]报告类型未显示在中 [!DNL Workfront] 实例，除非您的公司已购买 [!DNL Workfront Scenario Planner] 许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md">此 [!DNL Workfront Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目详细信息]</td> 
   <td>项目当前状态的详细信息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目预算成本]</td> 
   <td> <p> 这是项目在列表和报告中显示的[！UICONTROL预算成本]。</p><p>另请参阅本文中的“[！UICONTROL预算成本]”。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL项目管理]</td> 
   <td>一组管理项目创建、分类和命名阈值的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL项目管理费用]</td> 
   <td>在[！UICONTROL小时]报表中，此字段为与小时类型[！UICONTROL项目时间]记录的小时数关联的财务信息保留。 项目可以有自己的记帐费率，如果某个项目直接记录了一个小时，则这些费率将在计算中使用。 根据项目设置，项目也可以使用不同的货币，并且这些小时数可以有一个货币换算。 [！UICONTROL项目开销]对象允许 [!DNL Workfront] 来获取这些信息。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目所有者]</td> 
   <td>负责管理项目的范围、时间表和分配的用户。 更改单、财务更改和交付项的默认审批人。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目计划]</td> 
   <td>开发和维护项目计划的过程。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目发起人]</td> 
   <td>您每个用户的指定利益相关者个人资料。 In [!DNL Workfront]，这些被指定为[！UICONTROL访问级别]</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目团队]</td> 
   <td> <p>分配给项目的用户或角色的集合</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">项目团队概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL项目跟踪]</td> 
   <td>用于衡量项目运行状况和范围的数据</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL预计]</td> 
   <td> <p>根据任务、问题或项目的计划小时数和完成百分比，估计完成工作的时间戳。</p> <p>指任务、问题或项目的日期或[！UICONTROL持续时间]。 通常，它指定在部分工作已完成或经过一段时间后，更符合工作项生命周期的日期和持续时间。 </p> <p>例如，任务的[！UICONTROL预计完成日期]是指 [!DNL Workfront] 根据迄今为止在该任务上完成的工作量、分配给该任务的人数以及自开始日期以来已经过的时间，估计该任务将完成。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对截止日期]</td> 
   <td> <p>在包含[！UICONTROL Document Version]对象的报表中（如[！UICONTROL Document Version]报表和[！UICONTROL Proof Approval]报表），此字段显示验证截止日期的星期几、日期、时间和年份。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对决定]</td> 
   <td> <p>在包含[！UICONTROL Document Version]对象的报表中（如[！UICONTROL Document Version]报表和[！UICONTROL Proof Approval]报表），此字段显示验证的决策状态（待处理、需要更改或已批准）</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对名称]</td> 
   <td> <p>在包含[！UICONTROL Document Version]对象的报表中（如[！UICONTROL Document Version]报表和[！UICONTROL Proof Approval]报表），此字段显示验证名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对页]</td> 
   <td> <p>在包含[！UICONTROL Document Version]对象的报表中（例如[！UICONTROL Document Version]报表和[！UICONTROL Proof Approval]报表），此字段显示验证中包含的页数。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对进度]</td> 
   <td> <p>在包含[！UICONTROL Document Version]对象的报表中（如[！UICONTROL Document Version]报表和[！UICONTROL Proof Approval]报表），显示验证的进度状态([！UICONTROL Sent]、[！UICONTROL Open]、[！UICONTROL Commended]、[！UICONTROL Decision Made])。</p> <p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">校对进度概述</a> 在 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">校对进度和状态概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL校对]</td> 
   <td>一种审核过程，其中一个或多个用户在图像、文本文档、视频或交互式Web内容中应更改的内容上标记和注释。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL公共]</td> 
   <td>在[！UICONTROL注释]或[！UICONTROL文档]上，此选项可让其他用户甚至外部人员访问该对象 [!DNL Workfront]. 对于[！UICONTROL技术支持队列]，[！UICONTROL公共]表示所有可以提交问题的用户都可以通过[！UICONTROL技术支持]区域提交问题。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL品质]</td> 
   <td>组织内对工作质量的感知。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL队列]</td> 
   <td>也称为[！UICONTROL技术支持队列]。 这是已发布到[！UICONTROL技术支持]区域的项目，允许用户向其提交问题。 通常为特定主题（例如Bug、项目请求等）创建队列。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL队列属性]</td> 
   <td>这些设置为发布到[！UICONTROL技术支持]的项目定义问题提交规则。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL队列主题]</td> 
   <td> <p>[！UICONTROL技术支持队列]上的属性，它允许提交问题的用户选择主题。 主题可以：</p> 
    <ul> 
     <li>与自定义数据表单关联。</li> 
     <li>通过所选主题上的路由规则集自动将问题分配给用户、角色或团队。</li> 
     <li>通过所选主题上的路由规则集，将问题移动到其他项目或队列。</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排名]</td> 
   <td> <p>在[！UICONTROL访问级别]报表中，您可以手动指定[！UICONTROL访问级别]的[！UICONTROL排名]。 这有助于您，因为 [!DNL Workfront] 管理员，以直观地确定与每个访问级别相关的复杂程度。 例如，您可以为较复杂的（[！UICONTROL计划]级别）访问级别提供较低的数字，为较不复杂的（[！UICONTROL请求者]级别）访问级别提供较高的数字。 您不能对标准访问级别进行排名。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL就绪]</td> 
   <td> <p>任务报告上的此字段指示是否已在积压工作中将[！UICONTROL Agile]任务标记为[！UICONTROL Ready]。 此标记仅适用于[！UICONTROL Agile]任务，这些任务已分配给[！UICONTROL Agile]团队。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL循环频率]</td> 
   <td> <p>显示在周期性任务父级的[！UICONTROL任务详细信息]或[！UICONTROL编辑任务]框中的字段。 它是任务周期性发生的频率。 有关创建周期性任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建周期性任务</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL参考编号]</td> 
   <td> <p>项目、任务和问题在创建时自动与唯一的参考编号关联。 您可以在项目、任务或问题的[！UICONTROL详细信息]页面，或者在列表或报告中查看[！UICONTROL参考编号]。 </p> <p><b>笔尖</b><p><br>当两个项目具有相同的名称时，可以推迟参考编号，因为参考编号始终是唯一的。 </p> <p>[!DNL Workfront] 在系统级别自动生成连续参考编号。 每个项目、任务或问题都会获得序列中的下一个可用编号。 <br></p> <p>例如，如果用户创建任务， [!DNL Workfront] 可能会自动将参考号分配给100。 如果用户B在此之后立即创建问题， [!DNL Workfront] 将问题指定为参考编号101。 不能手动编辑参考编号。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL拒绝问题]</td> 
   <td>在项目或任务报告中，这是在项目或任务审批被拒绝时创建的问题。 有关拒绝问题的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建批准流程</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL剩余风险成本]</td> 
   <td> <p>显示项目的[！UICONTROL计划风险成本]与项目上所有风险的[！UICONTROL实际成本]总和之间差额的项目字段。 </p> <p>使用以下公式计算项目的[！UICONTROL剩余风险成本]：</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL重新规划]</td> 
   <td>更改项目日期以修复或解决问题。 例如，一个已搁置几个月的项目将需要重新规划以反映准确的日期。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL报表]</td> 
   <td>包含有关给定一个的信息的图表或表 [!DNL Workfront] 对象及其相关属性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL请求]</td> 
   <td> <p>在单个集中队列中分类的一种问题，与正在进行的工作无关。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL请求队列]</td> 
   <td>由流量和分类流程管理的问题积压。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL请求速率]</td> 
   <td>接收和完成请求的总工作周期时间。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL请求者]</td> 
   <td>通常为许可证类型。 具有请求者许可证的用户可以提交关于在系统中发生新工作的请求。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL保留时间]</td> 
   <td>在用户个人时间中指定的天数，表示用户将无法工作。 请参阅“[！UICONTROL非工作日]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解决问题]</td> 
   <td> <p>在问题报告中，在视图或过滤器中使用此字段引用可解决该问题的问题。 </p> <p>有关在报告中显示解析对象的信息，请参见 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报告中查看可解析和解析对象信息</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解析项目]</td> 
   <td> <p>在问题报告中，在视图或过滤器中使用此字段引用解决问题的项目。 </p> <p>有关在报告中显示解析对象的信息，请参见 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报告中查看可解析和解析对象信息</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL解决任务]</td> 
   <td> <p>在问题报告中，在视图或过滤器中使用此字段可引用解决问题的任务。 </p> <p>有关在报告中显示解析对象的信息，请参见 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报告中查看可解析和解析对象信息</a> 在 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL资源]</td> 
   <td>系统中存在并分配给项目团队和任务的用户和/或角色。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[！UICONTROL资源管理]</td> 
   <td> <p>[！UICONTROL Resource Management]是一套企业工具，可让您根据资源的可用性准确预测资源的使用情况，以便按时完成必须完成的工作并符合预算。 </p> <p>利用资源管理工具，您可以计划资源的长期产能和短期计划需求。 </p> <p>有关资源管理的信息，请参见 [!DNL Workfront]，请参见 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">资源管理入门</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL资源管理器ID]</td> 
   <td><p>在项目报告中，在创建过滤器以查找特定资源管理器时，可以使用此选项。 </p></td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL资源管理器]</td> 
   <td> <p>在项目报告或列表视图中，这是一个信息字段，显示指定在项目上执行资源管理活动的用户。  在报告中使用“[！UICONTROL资源管理器]”时，将显示资源管理器列表，项目中每个资源管理器之间用逗号分隔。 您最多可以为给定项目指定30名资源经理。</p> <p>有关更多信息，请参阅文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">为项目或模板指定资源经理 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[！UICONTROL资源规划者预算小时数] </td> 
   <td>在[！UICONTROL资源规划者]中为项目编列预算的时数以及与项目关联的资源。 另请参阅本文中的“[！UICONTROL预算小时数]”。 </td> 
  </tr>  
  <tr> 
   <td>[！UICONTROL资源规划者] </td> 
   <td>高级 [!DNL Workfront] 工具，用于查看和管理跨项目、工作角色或用户的资源。 有关信息，请参阅 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源规划者概述</a>. </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL资源规划者预算劳力成本]</td> 
   <td> <p>这些是与使用资源规划者的项目工作角色的预算小时数关联的成本。 </p> <p>另请参阅本文中的“预算劳力成本”。 </p> </td>

</tr> 
  <tr> 
   <td>[！UICONTROL资源池]</td> 
   <td> <p>资源池是可与项目关联的用户的集合。同一资源池中的用户通常属于同一部门，具有相似或互补的技能，或者由同一预算提供资金。 您可以将多个资源池关联到一个项目或一个用户。 资源池可以专门分配给一个项目或由多个项目共享。</p> 
   <p>有关资源池的详细信息，请参见 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 资源池概述 </a>.</p> 
   <p>在项目报告中，资源池显示与项目关联的所有池。 此对象不能在分组中使用。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL资源利用率]</td> 
   <td>显示特定时间段内可用小时数和报告中为每个用户安排的小时数的报告。 此数值还计算为[！UICONTROL平均每天小时数]和分配百分比。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[！UICONTROL结果]</td> 
   <td>In [!DNL Workfront Goals]，结果便是一个目标的进度指示器。 它可以是手动更新的数字、百分比值或货币金额。 您不能在报表中显示结果，也不能通过 [!DNL Workfront] API。 有关活动的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront目标中的结果和活动入门</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL收入]</td> 
   <td>任务或项目的可记帐金额。 数量可以是每小时、固定或两者的组合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL收入类型]</td> 
   <td>收入类型确定任务应计收入的方式。 某些示例包括[！UICONTROL固定小时]、[！UICONTROL角色小时]和[！UICONTROL角色小时（包含上限）。 有关在中跟踪收入的信息 [!DNL Workfront] 参见 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">开单和收入概览</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Reviewer]</td> 
   <td>通常为许可证类型。 具有[！UICONTROL Reviewer]许可证的用户能够审查和批准系统中的工作项。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL风险]</td> 
   <td> <p>这可能指以下概念： [!DNL Workfront]：</p> 
    <ul> 
     <li> <p>项目中的一个字段，用于指示项目的风险程度。 您可以根据风险级别安排执行项目的优先顺序。 项目可能具有以下风险级别：</p> <p>- [！UICONTROL非常低]</p> <p>- [！UICONTROL低]</p> <p>- [！UICONTROL Medium]</p> <p>- [！UICONTROL高]</p> <p>- [！UICONTROL非常高]</p> <p>无法自定义您为项目指定的风险级别。 </p> <p> 有关更新项目风险的信息，请参阅文章的“项目设置”部分 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">编辑项目</a>. 您可以在报告中显示项目的风险字段。 </p> </li> 
     <li> <p>在项目生命周期中可能发生的事件，可识别对项目的成本、范围或计划的潜在影响。 您可以定义项目的潜在风险，并在构建项目的业务案例时将发生这些风险的概率或成本关联。 有关为项目的业务案例添加风险的信息，请参阅“创建和编辑项目风险”。 </p> <p>您无法在报表中显示[！UICONTROL商业论证]中定义的风险。 您只能在报告和列表中显示几种类型的风险成本。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL风险成本]</td> 
   <td> <p>与项目风险关联的成本。 以下是与可在报表中显示的项目相关的风险成本：</p> 
    <ul> 
     <li> <p>[！UICONTROL实际成本]：显示已发生风险的实际成本的风险字段。 除了报告和列表之外，在编辑或创建风险时，您还可以在[！UICONTROL编辑风险]框中找到它。 </p> <p>有关项目、任务或问题成本，请参阅本文中的“[！UICONTROL实际成本]”。 </p> </li> 
     <li> <p>[！UICONTROL计划风险成本]：显示项目中所有[！UICONTROL潜在风险成本]总计的字段。 另请参阅本文中的“[！UICONTROL计划风险成本]”。 </p> <p>有关潜在风险成本的信息，请参见 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本 </a>. </p> </li> 
     <li> <p>[！UICONTROL剩余风险成本]：项目中的一个字段，它显示所有风险的[！UICONTROL实际成本]总额与[！UICONTROL计划风险成本]之间的差额。 另请参阅本文中的“剩余风险成本”。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[！UICONTROL风险管理]</td> 
   <td>识别、缓解和监控风险的流程。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL角色]</td> 
   <td>请参阅本文中的“[！UICONTROL工作角色]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL路由]</td> 
   <td>自动指派或移动问题，通常是由于队列主题或作为队列的默认路由（路由规则）。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL路由规则]</td> 
   <td>项目和队列中的设置，用于自动将问题分配给用户、角色或团队，或将问题移动到其他项目或队列。 路由规则通常与技术支持队列一起使用，以自动分配传入问题。</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL保存的搜索]</td> 
   <td>已保存搜索条件的搜索。 通过保存的搜索，可以轻松地再次运行相同的搜索，而无需再次输入搜索条件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL场景] (位于 [!DNL Workfront Fusion]) </td> 
   <td> <p>场景由一系列步骤（模块）组成，这些步骤（模块）指示应如何在应用程序/服务之间传输和转换数据。</p> <p>有关中的方案的信息 [!DNL Workfront Fusion]，请参见 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 方案概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Scenario](在 [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>在 [!DNL Scenario Planner]，场景是计划的副本。 </p> <p>此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">此 [!DNL Scenario Planner] 概述</a>. </p> <p>有关创建方案的信息，请参见 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">在中创建和比较计划方案 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划]</td> 
   <td>每周工作计划，包括工作时间，以及休息日（如假日）和例外日（如星期六工作日）。 可以将计划应用于项目和用户。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划劐免]</td> 
   <td>也称为[！UICONTROL Modified Shift]。 计划的天数，与计划定义的常规每周工作时间形成对比。 例如，计划工作的星期六，如果计划设置为仅工作星期一到星期五，则属于[！UICONTROL计划劐免]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL计划报告]</td> 
   <td> <p>在构建报告报告时，如果计划使用[！UICONTROL计划报告]字段交付报告，则可以显示有关报告计划的信息。 此字段在项目符号列表中显示多个值，每个报表的每个计划显示一个。 有关计划报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">报表交付概述</a>.</p> <p>由于此字段显示多个值，因此无法用于分组。 您只能在过滤器或视图中访问它。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL范围更改]</td> 
   <td>一个[！UICONTROL审核记录]，如果处于活动状态，则会在任何时候对项目或任务的范围进行更改时生成注释，例如，如果更改了[！UICONTROL任务持续时间]或[！UICONTROL前置任务]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL节]</td> 
   <td>创建带有自身标题的屏幕上区域以组织自定义数据以供显示。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL分节符]</td> 
   <td>区域之间的间隙或边框。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL安全性]</td> 
   <td>允许用户与系统中的特定对象进行交互的设置，而不与系统中的其他对象进行交互的设置。 另请参阅本文中的“[！UICONTROL访问级别]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL设置]</td> 
   <td>管理员可以设置系统配置和首选项的区域。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL严重性]</td> 
   <td> <p>[！UICONTROL Severity]表明项目影响工作完成的可能性。 例如，高[！UICONTROL严重性]的问题可能完全阻止任务的完成，但低[！UICONTROL严重性]的问题可能只是表面上的。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 更新问题严重程度</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL严重程度]</td> 
   <td>请参阅本文中的“[！UICONTROL严重性]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL共享]</td> 
   <td>允许其他用户在中查看或编辑特定项目的操作 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROLSlack日期]</td> 
   <td>在任务视图或报告中，[！UICONTROLSlack日期]显示任务肯定会影响项目的[！UICONTROL完成日期]的确切日期。 有关任务的[！UICONTROLSlack日期]的信息，请参见 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">任务Slack日期概述</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL智能分配]</td> 
   <td> <p>向用户分配任务或问题时， [!DNL Workfront] 根据最佳用户完成工作可用的时间及其与项目的关系，提出有关最佳用户完成工作的建议（[！UICONTROL智能分配]）。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">智能分配概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源]</td> 
   <td> <p>指示另一个对象的父对象。 例如，附加到任务的文档在[！UICONTROL文档]报告或视图的[！UICONTROL源]字段中具有任务的名称；在项目下记录的问题在问题报告或视图的[！UICONTROL源]字段中具有项目的名称。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL开始日期]</td> 
   <td> <p>项目工作的开始日期。 中存在多个开始日期 [!DNL Workfront]： </p> 
    <ul> 
     <li>[！UICONTROL计划]</li> 
     <li>[！UICONTROL Actual]</li> 
     <li>[！UICONTROL预计] </li> 
    </ul> <p>在[！UICONTROL费率报表]中，这是在项目级别的工作角色的新计费率开始的日期。 在此日期之后与项目关联的小时数乘以该记帐费率来计算项目收入。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL状态]</td> 
   <td> <p>用于表示工作项或战略目标的工作流位置的指示器。</p> <p>对于项目，[！UICONTROL状态]是项目中的一个设置，用于指示该项目是否为：</p> 
    <ul> 
     <li>[！UICONTROL当前版本]</li> 
     <li>[！UICONTROL已搁置] </li> 
     <li>[！UICONTROL完成] </li> 
     <li>[！UICONTROL已终止]</li> 
    </ul> <p>有关项目状态的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">访问系统项目状态列表</a>.</p>
    <p>对于任务，[！UICONTROL Status]是任务中的一个设置，用于指示任务是否为：</p> 
    <ul> 
     <li>[！UICONTROL新]</li> 
     <li>[！UICONTROL正在进行中]</li> 
     <li>[！UICONTROL完成]</li> 
    </ul> <p>有关任务状态的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">访问系统任务状态列表</a></p> <p>对于问题，[！UICONTROL状态]是问题中的一个设置，用于指示此问题是否为：</p> 
    <ul> 
     <li>[！UICONTROL新]</li> 
     <li>[！UICONTROL正在进行中]</li> 
     <li>[！UICONTROL等待反馈]</li> 
     <li>[！UICONTROL已搁置]</li> 
     <li>[！UICONTROL已解析]</li> 
     <li>[！UICONTROL无法解析]</li> 
     <li>[！UICONTROL无法复制]</li> 
     <li>[！UICONTROL验证完成]</li> 
     <li>[！UICONTROL已重新打开]</li> 
    </ul> <p>有关问题状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>.</p> 
    <p>对于策略目标，[！UICONTROL状态]是目标上的设置，用于指示目标是否为：</p> 
     <ul> 
      <li>[！UICONTROL活动]</li> 
      <li>[！UICONTROL草稿]</li> 
      <li>[！UICONTROL不活动]</li> 
      <li>[！UICONTROL已关闭]</li> 
     </ul> 
     <p>有关战略目标的更多信息，另请参阅本文中的“[！UICONTROL目标]”或“[！UICONTROL目标]”。 </p> 
     <p>对于战略目标，此字段仅在您的组织已购买的情况下可见 [!DNL Workfront Goals]. 有关使用管理战略目标的信息 [!DNL Workfront Goals]，请参见 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL状态更改]</td> 
   <td>[！UICONTROL审核记录]。 当用户更改项目、任务或问题的状态时，将生成注释。</td> 
  </tr> 
  <tr> 
   <td>状态图标</td> 
   <td> <p>您可以将内置的[！UICONTROL状态图标]字段添加为视图中的列，以增强对象关键点的可见性，例如：</p> 
    <ul> 
     <li>对象已附加文档</li> 
     <li>对象与审批流程相关联</li> 
     <li>对象具有与其关联的附加注释</li> 
     <li>费用是应计费的或应偿还的 </li> 
     <li>任务在关键路径上</li> 
     <li>用户属于公司、团队或位于不同的时区 </li> 
    </ul> <p>您可以在以下对象的视图中添加[！UICONTROL状态图标]字段： </p> 
    <ul> 
     <li>[！UICONTROL任务]</li> 
     <li>[！UICONTROL问题]</li> 
     <li>[！UICONTROL项目]</li> 
     <li>[！UICONTROL模板任务]</li> 
     <li>[！UICONTROL模板]</li> 
     <li>[！UICONTROL费用]</li> 
     <li>[！UICONTROL文档]</li> 
     <li>[！UICONTROL用户]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL状态更新]</td> 
   <td> <p>此字段显示用户在“[！UICONTROL更新状态]”字段中提供的最新状态更新。 对状态更新所做的注释不会显示在[！UICONTROL状态更新]列中。</p> <p>要显示“[！UICONTROL New]”、“[！UICONTROL In Process]”、“和“[！UICONTROL Complete]”状态，请使用[！UICONTROL Status]列。</p> <p>对状态更新所做的注释不会显示在[！UICONTROL状态更新]列中。</p> <p>有关状态的更多信息，请参阅文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任务状态</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL状态]</td> 
   <td>请参阅本文中的“[！UICONTROL状态]”。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL Storyboard]</td> 
   <td>一个图表，它表示故事的状态（敏捷方法中的任务）以及故事走向完成的方式。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL故事小时数]</td> 
   <td>用于衡量“故事”的难度或复杂性的量度。 Agile团队可以选择使用小时数还是点数。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL故事点]</td> 
   <td>用于衡量“故事”的难度或复杂性的量度。 Agile团队可以选择使用小时数还是点数。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL Strategic]</td> 
   <td>改变组织或组织工作方式的长期工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL策略对齐]</td> 
   <td>跨产品组合和计划衡量和协调公司目标。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL订阅者]</td> 
   <td> <p>订阅项目、任务或问题的用户。</p> <p>在报告中使用此字段时，将显示订阅者列表，每个订阅者之间用逗号分隔。</p> <p>有关更多信息，请参阅文章 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">订阅中的项目 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL摘要任务]</td> 
   <td>请参阅本文中的“[！UICONTROL父任务]”。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Subtask]</td> 
   <td>位于父任务下的子任务。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL系统管理]</td> 
   <td>一组管理系统更改和维护的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL系统集成]</td> 
   <td>将不同的计算系统和软件应用程序在物理或功能上连接在一起以便作为一个协调的整体的过程。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任务]</td> 
   <td> <p>作为实现最终目标（完成项目）的步骤而必须执行的活动。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">任务概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任务属性]</td> 
   <td>与任务关联并指示有关任务的某些详细信息的其他字段或对象。 例如[！UICONTROL规划完成日期]和[！UICONTROL状态]。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL任务约束]</td> 
   <td>请参阅“[！UICONTROL约束类型]”和“[！UICONTROL约束日期]”。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任务管理]</td> 
   <td>一组管理任务创建、分配、关闭和可见性阈值的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[！UICONTROL任务所有者]</td> 
   <td>负责估计工作量和完成任务的团队或用户</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[！UICONTROL团队]</td> 
   <td> <p>致力于相似目标或业务目标的用户集合。 通过将团队分配给工作项，可以将这些用户集体分配给工作项。</p> <p>有关Teams的详细信息，请参阅 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">团队概述</a>.</p> <p>项目可以有一个[！UICONTROL项目团队]，其中包含与项目工作关联的所有用户或角色。</p> <p>有关项目团队的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[！UICONTROL模板]</td> 
   <td> <p>项目模板是最可重复项目的一般概要。 在创建项目模板时，您可以定义任务、队列主题、自定义表单、附加文档或审批，以便在必须创建新项目时节省时间。 </p> <p>您可以将模板附加到现有项目，也可以使用它们来构建新项目。 模板中指定的所有信息都会传输到使用它创建的项目。 </p> <p>有关模板的详细信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">项目模板概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL模板任务]</td> 
   <td>属于模板一部分的任务。 模板任务在使用模板创建的项目中变为任务。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL线程]</td> 
   <td>与特定主题相关的[！UICONTROL注释]及其回复集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL缩略图]</td> 
   <td> <p> 在[！UICONTROL Document]列表或报表中，它以缩略图显示文档的预览。 </p> <p> 选择 <strong>[！UICONTROL缩略图]</strong>  查看报表中33-66像素宽的缩略图。 </p> <p>当您修改列表或报表中的列宽时，缩略图的大小会进行调整。</p> <p>另请参阅本文中的“[！UICONTROL大型缩略图]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL休息时间]</td> 
   <td>您可以构建一个[！UICONTROL休息时间]报表，以查看用户在其配置文件中指示休息时间的时机。 </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL时间表]</td> 
   <td> <p>允许用户输入在项目、任务或问题上花费的实际小时数，或用于与工作无关的其他活动（如会议或培训）的小时数的工时表。 除了输入工作所花费的时间量之外，您还可以通过使用小时类型来定义时间条目，指明时间是与工作有关还是相当于制造费用时间。 有关时间表的信息，请参阅 <a href="../../../timesheets/timesheets/timesheets-overview.md">工时表概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL时间表配置文件]</td> 
   <td> <p>[！UICONTROL时间表配置文件]是一个模板，用于 [!DNL Workfront] 使用自动为与其关联的用户创建时间表。 </p> <p>您可以配置一些设置，这些设置将在创建每个时间表时应用于每个时间表。 其中一些设置是：时间表应创建的频率（每周、每两周、每月或每月两次）、时间表开始日期、时间表批准者、用户可以与记录小时数关联的[！UICONTROL小时类型]。</p> </td> 
  </tr> 
  <tr > 
   <td>[！UICONTROL顶级父级ID] </td> 
   <td> <p>利用此字段，可识别和筛选列表或报告中有关顶级组及其子组的数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL顶级父名称] </td> 
   <td> <p>此字段允许您为列表或报告标识[！UICONTROL视图]中有关顶级组及其子组的数据。</p> <p>您还可以使用[！UICONTROL顶级父级ID]字段执行此操作。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL总小时数]</td> 
   <td> <p>在[！UICONTROL项目报告]中，此字段显示项目所有小时数的舍入总和，即上次计算项目财务的时间。 [！UICONTROL实际小时数]反映在项目上记录的准确小时数。 通常，[！UICONTROL实际小时数]应与[！UICONTROL总小时数]匹配。 如果[！UICONTROL总小时数]与[！UICONTROL实际小时数]字段显示有显着差异，则必须重新计算项目的财务。</p> <p>有关重新计算项目财务的更多信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">重新计算项目财务</a>.</p> <p>在时间表[！UICONTROL标准]视图中，此字段是指在时间表上显示的日期为项目记录的总小时数。 此内置视图中时间表的[！UICONTROL Total Hours]字段引用“[！UICONTROL hoursDuration]”字段，该字段动态计算时间表开始日期和结束日期之间的小时数差异。 如果用户记录的时间比时间表时间范围内的可用小时数还长，则使用此选项以红色显示[！UICONTROL总小时数]列。 有关更多信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">在时间表上查看总小时数</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL跟踪模式]</td> 
   <td> <p>任务的属性。 这决定了如何更新任务的预计时间线，以及如何更新预计时间线。 例如：</p> 
    <ul> 
     <li>[！UICONTROL用户必须更新]要求手动更新任务。 否则，它将变成[！UICONTROL Backed Schedule]，然后[！UICONTROL Late]。</li> 
     <li>当到期日期或[！UICONTROL规划完成日期]已过时，[！UICONTROL自动完成]将自动完成任务。</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任务跟踪模式概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[！UICONTROL Trigger]</td> 
   <td>启动方案的事件。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL故障任务]</td> 
   <td>条件为[！UICONTROL Late]、[！UICONTROL Backed Schedule]或[！UICONTROL At Risk]的未完成任务。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL未分配任务]</td> 
   <td>未分配给任何用户、角色或团队的任务。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL更新类型]</td> 
   <td> <p>项目中的一个设置，用于确定何时重新计算项目的预计时间线。 选项包括：</p> 
    <ul> 
     <li>[！UICONTROL Automatic and On Change]</li> 
     <li>[！UICONTROL Automatic Only]</li> 
     <li>[！UICONTROL手册] </li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用户]</td> 
   <td>在中创建的帐户 [!DNL Workfront] 允许人员登录并与系统交互。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[！UICONTROL用户委派]</p> </td> 
   <td> <p>可报告对象，用于告知您：</p> 
    <ul> 
     <li>哪些用户已委派任务、问题和项目审批</li> 
     <li>哪些用户具有委托给他们的任务、问题和项目审批</li> 
     <li>当这些委托开始和结束时</li> 
    </ul> <p>要了解更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">创建用户委派报告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用户界面]</td> 
   <td>的所有可视化和交互式方面 [!DNL Workfront] 应用程序。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用户界面首选项]</td> 
   <td>[！UICONTROL用户界面设置]。 [!DNL Workfront] 管理员可以更改这些设置以自定义用户界面的各个方面。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[！UICONTROL利用率]</td> 
   <td>用户或角色的可用性，基于分配的调度、PTO和当前工作负载。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用户使用情况]</td> 
   <td> <p>搜索与显示用户（资源）如何分配或过度分配的报表相结合。 请参阅本文中的“[！UICONTROL资源利用率]”。</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>对象名称</th> 
   <th>描述</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Velocity]</td> 
   <td>对总工作周期时间（完成某项工作需要多长时间）以及工作在最初提交的时间内的完成频率（工作与提交时间的比率）的衡量。</td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL视图]</td> 
   <td> <p>视图可用于修改报告或项目、任务或问题列表中的列，也可用于指示用户仅有权查看访问级别或权限共享级别的信息。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL视图图标]</td> 
   <td> <p> 这是与状态图标相同的字段，但它仅适用于以下视图： </p> 
    <ul> 
     <li> [！UICONTROL文档] </li> 
    </ul> <p> 有关更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上个月查看次数]</td> 
   <td> <p>在报表列表中，它显示上个月查看报表的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL上季度查看次数]</td> 
   <td>在报表列表中，它显示上季度查看报表的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >查看报告使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL去年查看次数]</td> 
   <td>在报表列表中，它显示去年查看报表的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL本月查看次数]</td> 
   <td> <p>在报表列表中，它显示本月查看报表的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL本季度查看次数]</td> 
   <td>在报表列表中，它显示本季度报表被查看的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报告使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL今年的查看次数]</td> 
   <td>在报表列表中，它显示本年度查看报表的次数。<br>有关报告列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">查看报告使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>在项目、任务或问题报告中，在文本模式下使用以下语句显示项目、任务或问题的已计划小时数：</p>
   <p></p><p></p> 
   <p>有关使用文本模式的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>. </p> 
   <p><b>笔尖</b> 
   <p>在问题报告中，添加一个[！UICONTROL Planned Hours]字段将添加 <code>work </code>字段到报表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作]</td> 
   <td> <p>两种主要许可证类型之一。 此计划的访问权限少于[！UICONTROL计划]，但可以在系统中创建和进行更新。 与[！UICONTROL External]、[！UICONTROL Reviewer]或[！UICONTROL Requester]许可证类型相比，这种功能更强大。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> <p>工作可能是指项目、任务或问题的[！UICONTROL已计划小时数]。 有关更多信息，请参阅此表中的“[！UICONTROL工作]”字段。 </p> <p>提示：在问题报告中，添加一个[！UICONTROL已计划小时数]字段将添加 <code>work </code>字段到报表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作分解结构]</td> 
   <td>项目团队根据父/子关系执行任务的层次结构。</td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL工作量] </td> 
   <td> 
    <p>项目经理可能会决定使用此字段而不是[！UICONTROL计划小时数]来估算完成任务所需的工作量。 仅当满足以下条件时，此字段才可见：</p> 
     <ul> 
      <li> <p>该任务具有[！UICONTROL简单持续时间类型]。 </p> <p>提示：如果将任务[！UICONTROL持续时间类型]更新为任何其他类型，则此字段将变为隐藏。 </p> </li> 
      <li>项目经理已启用[！UICONTROL使用工作投入]以自动计算项目中的任务[！UICONTROL已计划小时数]字段。 </li> 
     </ul> 
     <p>有关使用[！UICONTROL工作投入]而不是[！UICONTROL计划小时数]来估计任务投入的信息，请参阅 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作投入概述</a>. </p> 
     <p>您可以在任务报告和列表中显示此字段。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[！UICONTROL工作项]</td> 
   <td> <p>此字段是指中的任务或问题 [!DNL Workfront]. </p> <p>[！UICONTROL工作项]报告同时显示任务和问题的信息。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理组合]</td> 
   <td>用于运行业务与更改业务的工作分配比例的[！UICONTROL工作绩效指标] (WPI)。 混合WPI可帮助您在组织层面了解您的策略是否应用了任何实际的工作分配。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理资源]</td> 
   <td>系统中有资格接收工作或跟踪时间的角色指定。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理角色和职责]</td> 
   <td>定义负责管理指定问题、任务、项目、项目群或项目组合的范围、执行和批准的所有者和利益相关者。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理SLA]</td> 
   <td>所有利益相关者商定的可量化的指标。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理利益相关者]</td> 
   <td>在工作请求的结果中具有既得利益的用户集合。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作管理接触点]</td> 
   <td>利益相关者之间通信的数字化记录。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作绩效指标] </td> 
   <td> <p>混合比例、容量、速度、质量和参与度。</p> <p>WPI是[！UICONTROL工作绩效指标]的常用首字母缩写。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作流程]</td> 
   <td> <p>接收、区分优先次序和执行工作的方法。 您执行工作的方式通常称为“工作流”或“项目计划”（包含日期、前置任务关系等任务的列表）。 </p> <p>工作流程的示例可能是生产单个资产或交付多资产营销活动。 </p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作流模板]</td> 
   <td>在[！UICONTROL验证审批]报告中，此字段显示附加到验证的任何工作流模板。 如果没有附加模板，则该列为空。</td> 
  </tr>

<tr> 
   <td>[！UICONTROL工作时间]</td> 
   <td>

<p>表示用户在相当于全职([！UICONTROL FTE])时间中可用于实际工作（不包括开销）的百分比。 [！UICONTROL工作时间]必须是最多为1的小数，并且不能为0。 例如，实际工作的20%可用性将是0.2。</p>
   </p>该字段的默认值为1，表示用户将其整个[！UICONTROL FTE]用于实际的项目相关工作。  </p>
   <p>系统使用此数字来计算用户实际完成项目相关工作的可用性。 </p>
   <p> 安排例外和休息时间也可能会影响用户容量。 </p>
   <p>有关在Workfront中创建调度的详细信息，请参见 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>. </p>
    <p>Workfront根据[！UICONTROL设置]区域中的资源管理首选项计算用户的可用性。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">配置资源管理首选项</a>. </p> 
   <p>在编辑或创建用户时，您可以更新该用户的[！UICONTROL工作时间]。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">编辑用户配置文件</a></p> 
   <b>笔尖</b> 
   <p>将[！UICONTROL工作时间]值设置为1，表示用户可用于其整个全职等效项目相关工作。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL工作时间]</td> 
   <td>在Workfront文档中，此术语用于描述根据计划分配的工作时间。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>在项目、任务或问题报告中，在文本模式下使用以下语句显示项目、任务或问题的已计划小时数，后跟“小时数”：</p>
   <p></p><p></p>
    <p>有关使用文本模式的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
