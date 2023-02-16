---
content-type: reference
navigation-topic: workfront-navigation
title: 术语表 [!DNL Adobe Workfront] 术语
description: 的 [!DNL Adobe Workfront] 术语表列出了Adobe Workfront中常用的术语。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: 4a33d72e234ff812a72d7d7a382226697f858df6
workflow-type: tm+mt
source-wordcount: '19106'
ht-degree: 0%

---

# 术语表 [!DNL Adobe Workfront] 术语

>[!IMPORTANT]
>
>本文应作为参考，以了解您在 [!DNL Adobe Workfront] 应用程序，在 [!DNL Workfront] 文档，或通常涉及规划和管理工作时。 我们当前正在更新此信息，因此此表可能不完整。 当我们认为此信息详尽无遗时，我们将删除此免责声明。

下表是Adobe Workfront中常用术语的列表：

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
   <td>[!UICONTROL访问级别]</td> 
   <td>用户配置文件，用于确定用户如何与Workfront中的不同对象和工具进行交互。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>当前项目中的未完成任务，该任务无法被前置任务处理，并且没有具有未来计划起始日期的任务约束。 换句话说，它今天可以用。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>在 [!DNL Workfront Goals]，则活动是目标的进度指示器。 它可以是手动更新的进度条，也可以是与目标关联的项目。 您无法在报表中显示活动，也无法通过 [!DNL Workfront] API。 有关活动的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">在Adobe Workfront目标中开始使用结果和活动</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL实际成本]</td> 
   <td> <p>对于任务和问题，这是与实际记录的小时数相关的成本，与分配给任务或问题的资源的每小时成本率有关。 对于项目，这是项目任务和问题中的所有[!UICONTROL实际成本]的总和。 有关信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL实际费用成本]</td> 
   <td> <p>为项目或任务记录的所有费用的[!UICONTROL实际金额]总和。</p> <b>示例 </b>
   <p>如果为任务1创建费用，并在“[!UICONTROL实际金额]”字段中输入$600.00，则此任务的“[!UICONTROL实际费用成本]”为$600.00。 </p> 
   <p>对于项目， [!DNL Workfront] 使用以下公式计算[!UICONTROL实际费用成本]:</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs)</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL实际小时数]</td> 
   <td> <p>在项目、任务或问题报表中，[!UICONTROL实际小时数]是记录在项目、任务或问题上的所有小时数之和。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span> 如果从任务1的[!UICONTROL Updates]选项卡中，单击“Log Time”（日志时间）并输入25小时，则任务1的实际小时数= 25小时。 </p> <p>[!DNL Workfront] 使用以下公式计算父任务或项目的[!UICONTROL实际小时数]:</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL实际人工成本]</td> 
   <td> <p>与在任务或项目中投资的人工关联的[!UICONTROL实际成本]。 </p> <p>对于任务， [!DNL Workfront] 使用以下公式计算[!UICONTROL实际人工成本]:</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>如果任务的[!UICONTROL成本类型]为[!UICONTROL用户每小时]，则 [!DNL Workfront] 使用用户费率。 如果任务的[!UICONTROL成本类型]为[!UICONTROL角色“每小时”]，则 [!DNL Workfront] 使用任务职责费率计算[!UICONTROL实际人工成本]。 </p> <p>对于项目， [!DNL Workfront] 使用以下公式计算[!UICONTROL实际人工成本]:</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>例如，如果用户使用[!UICONTROL用户每小时] [!UICONTROL成本类型]记录某项任务的5小时，并且其每小时费率为$100，则[!UICONTROL实际人工成本]为$500。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL实际收入] </td> 
   <td> <p>项目或任务的[!UICONTROL实际收入]是与项目或任务的[!UICONTROL实际小时数]关联的金额。 </p> <p>有关跟踪 [!DNL Workfront]，请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL实际开始]</td> 
   <td>用户在为其分配的工作中更改正在进行的对象时的时间戳。</td> 
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
   <td>[!UICONTROL Agile]方法</td> 
   <td>一种方法，它基于需求和解决方案与跨职能团队的协作演变。 它鼓励根据固定的时间表进行灵活和更改。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>与传统团队不同，因为他们会从积压的工作中提取其潜在工作，并在称为[!UICONTROL迭代]的设定时间段内对其进行处理。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的所有团队]</td> 
   <td> <p>当在[!UICONTROL过滤器]中引用该过滤器时，此字段会显示属于登录用户所属任何团队的用户，或分配给登录用户所属任何团队的工作项目。 </p> <p>我们建议在过滤器中使用此字段，以便在与其他用户共享报表时使报表更加通用。 这样，您就只能构建一个报表，该报表将根据登录者查看该报表的方式显示不同的信息，因为该信息始终为登录用户进行自定义。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配日期]</td> 
   <td> <p>您可以在以下类型的报表中找到此字段：</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project]（财务数据）</li> 
     <li>[!UICONTROL预算小时数]</li> 
    </ul> <p>对于<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL项目（财务数据）]报表： </p> 
    <ul> 
     <li>在尝试了解时构建此报表 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> 分配给您的资源的[!UICONTROL计划时数]。</li> 
     <li> <p>[!UICONTROL分配日期]是一周的第一天（星期日），此时将[!UICONTROL作业角色]分配到任务。 资源（[!UICONTROL作业角色]）在分配给的任务的[!UICONTROL持续时间]期间，其分配日期可以与其拥有的周数相同。 如果任务跨越多个月，则当任务在任务的[!UICONTROL持续时间]内时，一个月的第一天也可以成为[!UICONTROL分配日期]。</p> <p>例如，您可以将[!UICONTROL作业角色]分配给一个跨越3周且具有90 [!UICONTROL计划时数]的任务。 这些小时在任务期间平均分配，这会使每天将6 [!UICONTROL计划时间]分配给您的工作角色：</p> <p><em> [!UICONTROL每日计划时数] = [!UICONTROL总计划时数]/任务[!UICONTROL工作日数]期间的任务[!UICONTROL持续时间] </em> </p> <p>因此，有三个[!UICONTROL分配日期]，在任务的[!UICONTROL持续时间]期间，每周的星期日各显示一个日期，每个日期都与这些日期关联一定数量的[!UICONTROL计划时间]。<br>如果任务在一个月的最后一周中开始，并在新月份开始后的两周结束，则该任务将具有四个[!UICONTROL分配日期]:在任务的[!UICONTROL持续时间]期间，每周的星期日各显示一个，在新月份的第一天显示一个。</p> <p>为了充分利用此信息，我们建议您构建 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> 项目（财务数据）报表并为[!UICONTROL分配日期]添加矩阵分组，然后对结果进行每周、每月、每季或每年分组，以获得最准确的数据。<br>有关构建矩阵分组的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">创建矩阵报表</a>.</p> </li> 
    </ul> <p>仅当与财务信息关联的数据不到5年时，财务信息才会填充在[!UICONTROL项目（财务数据）]报表中。 例如，如果在2015年1月将作业角色分配给任务，而今天是2021年9月，则诸如作业角色的[!UICONTROL分配日期]之类的财务字段不会在[!UICONTROL项目（财务数据）]报表中填充。 </p> 
    <div> 
     <p>对于[!UICONTROL Debuded Hour]报表：</p> 
     <ul> 
      <li>在尝试了解分配给您的资源或资源计划器中项目的[!UICONTROL预算小时数]时，生成此报表。</li> 
      <li> <p>[!UICONTROL分配日期]是您在[!UICONTROL资源计划器]中预算小时数的一周的第一天（星期日）。 </p> <p>提示：   <p>如果一周跨越两个月，它将在报表中生成两行：一个对应于一周的第一天（第一周的星期日，即在第一个月），而第二行则显示第二个月的第一天。 </p> <p>例如，如果您为6月30日（星期日） — 7月6日（星期六）这一周的用户预算8小时，则这两行将显示6月30日和7月1日的[!UICONTROL分配日期]。 </p> </p> <p>有关 [!DNL Resource Planner]，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">预算资源 [!DNL Resource Planner] 使用[!UICONTROL Project]和[!UICONTROL Role]视图</a>.</p> <p>有关生成[!UICONTROL预算小时]报表的信息，请参阅 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">报表：预算小时数</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公告]</td> 
   <td> <p>一种与系统内的用户信息通信的方法。 这些信息通常来自 [!DNL Workfront] 从管理员到用户。 </p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">发送公告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL应用程序集成]</td> 
   <td>应用程序通常表示软件应用程序的连接器，但也可以表示处理数据的特殊功能。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL审批者决策]</td> 
   <td> <p>在[!UICONTROL校样批准]报表中，此字段显示不再活动的校样的校样批准决策。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL审批者阶段]</td> 
   <td>在[!UICONTROL校样批准报表]中，此字段显示有关当前阶段校样的信息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>给定工作项（如任务、文档或时间表）可能要求主管或其他用户在工作项上签名。 此注销过程称为批准。 </p> <p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">审批流程概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL批准日期]</td> 
   <td>在[!UICONTROL校样批准]报表中，此字段显示校样批准的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL审批者]</td> 
   <td>必须在给定工作项上注销的用户或职务角色，或在工时单上批准工时条目的用户。</td> 
  </tr> 
  <tr> 
   <td>[!Uicontrol已分配给]</td> 
   <td> <p>在[!UICONTROL任务或问题]报表中，此字段显示任务或问题的所有者，或[!UICONTROL主要被分派人]。 您也可以按此字段进行筛选或分组。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配]</td> 
   <td>分配给问题或任务的用户、作业角色或团队。 项目、项目组合或项目群不能有分配。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配]</td> 
   <td> <p>在[!UICONTROL任务]或[!UICONTROL问题]报表中，此字段显示分配给该任务或问题的所有实体（用户、作业角色、团队）的列表。 您可以使用字段[!UICONTROL Assignment Users]和[!UICONTROL Assignment Roles]按此字段过滤。 您可以使用“团队”字段按分配给任务或问题的团队进行筛选。 不能按此字段对报表进行分组。</p> <p>放置在[!UICONTROL回收站]中的工作项将继续显示在某些报表中，这些报表引用了[!UICONTROL分配]对象，其中 [!DNL OR] 过滤器修饰符。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配角色]</td> 
   <td>
   <p>在[!UICONTROL任务]或[!UICONTROL问题]报表中，此字段显示分配给任务或问题的作业角色的信息。 此字段显示[!UICONTROL主要所有者]，以及分配给任务或问题的其他作业角色。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配状态]</td> 
   <td> <p>在分配、任务或问题报表中，[!UICONTROL分配状态]显示分配给工作项的用户是单击了[!UICONTROL Work On It]按钮还是单击[!UICONTROL Done]按钮以接受或完成工作。 存在以下[!UICONTROL分配状态]:</p> 
    <ul> 
     <li><b>[！已请求UICONTROL]</b>:已为用户分配了任务或问题，但他们尚未单击[!UICONTROL Work On It]按钮以开始处理该任务或问题。</li> 
     <li><b>[!UICONTROL工作]</b>:用户已单击[!UICONTROL Work On It]按钮，且当前正在处理该项目。 </li> 
     <li><b>[!UICONTROL Done]</b>:用户已单击[!UICONTROL Done]按钮，并完成了对该项目的工作。 </li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL Work It]和[!UICONTROL Done]按钮概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配团队]</td> 
   <td>
   <p>在[!UICONTROL task]或[!UICONTROL issue]报表中，此字段显示分配给任务或问题的团队的信息。 该字段显示[!UICONTROL主要所有者]，以及分配给任务或问题的其他团队。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL分配用户]</td> 
   <td>
   <p>在[!UICONTROL任务]或[!UICONTROL问题]报表中，此字段显示有关分配给任务或问题的用户的信息。 此字段显示[!UICONTROL主要所有者]，以及分配给任务或问题的其他用户。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL属性]</td> 
   <td>属性是 [!DNL Workfront] 对象。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL审核区域]</td> 
   <td> <p>审核是用于记录在Workfront中发生的操作的系统消息。 记录了以下审计类型：</p> 
    <ul> 
     <li>[!UICONTROL范围更改]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL状态更改]</li> 
     <li>[!UICONTROL注意]</li> 
     <li>[!UICONTROL组合条目]</li> 
     <li>[!UICONTROL错误条目]</li> 
     <li>[!UICONTROL状态更改]</li> 
     <li>[!UICONTROL订阅更改]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL审核记录]</td> 
   <td>由通过“记录的更改”（[!UICONTROL审核区域]）进行跟踪的事件自动生成的注释集合。 每张便笺都记录了谁执行了该操作，他们执行了什么操作，以及他们何时执行了该操作。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>[!UICONTROL项目更新]类型之一。 当夜间重新计算流程运行以及对项目中的项目或任务进行任何更新时，系统将重新计算项目的预计时间轴和计划时间轴。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>可用性</p></td> 
   <td> <p>此术语用于“用户可用性”或“资源可用性”，它说明资源（用户或作业角色）可用于工作的时间。 </p> 
   <p>Workfront使用多个字段计算用户可用性，具体取决于资源管理首选项在您的系统中的设置。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>. </p>
   <p>有关资源可用性的更多信息，请参阅 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">资源管理入门</a></p>
   或者，“能力”也用于指资源可用性。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>[!UICONTROL项目更新]类型之一。 这将在夜间重新计算流程运行时重新计算预计时间轴和计划时间轴。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>“一切照常”的工作，有助于运行日常的主要业务目标。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL积压工作]</td> 
   <td>在灵活环境中，新问题会一直保留到准备处理为止的区域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL基线]</td> 
   <td>用于在灵活环境中测量迭代的数据源。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL账单记录]</td> 
   <td> <p>记录可开单的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">创建帐单记录</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>帐单记录状态</td> 
   <td> <p>在“开单记录”或“小时”报表中，开单记录的状态指示开单记录是否已开单。 您无法删除与已计费账单记录关联的项目或编辑时间。 有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >创建帐单记录</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL品牌策略]</td> 
   <td>定制过程 [!DNL Workfront] 使界面具有与您的公司相似的外观，使用您的颜色和徽标。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL痕迹导航]</td> 
   <td> <p>页面顶部的区域，显示用户在应用程序中的分层位置。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">有关更多信息，请参阅 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">痕迹导航概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL预算状态]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与某个功能相关 [!DNL Workfront] 已删除，且无法更新字段。 </p> <p>此字段显示项目是否已添加到[!UICONTROL Capacity Planner]中，以及是否已为其完成预算计算。 [!UICONTROL Capacity Planner]已从 [!DNL Workfront]. </p> 
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
   <td>[!UICONTROL预算完成日期]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与某个功能相关 [!DNL Workfront] 已删除。 无法更新此字段。 </p>
   <p> 此字段仍在[!UICONTROL项目]和[!UICONTROL tasks]报表和列表中可见。</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL预算成本]</td>

<td> <p>这是与项目预算资源关联的成本。 </p>
   <p>该字段显示在 [!DNL Workfront] 名称如下：</p>
   <ul>
   <li><strong>[!UICONTROL预算成本]</strong>:在[!UICONTROL业务案例摘要]面板中</li>
   <li><strong>[!UICONTROL成本]</strong>:在[!UICONTROL Cost]查看信息时显示在[!UICONTROL Utilization]区域</li>
   <li><strong>[!UICONTROL项目预算成本]</strong>:在列表和报表中</li>
   </ul>   
    <p>项目的[!UICONTROL预算成本]使用以下公式计算：</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>有关计算[!UICONTROL预算成本]并在 [!DNL Workfront]，请参阅 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">计算项目预算成本</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL预算小时数]</td> 
   <td> <p>为项目所需完成的工作的资源编入预算的小时数。 此字段是指在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域（或在[!UICONTROL Resource Planner]中）为项目或项目资源编入预算的小时数。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">了解项目的[!UICONTROL预算人工成本]和[!UICONTROL预算工时]</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> 有关在 [!DNL Resource Planner]，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">预算资源 [!DNL Resource Planner] 使用[!UICONTROL Project]和[!UICONTROL Role]视图</a>. </p> 
    <p>在[!UICONTROL Business Case]或[!UICONTROL Resource Planner]的[!UICONTROL Budgeting]区域预算的小时数显示在以下区域： [!DNL Workfront] 名称如下：</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL预算小时数]显示名称</strong></td> 
        <td><strong>区域 [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL小时数]</td> 
        <td>[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Hours]查看的[!UICONTROL Resource Planner]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL预算小时数]</td> 
        <td> <p>利用率报表[!UICONTROL小时数]视图</p> <p>有关[!UICONTROL Utilization]报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL Resource Utilization]报表概述</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. 小时]</td> 
        <td> <p>[!UICONTROL预算小时]报表</p><p>“已编入预算的小时”报表中的[!UICONTROL已编入预算的小时]对象引用与已弃用的资源管理工具相关的信息。 仅“[!UICONTROL Bud”。 此报表中的“小时”字段是指在[!UICONTROL Resource Planner]或项目[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域预算的小时数。 </p> <p>有关创建报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL资源计划员预算小时数] </td> 
        <td> <p>可在以下报表中找到：</p>
        <ul>
        <li>[!UICONTROL项目]报表
        <li>[!UICONTROL项目（财务数据）]报表
        <li>[!UICONTROL任务]报表
        <li>[!UICONTROL问题]报表
        <li>[!UICONTROL预算小时]报表</li>
        </ul>
         <p>有关创建报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>在 [!DNL Adobe Workfront] 是指使用已从Workfront中删除的已弃用功能编入预算的小时数。 这些是仅查看字段，在使用当前资源预算工具时，不会使用当前信息进行更新。 </p>
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
   <td>[!UICONTROL预算的人工成本]</td> 
   <td> <p>这是与您（作为资源经理）在项目中完成任务职责所需工作的预算相关的小时数成本。 </p> <p>项目报表中的[!UICONTROL预算人工成本]使用以下公式计算：</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>此字段可能指：</p> 
    <ul> 
     <li> <p>在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域或[!UICONTROL Resource Planner]中显示与项目中的任务职责成本关联的人工成本。 有关计算[!UICONTROL预算人工成本]的信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL了解项目的预算人工成本]和[!UICONTROL预算工时]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域中显示的人工成本，反映在与项目关联的方案中的[!UICONTROL People Costs](从 [!DNL Scenario Planner] 在您使用方案计划员来预算项目资源时。 有关计划的信息，请参阅 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">方案规划器中的方案概述</a>. </p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>. </p> </li> 
     <p>它会在的以下区域中以以下名称显示：</p>
   <ul>
   <li><strong>[!UICONTROL预算的人工成本]</strong>:（在[!UICONTROL Business Case]的[!UICONTROL Resource Budgeting]区域中）。
   <li><strong>[!UICONTROL预算成本]</strong>:在[!UICONTROL Utilization]报表[!UICONTROL Cost]视图中
   <p>有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">查看资源利用信息 </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>:在 [!DNL Resource Planner] 项目或 [!DNL Role] 查看次数，按成本查看时
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>:在以下报表中： 
   <ul>
    <li>[!UICONTROL项目]报表</li>
    <li>[!UICONTROL项目（财务数据）]报表</li>
    <li>[!UICONTROL任务]报表</li>
    <li>[!UICONTROL问题]报表</li>
    <li>[!UICONTROL预算小时]报表</li> 
    </ul>
    <p>有关创建报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p>
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
   <td>[!UICONTROL预算的开始日期]</td> 
  <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与某个功能相关 [!DNL Workfront] 已删除。 无法更新此字段。</p>
  <p>这些区域已从 [!DNL Workfront]. </p> 
  <p>该字段仍显示在[!UICONTROL项目]和[!UICONTROL任务]报表和列表中。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL燃耗图]</td> 
   <td>折线图，可直观地表示已完成和剩余的工作。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>一个用于评估项目是否应从[!UICONTROL Idea]状态移至[!UICONTROL Planning]状态的工具。 换言之，[!UICONTROL业务案例]可帮助组织确定启动和完成项目是否值得，尤其是在将项目与产品组合中的其他项目进行比较时。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">为项目创建[!UICONTROL Business Case] </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL商业案例预算小时数]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与某个功能相关 [!DNL Workfront] 已删除。 无法更新此字段。</p> <p>此字段仍显示在项目和[!UICONTROL任务]列表和报表中。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计算分配]</td> 
   <td> <p>任务[!UICONTROL持续时间]类型之一。 这将根据任务的[!UICONTROL持续时间]和[!UICONTROL需要工作]计算分配给任务的用户在8小时工作日中分配给任务的百分比。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[!UICONTROL持续时间]和[!UICONTROL持续时间类型]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计算工作]</td> 
   <td> <p>任务[!UICONTROL持续时间类型]中的一项。 这将计算任务的[!UICONTROL Required]，假定[!UICONTROL Duration]和用户[!UICONTROL Assignment]百分比（基于8小时工作日）。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[!UICONTROL持续时间]和[!UICONTROL持续时间类型]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL日历]</td> 
   <td> <p>在 [!DNL Workfront]:[!UICONTROL主日历]和日历报表。</p> <p>[!UICONTROL主日历]是一个个人日历，它允许用户根据其在 [!DNL Workfront]. 用户还可以将他们的[!UICONTROL Home Calendar]与 [!DNL Outlook] ([!DNL Google] 和 [!DNL Microsoft] 集成)。 </p> <p>有关[!UICONTROL主日历]的更多信息，请参阅 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL主页日历]视图</a>.</p> <p>日历报表是一个动态报表，用户可以在其中查看事件的日期和其他重要详细信息，包括到期日期、工作状态以及将事件分配给的用户。</p> <p> 有关日历报表的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">日历报表概述</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL可以开始]</td> 
   <td> <p>此字段指示任务是否已准备好开始处理。 如果已准备好在任务的[!UICONTROL Can Start]字段中处理开始，则会将该任务设置为[!UICONTROL True]。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">任务的“[!UICONTROL Can Start]”概述</a>.</p> 
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
   <td> <p>[!UICONTROL类别]</p> </td> 
   <td> <p>类别是自定义表单。 您可以为此对象生成报表，也可以在其他对象报表中显示该报表。 并非所有对象都可以具有自定义表单或类别。 以下对象可以具有自定义表单： <br></p> 
    <ul> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL任务]</li> 
     <li>[!UICONTROL问题]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL费用]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL用户]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL类别名称]</td> 
   <td> <p>作为列添加到以下任何对象的视图时，它会显示与这些对象关联的所有自定义表单的列表：</p> 
    <ul> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL任务]<br></li> 
     <li>[!UICONTROL问题]<br></li> 
     <li>[!UICONTROLPortfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL费用]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL用户]<br></li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>一个实践领域，其重点是定义、了解和调整计划工作以适应范围、计划、成本和资源因素的变化。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL更改顺序]</td> 
   <td>针对项目提出的问题类型，该项目概述了对商定范围所要求的更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL仅更改]</td> 
   <td>项目[!UICONTROL更新类型]之一。 当对项目或任务执行任务更新或编辑时，它只会更新[!UICONTROL Project Projected]和[!UICONTROL Planeded]时间轴。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更改顺序]</td> 
   <td> <p>[!UICONTROL问题]的一种类型，通常指示在项目完成之前必须完成计划外工作量。</p> <p>有关[!UICONTROL问题]类型的更多信息，请参阅文章中的“默认问题类型”部分 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">自定义默认问题类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子任务]</td> 
   <td>任务是[!UICONTROL父任务]（[!UICONTROL摘要任务]）的[!UICONTROL子任务]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子项]</td> 
   <td>[!UICONTROL子任务]到[!UICONTROL父任务]（[!UICONTROL摘要任务]）的集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching]和[!UICONTROL Training]</td> 
   <td>学习模块、认证、标准或实践社区。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>一种通信工具，用于用户对任务交付件设定期望。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL提交日期]</td> 
   <td>一种通信工具，用于围绕任务交付项设置期望值。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication]和[!UICONTROL Reporting]</td> 
   <td>用于审查项目、项目或项目组合的例外和运行状况的标准</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL公司]</td> 
   <td> <p>[!UICONTROL公司]是 [!DNL Workfront]. </p> 
   <p> 您可以将用户或项目与一个公司关联。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">创建和编辑公司</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日期]</td> 
   <td> <p>项目、任务或问题设置为完成的日期。 中的[!UICONTROL完成日期]有多种类型 [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL实际完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">项目[!UICONTROL实际完成日期]概述 </a>.</li> 
     <li>[!UICONTROL计划完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">设置项目[!UICONTROL计划完成日期]</a> 和 <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务[!UICONTROL计划完成日期]概述</a>.</li> 
     <li>[!UICONTROL预计完成日期]。 有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的[!UICONTROL预计完成日期]概述</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成日]</td> 
   <td>相对于[!UICONTROL模板]的开始，[!UICONTROL模板任务]或[!UICONTROL模板]应该已完成的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成模式]</td> 
   <td> <p>这表示项目将如何标记为[!UICONTROL Complete]。 它可以有两个值：</p> 
    <ul> 
     <li>[!UICONTROL Manual]:用户必须将项目状态更改为[!UICONTROL Complete]。</li> 
     <li>[!UICONTROL Automatic]（自动）：当项目中的所有任务完成100%且所有问题都结束时，项目状态将自动更改为[!UICONTROL完成]。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL条件]</td> 
   <td> <p>这是任务、问题或项目进度的直观表示形式。</p> <p>对于项目，条件可由项目所有者手动设置，也可以由 [!DNL Workfront]，基于项目的进度状态。 </p> <p>项目条件的可能值为：</p> 
    <ul> 
     <li>[!Uicontrol On Target]</li> 
     <li>[!UICONTROL面临风险]</li> 
     <li>[!UICONTROL遇到问题]</li> 
    </ul> <p>有关项目条件的更多信息，请参阅文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL项目条件]和[!UICONTROL条件类型]概述</a>.</p>
     <p>您可以将任务和问题条件与可在报表中显示的数字相关联。 以下列表显示任务和问题条件的默认名称和编号。 您的系统管理员可以更新条件的名称，并且他们可以添加具有不同编号的新条件。 在某个数字与某个条件关联后，便无法对其进行编辑。  </p> 
     <p>对于任务，条件由任务所有者手动设置。 任务条件的可能值为：</p> 
    <ul> 
     <li>[!UICONTROL顺利运行](0)<br></li> 
     <li> [!UICONTROL一些注意事项](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> <p>有关任务条件的详细信息，请参阅文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">为任务和问题更新[!UICONTROL条件]</a>.</p> <p>对于问题，条件由问题所有者手动设置。 问题条件的可能值为：<br></p> 
    <ul> 
     <li>[!UICONTROL顺利运行](0)<br></li> 
     <li>[!UICONTROL一些注意事项](1)<br></li> 
     <li>[!UICONTROL主要路障](2)</li> 
    </ul> 
   <p><b>注释</b></p>
    <p>在[!UICONTROL日记帐分录]报表中跟踪[!UICONTROL条件]字段时，[!UICONTROL New]和[!UICONTROL旧数值]会显示与该条件关联的数字，而不是其名称。 如果最初没有为任务或问题定义条件，稍后又更新该条件，则捕获该更新的日记帐分录将显示[!UICONTROL Condition]字段的[!UICONTROL Old Number Value](-2,147,483,648)。 另请参阅本文中的“[!UICONTROL New Number Value]”、“[!UICONTROL Old Number Value]”和“[!UICONTROL Journal Entry]”。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL条件更新]</td> 
   <td> <p>此字段显示任务、项目或问题的当前状态。 此选项显示任务、项目或问题所有者在[!UICONTROL更新状态]字段中提供的最新更新，以及新条件。</p> <p>对条件更新所做的注释不会显示在[!UICONTROL条件更新]列中；只显示主更新。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL约束日期]</td> 
   <td> <p>如果您使用的[!UICONTROL任务约束]与特定日期（如[!UICONTROL必须从开始]）绑定，则该特定日期将变为任务的[!UICONTROL约束日期]。</p> <p>以下任务约束更新了[!UICONTROL约束日期]字段：</p> 
    <ul> 
     <li>[!UICONTROL必须开始]</li> 
     <li>[!UICONTROL必须在]完成</li> 
     <li>[!UICONTROL开始时间不晚于]</li> 
     <li>[!UICONTROL开始时间不早于]</li> 
    </ul> <p>提示：   
     <ul> 
      <li> <p>具有[!UICONTROL Constraint]的[!UICONTROL Fixed Dates]的任务没有[!UICONTROL Constraint Date]。 </p> </li> 
      <li> <p> [!UICONTROL约束日期]只能在报表或自定义视图中查看。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL约束日]</td> 
   <td> <p>如果在与特定日期（如必须开始）关联的模板任务中使用任务约束，则该特定日期将成为模板任务的约束日。</p> <p>以下任务约束更新了[!UICONTROL Constraint Day]字段：</p> 
    <ul> 
     <li>[!UICONTROL必须开始]</li> 
     <li>[!UICONTROL必须在]完成</li> 
     <li>[!UICONTROL开始时间不晚于]</li> 
     <li>[!UICONTROL开始时间不早于]</li> 
    </ul> <p>提示：[!UICONTROL Constraint Day]只能在报表或自定义视图中查看。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL约束类型]</td> 
   <td> <p>任务的计划趋势。 例如，[!UICONTROL As Op Hop Ach Invest Op Than]将安排一项任务尽快开始，而[!UICONTROL Finish No Beat Than]将安排一项任务在[!UICONTROL Constraint Date]之前完成，不晚于[!UICONTROL Constraint Date]。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL任务约束]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上下文菜单]</td> 
   <td>位于屏幕左侧的菜单，项目会在该菜单上更改为与活动内容关联。 例如，当用户查看项目时，[!UICONTROL上下文菜单]将显示指向项目相关信息和工具的链接。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已转换的问题创作者]</td> 
   <td>项目或任务报表中的字段，用于在将问题转换为项目或任务时显示与问题的[!UICONTROL主要联系人]用户相关的信息。 该字段还显示在[!UICONTROL项目详细信息]部分，其中显示已转换问题的[!UICONTROL主要联系人]的名称。 另请参阅本文中的“[!UICONTROL Primary Contact]”。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL成本]</td> 
   <td> <p>完成项目、任务或问题时必须花费的货币金额。 </p> <p>您可以跟踪与项目相关的各种类型的人工成本、费用和风险。有关跟踪 [!DNL Workfront] 请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟踪成本</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL成本类型]</td> 
   <td>对于任务，[!UICONTROL成本类型]确定任务将如何应计成本。 一些示例包括[!UICONTROL Fixed Horly]、[!UICONTROL User Horly]和[!UICONTROL User Horly加Fixed]。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL跨项目依赖项]</td> 
   <td> <p>一个项目的任务取决于来自其他项目的任务。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">创建跨项目前置项</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL自定义数据]</td> 
   <td> <p>组织特有的数据。 组织可以自定义 [!DNL Workfront] 应用程序时，需创建自定义表单和自定义字段。 此自定义信息可推动报告KPI、审核和需求组合。 </p> <p>[!UICONTROL Custom Data]可以链接到：</p> 
    <ul> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL任务]</li> 
     <li>[!UICONTROL用户]</li> 
     <li>[!UICONTROL公司]</li> 
     <li>[!UICONTROL问题]</li> 
     <li>[!UICONTROL文档]</li> 
     <li>[!UICONTROL费用]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程序]</li> 
     <li>[!UICONTROL迭代]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义数据类型]</td> 
   <td>用于指定[!UICONTROL Custom Data]字段是否以文本、日期、数字或货币形式存储在数据库中的选项。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义显示类型]</td> 
   <td>自定义字段的字段显示类型。 示例包括[!UICONTROL下拉列表]、[!UICONTROL文本字段]、[!UICONTROL文本区域]、[!UICONTROL单选按钮]等。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义字段]</td> 
   <td>对于允许用户从多个选项中进行选择的自定义数据，这些值是用户可以从中进行选择的值。 自定义选项仅在[!UICONTROL下拉列表]、[!UICONTROL多选下拉列表]、[!UICONTROL单选按钮]和[!UICONTROL复选框]中有效。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义表单标签]</td> 
   <td>使用包含自定义选项的自定义显示类型时，这是将在下拉菜单、复选框或该自定义选项的单选按钮中显示的用户界面文本。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义值]</td> 
   <td>使用具有自定义选项的自定义字段时，此值将存储在特定选项的数据库中。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL自定义视图]</td> 
   <td>为列表中每个对象显示的数据字段或列的定义。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL客户]</td> 
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
   <td>[!UICONTROL功能板]</td> 
   <td> <p> 您可以在报表或报表对象列表中添加此字段，以显示报表在列表中列出的功能板。 </p> <p> 您还可以使用此字段过滤特定功能板上列出的报表。 </p> <p> 有关在报表对象报表中包含功能板信息的更多信息，请参阅文章中的“了解功能板中列出的报表”部分 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">访问和组织报告</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL数据类型]</td> 
   <td>请参阅“[!UICONTROL自定义数据类型]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL延迟天数]</td> 
   <td> <p>如果缺少[!UICONTROL实际完成日期]，此字段将显示[!UICONTROL计划开始]和[!UICONTROL今天]之间的日期差。</p> <p>此外，还显示[!UICONTROL Actual Completion]和[!UICONTROL Planed Completion]（当存在[!UICONTROL Actual Completion Date]）之间的日期差。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL默认计划]</td> 
   <td> <p>要分配给组织内的用户和项目的自定义默认工作时间。 </p> <p>计划用于计算分配给用户的任务的计划日期、开始日期和完成日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL可交付项]</td> 
   <td>在项目完成时必须提供的可量化货物或服务。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>对摄取过程进行评分和确定优先级。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL部门目标]</td> 
   <td>特定部门特有的目标，该部门重点改进部门内的运营量度。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依赖项]</td> 
   <td>需要一个任务更改状态才能另一个任务更改状态的两个任务之间的链接。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL依赖项类型]</td> 
   <td> <p>任务与其前身之间的计划关系类型。 例如[!UICONTROL Finish-Start]，它要求第一个任务必须完成，然后第二个任务才能开始。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">任务依赖关系类型概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>附加到 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文档版本]</td> 
   <td> <p>每次将同一文档上传到同一对象时，都会为其分配版本号。 用户可以查看和更改文档以前版本的多个选项。</p> <p>有关更多信息，请参阅 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">管理文档版本</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持续时间]</td> 
   <td> <p>为完成任务问题或项目分配的时间范围（由[!UICONTROL计划开始]和计划完成之间的天数确定）。</p> 
    <ul> 
     <li>对于任务，如果任务的持续时间类型不是简单，则持续时间是可编辑的字段。 如果任务的持续时间类型为“简单”，或者如果任务约束为“固定日期”，则持续时间是由Workfront执行的计算。</li> 
     <li>对于问题，持续时间始终是可编辑的字段，它应表示需要解决问题的估计天数。</li> 
     <li>对于项目，持续时间是由 [!DNL Workfront] 它表示最早任务的计划起始时间与项目上最新任务的[!UICONTROL计划完成时间]之间的天数差。</li> 
    </ul> <p>有关任务的[!UICONTROL持续时间]与[!UICONTROL计划持续时间]之间差异的详细信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">任务的[!UICONTROL计划持续时间]与[!UICONTROL持续时间]之间的差异</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL持续时间（以分钟为单位）]</td> 
   <td>此字段显示的信息与[!UICONTROL Duration]字段（以分钟而不是天为单位）的信息相同。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL每次发生的持续时间]</td> 
   <td> <p>它显示在循环任务父项的[!UICONTROL任务详细信息]和[!UICONTROL编辑任务]框中。 它显示每个定期任务的持续时间。 有关创建定期任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建定期任务</a>. </p> <p> <span>在单个定期任务中修改的持续时间不会显示此字段中指示的值。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL持续时间类型]</td> 
   <td> <p>一个任务字段，指示完成任务所需的工作如何在任务持续时间内分配给受分配者。 它表示任务的[!UICONTROL持续时间]与[!UICONTROL Work Required]与时间量之间的关系，或[!UICONTROL Allocation]（分配的资源应花费在任务上以完成它）。 </p> <p>此字段显示在任务的[!UICONTROL详细信息]选项卡上。 </p> <p>选项包括：</p> 
    <ul> 
     <li>[!UICONTROL计算分配]</li> 
     <li>[!UICONTROL计算工作]</li> 
     <li>[!UICONTROL工作驱动]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[!UICONTROL持续时间]和[!UICONTROL持续时间类型]概述</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL持续时间单位]</td> 
   <td>用于测量电源搜索中时间的单位。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作驱动]</td> 
   <td>用户数量与任务完成所花费的时间之间的关系。 添加更多用户后，计划完成任务的总时间会减少，但任务的持续时间保持不变。 例如，如果任务在炮击一桶花生，则增加更多人将减少计划的时间，但人员日的持续时间将保持不变。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已用时间]</td> 
   <td> <p>[!UICONTROL Elapsed time]是任务的[!UICONTROL Duration]的时间单位。 它介于任务的[!UICONTROL计划开始日期]和[!UICONTROL计划完成日期]之间的时间（包括假日、周末和休息时间）。 换言之，已用时间即为日历日的过去。 </p> <p>[!DNL Workfront] 在任务持续时间中支持以下已用时间单位：</p> 
    <ul> 
     <li> <p>[!UICONTROL已用分钟数]</p> </li> 
     <li> <p>[!UICONTROL已用小时数]</p> </li> 
     <li> <p>[!UICONTROL已用天数]</p> </li> 
     <li> <p>[!UICONTROL已用周]</p> </li> 
     <li> <p>[!UICONTROL已用月份]</p> </li> 
    </ul> <p>有关任务持续时间（包括已用时间）的详细信息，请参阅 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[!UICONTROL持续时间]和[!UICONTROL持续时间类型]概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL结束日期]</td> 
   <td> <p> 在[!UICONTROL费率]报表中，这是项目层职务角色的新开单费率结束的日期。 在此日期之前与项目关联的小时数乘以此开单费率，以计算项目收入。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>[!UICONTROL工作绩效指标](WPI)，指示对任务、项目、团队或组织的承诺和信念何时减弱。 这表明，您需要采取行动来恢复这种信念和承诺。 WPI会通过问一些简单的问题来衡量， “你理解你的期望吗？ 您分配的工作是否对组织有影响？ 你做得好吗？”</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>跨职能目标，有助于公司目标的量度。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>项目或任务中的任何更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件处理程序]</td> 
   <td>发生事件时发生的自动任务。 一个常见的示例是自动电子邮件通知。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL事件通知]</td> 
   <td>从事件处理程序生成的电子邮件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL费用]</td> 
   <td>任务或项目的非人工成本。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>通常是许可证类型或具有此许可证的用户，此类用户只能查看系统中的信息。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL External System]</td> 
   <td>在指定的记录系统之外存储和管理的任何服务或软件。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL过滤器]</td> 
   <td> <p>报表或列表元素的主要构建基块之一，用于定义在屏幕上显示的信息。 有关报表元素的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报表元素：过滤器、视图和分组</a>.</p> <p>过滤器可确定在报表或 [!DNL Workfront] 面板列表，如项目、任务或问题。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>在 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定成本]</td> 
   <td>您可以为项目定义固定成本金额。 这是项目的[!UICONTROL计划成本]的一部分，它表示完成项目所需的资金量。 有关成本的信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">跟踪成本</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL固定收入]</td> 
   <td>您可以为项目定义固定的收入额。 这是项目的[!UICONTROL计划收入]的一部分，它表示在完成项目时您可能获得的金额。 有关收入的信息，请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL标记]</td> 
   <td> <p> 此字段与[!UICONTROL状态图标]相同，但仅适用于以下视图： </p> 
    <ul> 
     <li> [!UICONTROL模板] </li> 
     <li> [!UICONTROL费用] </li> 
    </ul> <p> 有关更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹]</td> 
   <td>文件夹用于组织与对象关联的文档或报表。</td> </tr>
  <tr>
  <td>FTE（相当于全职）</td> 
   <td>这是“等效全时”，用于指示资源可用于工作的时间。 
   FTE字段显示在以下区域： 
  <ul>
   <li> 编辑或创建用户时的用户配置文件 </li>
   <li> 资源规划程序 </li>
   <li> 方案计划员(需要为Workfront方案计划员提供附加许可证) </li>
   <li> 用户列表和报表 </li> </ul>

<p>FTE必须是最多1的小数，并且不能是0。 </p>
   <p> FTE为1（如用户配置文件中所定义，此为用户FTE字段的默认值）表示资源（用户或角色）根据计算其可用性的计划计算整个小时数。 </p>
   <p>您的Workfront管理员可决定将哪个计划用于确定用户的可用性。  </p>
   <ul>
   <li> 使用默认计划时，Workfront会使用其配置文件中找到的用户的FTE来计算可用性。 </li>
   <li> 使用用户计划时，Workfront会使用用户的休息时间， <span class="preview">工作时间值</span>和默认计划的小时数来计算用户的FTE。 </li> </ul>

<p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">配置资源管理首选项</a>.  </p>
   <p>有关在Workfront中创建计划的更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">创建计划</a>. </p>

<p><b>注释</b></p>
   <p>对于方案计划器中的所有计算，Workfront会使用以下值：1个FTE = 8小时。</p>
   <p>有关更多信息，请参阅 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">方案规划器入门</a>. </p>
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
   <td>[!UICONTROL甘特图]</td> 
   <td> <p>在日历视图中，项目日期的可视时间轴基于当前计划项目任务的计划日期或预计日期。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目标]</td> 
   <td><p>中有两个目标概念 [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>项目目标</b>:由项目相关利益相关方商定的一组业务目标。 项目目标是项目业务案例的一部分。 </p> <p>您不能在列表或报表中显示项目目标，但可以通过API访问它们。 </p> <p>有关业务案例项目目标的信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">创建业务案例目标 </a>. </p> </li> 
     <li> <p><b>战略目标</b>:战略目标是您创建的目标，用于在特定时间段内规划工作策略。 您可以使用 [!DNL Workfront Goals]. 贵组织必须购买额外的许可证，您必须有权访问此功能才能创建战略目标。 [!DNL Workfront Goals] 仅在附加许可证的情况下可用。</p> 
     <p>有关更多信息，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </p> 
     <p>您可以在目标或项目报表中显示战略目标，并通过API访问这些目标。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目标层次结构]</td> 
   <td> <p>在[!UICONTROL目标]和[!UICONTROL项目]报表中，这是一个收集字段，用于在战略目标与其他目标保持一致时，在层次结构中显示该目标所属的目标。 目标由▸分隔符分隔。 </p> <p>此字段中仅显示目标和目标的父项。 不显示子项目标。 </p> <p>有关在 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">中的目标协调概述 [!DNL Workfront Goals]</a>. </p> 
   <p>仅当贵组织已购买时，此字段才可见 [!DNL Workfront Goals]. 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL目标成功得分]</td> 
   <td> 在[!UICONTROL项目报表]中，此字段用于引用与[!UICONTROL Business]案例关联的项目级别目标。 目前，这是已弃用的字段，与任何功能都不相关。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL目标] </td> 
   <td> <p>在[!UICONTROL项目]报表中，这是一个收集字段，用于显示与项目关联的所有战略目标。 目标之间用逗号分隔。</p> <p>仅当贵组织已购买时，此字段才可见 [!DNL Workfront Goals]. 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. 有关 [!DNL Workfront]，请参阅本文中的“[!UICONTROL目标]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL全局界面首选项]</td> 
   <td>影响所有用户的界面设置。 [!UICONTROL Global Interface Preferences]可被[!UICONTROL User Interface Preferences]覆盖。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL组]</td> 
   <td> <p>有权访问相同对象的用户集合（可能来自同一部门或业务部门）。 除了用户之外，群组还可以与项目组合、项目、<span> 项目模板，</span> 公司、团队、计划、布局模板和时间表配置文件。</p> <p>您还可以按组授予对象的权限。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">群组概述</a>.</p> <p>在以下类型之一的对象列表或报表中，您可以使用[!UICONTROL Group]字段列出与特定组关联的该类型对象：用户，组合，项目，项目， <span>项目模板</span>、公司、团队、计划、布局模板或时间表配置文件。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL组管理员]</td> 
   <td> <p>管理指定用户组的对象、访问权限和用户的用户。</p> <p> 在[!UICONTROL组]报表中，此字段显示组中指定为[!UICONTROL组管理员]的用户的名称。 有关组管理员的详细信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[！具有管理访问权限的UICONTROL组]</td> 
   <td> <p> 在[!UICONTROL布局模板]、[!UICONTROL时间表配置文件]或[!UICONTROL计划报表]中，此字段显示组管理员有权修改模板的组。 您也可以按此字段过滤此报表。 </p> <p> 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">创建和管理布局模板</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL分组]</td> 
   <td> <p>用于按通用标准对列表中的信息进行分类的报告元素。</p> <p>有关更多信息，请参阅文章中的“[!UICONTROL分组]”部分 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">报表元素：过滤器、视图和分组</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL切换日期]</td> 
   <td> <p>任务可用于工作的日期。 [!UICONTROL切换日期]是一种计算方式，不能手动设置。 <br>有关[!UICONTROL切换日期]的更多信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL任务切换日期]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL帮助台]</td> 
   <td>部分 [!DNL Workfront] 包含所有问题队列。 [!UICONTROL Help Desk]可用于处理客户支持票证、项目请求、帮助台票证等。 这与[!UICONTROL请求]区域相同。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL所有者]</td> 
   <td>在[!UICONTROL Hour]报表中，[!UICONTROL Owner]是将小时归因到的用户。 这与实际记录时间的用户不同。 这两个实体有时可以是两个不同的用户。 <br>有关为其他用户记录时间的更多信息，请参阅文章 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">日志时间</a>.</td> 
  </tr>

<tr> 
   <td>小时状态</td> 
   <td> <p>由Workfront为用户记录任务、问题或项目的实际小时数设置的属性。 </p>

小时条目在Workfront中可以具有以下状态之一：
<ul>
   <li><b>已提交</b>:已记录项目、任务或问题的小时数。 它们是账单记录的一部分或尚未添加到账单记录中。</li>
   <li><b>已批准</b>:已记录这些小时数，且已获得项目所有者的批准。 它们是账单记录的一部分或尚未添加到账单记录中。</li> 
   <li><b>未批准</b>:项目所有者已记录并拒绝这些小时。 它们是账单记录的一部分或尚未添加到账单记录中。</li>
   <li><b>已计费</b>:小时已记录，已添加到账单记录中，并且账单记录状态已标记为已开单。 它们不需要获得项目所有者的批准。</li>
   <li><b>已计费和已批准</b>:已记录并获得项目所有者的批准的小时数，并且帐单记录状态已标记为已开单。</li>
   </ul>


<p>当小时是计费记录的一部分时，“小时状态”指示小时是否已批准，或者它们所属的计费记录是否已计费。 小时条目的小时状态仅在小时列表或报表中可见。 </p>

<p>有关向帐单记录添加小时数的更多信息，请参阅文章中的“向帐单记录添加小时数”一节 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >创建帐单记录</a>.</p>

<p>有关批准项目时间的更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >需要时间来批准项目</a>.</p>

<p><b>笔尖</b></p>

<p>未直接登录工作项的常规小时数不显示“小时”状态。 </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL小时类型]</td> 
   <td> <p>可为用户记录任务、问题或项目的实际小时数设置的属性。 这也是未直接链接到工作的记录小时数的一个属性，如[!UICONTROL Vacation]和[!UICONTROL Time Off]。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">管理小时类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID是与中的每个对象关联的字母数字指示器 [!DNL Workfront]. 它唯一标识 [!DNL Workfront] 数据库。 您可以查看报表中任何对象的ID或每个对象的列表。 </p> <p>提示：   <p>您还可以在对象页面的URL中查看ID。 例如，当您访问[!UICONTROL项目详细信息]页面时，项目的ID可能与以下URL中列出的数字类似：</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>个人目标，这些目标对团队目标的指标有贡献，但与个人或职业发展无关。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL继承访问]</td> 
   <td>允许访问从对象传播到另一个对象的共享函数。 例如，项目用户继承在项目群和项目组合记录中定义的访问权限。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>在 [!DNL Workfront Scenario Planner]，您可以将计划划分为多个计划，以便更轻松地管理计划。 <span>您可以构建一个[!UICONTROL Initiative]报表，并可以在[!UICONTROL Project]报表中访问[!UICONTROL Initiative]信息。</span></p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>. </p> <p>的 [!DNL Initiative] 报表在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。 您无法通过API访问[!UICONTROL计划]。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>[!UICONTROL方案任务职责]报表类型显示有关与 [!DNL Workfront Scenario Planner].</span> </p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>. </p> <p><span>此报表类型在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative作业角色小时数]</span> </td> 
   <td> <p><span> 在[!UICONTROL方案作业角色]报表中，此报表显示与方案中的作业角色关联的小时数。</span> </p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>. </p> <p>此字段和[!UICONTROL Initiative Job Role]报表类型在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative作业角色计数]</td> 
   <td> <p>在[!UICONTROL方案作业角色]报表中，此报表显示与方案关联的特定作业角色的数量。</p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>. </p> <p>此字段和[!UICONTROL Initiative Job Role]报表类型在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划上次发布日期]</td> 
   <td> <p>[!UICONTROL方案]、[!UICONTROL方案作业角色]和[!UICONTROL项目]报表中的字段，用于显示计划方案上次发布到项目的日期。 您可以发布计划以创建项目或更新与计划关联的项目。</p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>. </p> <p><span>有关发布计划的信息，请参阅</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">发布方案以在 [!DNL Workfront Scenario Planner]</a>. 此字段在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL内联搜索]</td> 
   <td>在填写表单过程中执行搜索，以查找某个特定字段的可能条目。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL界面设置]</td> 
   <td>应用程序中用于定义自定义视图、过滤器、分组、列表控件等的区域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL是公司目标]</p></td> 
   <td> <p>在 [!DNL goal reports]，则会为每个战略目标显示“[!UICONTROL True]/ [!UICONTROL False]”值，以指示贵组织是否已分配给目标作为其所有者。 </p> 
   <p>仅当贵组织已购买时，此字段才可见 [!DNL Workfront Goals]. 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概述 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL问题]</td> 
   <td> <p>计划外工作项，通常指示存在阻止完成任务或项目的问题。 对它进行筛选和评估，以供进一步的工作考虑</p> <p>[!UICONTROL问题]也可以是[!UICONTROL帮助台]请求。 [!UICONTROL更改订单]、[!UICONTROL请求]和[!UICONTROL错误]也是[!UICONTROL问题]。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL问题管理]</td> 
   <td> <p>控制问题类型定义的流程和规则，以及与每种类型关联的路由、细分或流量流程。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL问题所有者]</td> 
   <td>负责筛选和完成问题的团队或用户。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL迭代]</td> 
   <td>一个时间段，在该时间段内，团队会生成一组预定义的交付件。</td> 
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
   <td>[!UICONTROL作业角色]</td> 
   <td> <p>用于标识用户的日常工作职能和职责。 可以为工作项分配职务角色，以确定完成工作过程所需的技能，而无需将其分配给特定用户。 </p> <p>用户可以拥有多个角色。 例如，图形设计人员或顾问。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL日记帐分录]</p> </td> 
   <td> <p>一个可报告对象，用于告知有关项目、任务、问题和其他对象的[!UICONTROL Updates]区域中显示的跟踪字段的系统更新信息。</p> <p>要了解更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">有关[!UICONTROL更新]区域的报告</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL看板标记]</td> 
   <td> <p>在[!UICONTROL任务]报表或[!UICONTROL问题]报表中，[!UICONTROL看板标志]字段显示在[!UICONTROL看板板]上文章中设置的标志状态。 可能的值包括[!Uicontrol On Track]、[!UICONTROL Ready To Pull]和[!UICONTROL Is Blocked]。</p> <p>有关在[!UICONTROL看板文章板]上设置文章标记状态的详细信息，请参阅文章 <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">在[!UICONTROL看板板]上的文章中使用标记</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>一个可衡量的价值，它表明公司如何有效地实现关键业务目标。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>在前置任务的[!UICONTROL计划完成日期]过后，必须经过的时间，直到从属任务开始。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL滞后类型]</td> 
   <td> <p>计算[!UICONTROL Lag]的方法。 它可以是：</p> 
    <ul> 
     <li>[!UICONTROL Days]（工作日）</li> 
     <li>[!UICONTROL日历天数]（忽略假日）</li> 
     <li>[!UICONTROL百分比]</li> 
     <li>[!UICONTROL每周时间]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">滞后类型概述</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL大缩略图]</td> 
   <td> <p> 在[!UICONTROL文档]列表或报表中，它以缩略图显示文档的预览。 </p> <p>选择 <strong>[!UICONTROL大缩略图]</strong> 查看报表中400像素范围的缩略图。</p> <p>当您修改列表或报表中列的宽度时，缩略图的大小会随之发生调整。</p> <p>另请参阅本文中的“[!UICONTROL Thumbnail]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最近10个查看器]</td> 
   <td> <p>在报表列表中，此字段显示最多10个最近查看了报表的用户的名称。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>此字段显示对象所有者上次在对象上输入的更新，这是所有者在对象上的最新活动或交互。</p> <p>的 [!DNL Last Condition Note] 列的空值。 当在对象上输入新注释时，该注释将成为最后一个注释，并再次显示在列中。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次财务更新日期]</td> 
   <td>在[!UICONTROL项目]报表中，此字段会捕获项目财务状况的上次计算和更新日期和时间。 有关项目财务的信息，请参阅 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">项目财务概述</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最后注释]</td> 
   <td> <p>此字段显示任何用户上次在对象上输入的更新。 这是对象上最近的活动或交互。</p> <p>如果删除了对象最后一个注释的文本，则[!UICONTROL Last Note]列为空。 当在对象上输入新注释时，该注释将成为最后一个注释，并再次显示在列中。</p>
   <p>将此字段添加到[!UICONTROL任务]报表后，子对象（如问题、子任务、文档等）上剩余的任何更新。  — 此列中不显示任务。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次查看者]</td> 
   <td> <p>在报表列表中，此字段显示有关上次查看报表的用户的信息。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上次查看日期]</td> 
   <td> <p>在报表列表中，此字段显示报表最后显示的日期。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL布局模板]</td> 
   <td>由系统管理员或组管理员定义，用于标识在给定用户工作区中显示的选项卡和报表。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL布局类型]</td> 
   <td>与[!UICONTROL自定义视图]一起，[!UICONTROL布局类型]指定[!UICONTROL自定义视图]的类型。 目前，只有列表可用。 将来，[!UICONTROL Detail]（对象的[!UICONTROL Detail]视图）可能会变得可用。</td> 
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
   <td>[!UICONTROL库任务]</td> 
   <td>单个任务的模板，用于在应用程序中提供[!UICONTROL Tasks]和[!UICONTROL Template Tasks]的一致命名。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL许可证类型]</td> 
   <td>分配给[!UICONTROL访问级别]的许可证类型。 它可以是[!UICONTROL Full User]、[!UICONTROL Limited User]或[!UICONTROL Requester]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL许可证限制计划]</td> 
   <td> <p>在[!UICONTROL Group]视图或报表中，此字段显示可分配给相应组被指定为其[!UICONTROL Home Group]的用户的[!UICONTROL Plan]许可证的最大数量。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL许可证限制工作]</td> 
   <td> <p>在[!UICONTROL组]视图或报表中，此字段显示可分配给将相应组指定为其[!UICONTROL主组]的用户的[!UICONTROL工作]许可证的最大数量。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL有限用户]</td> 
   <td>允许创建 [!DNL Access Level] 包含仅查看权限，且能够提交问题、输入注释和上传文档。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL列表控件]</td> 
   <td> <p>[!UICONTROL界面设置]的一部分，它允许将自定义过滤器、视图和分组关联到单个用户或全局关联到所有用户。</p> </td> 
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
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>[!UICONTROL项目]的[!UICONTROL更新类型]之一。 此设置允许仅在单击“[!UICONTROL重新计算的时间轴]”时更新[!UICONTROL Project Projected]和[!UICONTROL Planeded]时间轴。 在轻度重新计算过程和更新项目中的项目或任务期间，将忽略通过这种方式设置的项目。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目[!UICONTROL更新类型] </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>这是指当前已登录的用户。 </p> <p>我们建议在过滤器中使用此字段，以便在与其他用户共享报表时使报表更加通用。 这样，您就只能构建一个报表，该报表将根据登录者查看该报表的方式显示不同的信息，因为该信息始终为登录用户进行自定义。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL最大用户数]</td> 
   <td> <p>这是一个已弃用的字段。 此字段可能显示的任何信息都与某个功能相关 [!DNL Workfront] 已删除，且无法更新字段。 </p> <p>在以前的版本中 [!DNL Workfront]，您可以在创建或编辑作业角色时更新此字段。 它显示了每个项目上可以与角色关联的用户总数。 对于可以在项目中分配的无限数量的用户，允许值为零。 </p>该字段在某些报表和列表中仍可见，但显示的信息无法更新。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑]</td> 
   <td> <p>可以与任务关联的标记，用于指示任务完成后项目中的关键点已实现。 通常，您可以使用里程碑来显示重要事件，例如项目的某一阶段或一组关键活动的完成情况。 [!UICONTROL Milestones]通常与父任务关联。 必须先创建里程碑，然后才能将其附加到任务。 有关里程碑的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">创建里程碑路径</a> 和 <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">将里程碑与任务关联</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL里程碑路径]</td> 
   <td>[!UICONTROL里程碑]的集合。 [!UICONTROL里程碑路径]用于项目，以区分具有某些类型的[!UICONTROL里程碑]的项目和具有不同[!UICONTROL里程碑]集的项目。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL里程碑任务]</td> 
   <td>标记为指示要测量的可报告事件的任务。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL模块]</td> 
   <td>在 [!DNL Workfront Fusion] 功能（根据关联的应用程序执行某些功能）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的主要角色]</td> 
   <td> <p>当过滤器中引用该参数时，它会显示与登录用户具有相同[!UICONTROL主要角色]的用户，或分配给登录用户的[!UICONTROL主要角色]的工作项。</p> <p>我们建议在过滤器中使用此字段，以便在与其他用户共享报表时使报表更加通用。 这样，您就只能构建一个报表，该报表将根据登录者查看该报表的方式显示不同的信息，因为该信息始终为登录用户进行自定义。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL我的家庭团队]</td> 
   <td> <p>当过滤器中引用了该内容时，此字段会显示属于已登录用户的[!UICONTROL Home Team]的用户，或分配给已登录用户的[!UICONTROL Home Team]的工作项。 </p> <p>我们建议在过滤器中使用此字段，以便在与其他用户共享报表时使报表更加通用。 这样，您就只能构建一个报表，该报表将根据登录者查看该报表的方式显示不同的信息，因为该信息始终为登录用户进行自定义。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL命名约定]</td> 
   <td>组织范围的规则集，使用数据创建项目、任务和交付项的名称。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL本机集成]</td> 
   <td>无需手动编码或API配置的集成。 也称为“现成”集成。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL导航菜单]</td> 
   <td>应用程序的中心上方的面板，其中包含指向[!UICONTROL Workfront]主要区域的链接。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL新数字值]</td> 
   <td>在[!UICONTROL日记帐分录]报表中，此报表显示替换[!UICONTROL旧数值]的字段的更新值。
   有关更多信息，请参阅本文中的“[!UICONTROL旧数字值]”。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL非工作日]</td> 
   <td>未分配给完成任何分配的日期。 这通常是度假日、假期或周末。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注意]</td> 
   <td>对 [!DNL Workfront] 对象。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注释文本]</td> 
   <td> <p>这会显示用户在任何对象上输入的更新文本。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL链接目标的数量]</td> 
   <td> <p>在[!UICONTROL项目]报表中，这是与项目关联的战略目标数。 有关将项目与战略目标关联的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">将项目添加到  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>有关战略目标的信息，另请参阅本文中的“[!UICONTROL目标]”。</p> 
   <p>仅当贵组织已购买时，此字段才可见 [!DNL Workfront Goals]. 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">将项目添加到[!UICONTROL Adobe Workfront Goals]中的目标</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL对象]</td> 
   <td> <p>组织的工作项目和报表，以及在[!UICONTROL Workfront]中管理这些项目的用户组。 对象可以是：</p> 
    <ul> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程序]</li> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL任务]</li> 
     <li>[!UICONTROL问题]</li> 
     <li>[!UICONTROL文档]</li> 
     <li>[!UICONTROL功能板]</li> 
     <li>[!UICONTROL报表]</li> 
     <li>[!UICONTROL组]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL用户]</li> 
     <li>[!UICONTROL公司]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解[!UICONTROL Adobe Workfront]中的对象</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL对象类型]</td> 
   <td>如果创建包含所有自定义表单的报表或列表，则可以将此字段用作视图或过滤器，以查看哪些对象类型与每个表单相关联。 </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL旧数值]</td> 
   <td>在[!UICONTROL日记帐分录]报表中，此报表显示更新之前字段的原始值。 更新字段值后，该值将在[!UICONTROL日记帐分录]报表中显示为[!UICONTROL新数字值]。 有关更多信息，另请参阅“[!UICONTROL New Number Value]”。</td> 
  </tr>
  <tr> 
   <td>[！仅更改时UICONTROL]</td> 
   <td> <p>[!UICONTROL项目更新]类型之一。 选择此选项后，仅当对项目或项目中的任务进行更新或更改时，[!UICONTROL Project Projected]和[!UICONTROL Planeded]时间轴才会更新。 它不会每晚更新项目。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>在 [!DNL Workfront] 数据库，在文本模式报表或计算的自定义数据中使用。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>未完成但正在处理的问题或任务。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL组织图]</td> 
   <td>组织图的简称。 这是一个显示组织层次结构的图表。 它还位于[!UICONTROL User]详细信息屏幕的选项卡中，该选项卡上显示并允许设置[!UICONTROL User]的[!UICONTROL Company]和[!UICONTROL Reporting]关系。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL组织设置]</td> 
   <td>这为贵组织定义了[!UICONTROL公司]、[!UICONTROL组]和[!UICONTROL安全配置文件]。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL其他组]</td> 
   <td> <p>在列出用户的报表或视图中，此字段显示每个用户是其成员的所有组。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆盖货币]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作业角色]报表中，这是与作业角色关联的货币。 它是对[!UICONTROL Setup]区域中[!UICONTROL Base Currency]的覆盖，该覆盖在[!UICONTROL Setup]区域中通过 [!DNL Workfront] 管理员。 </p> 
     <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆盖货币帐单/小时]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作业角色]报表中，这是使用作业角色的选定[!UICONTROL覆盖货币]的作业角色每小时计费费率。</p> 
     <p> 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL覆盖货币成本/小时]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL作业角色]报表中，这是使用作业角色的选定[!UICONTROL覆盖货币]的作业角色每小时成本比率。 </p> 
     <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">创建和管理作业角色</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL所有者]</td> 
   <td>负责完成指定对象的用户。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL所有者类型]</span> </td> 
   <td> 
    <div> 
     <p>在[!UICONTROL目标]报表中，此报表显示分配给战略目标的所有者类型。 以下是目标所有者类型：</p> 
     <ul> 
      <li> <p>[!UICONTROL用户]</p> </li> 
      <li> <p>[!UICONTROL团队] </p> </li> 
      <li> <p>[!UICONTROL组]</p> </li> 
     </ul> 
     <p>当目标所有者是您的组织时，此字段中不会显示任何值。 </p> 
     <p>这需要额外的许可证。 有关 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概述</a>. </p> 
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
   <td>[!UICONTROL参数]</td> 
   <td> <p>[!UICONTROL参数]是自定义字段。 您可以为系统中的所有参数或自定义字段构建报表。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父项]</td> 
   <td>在报表中，此字段显示有关对象父项的信息。 例如，在[!UICONTROL问题]报表中，它可能显示有关记录问题的任务或项目的信息；在任务报表中，它可能显示有关直接父任务或项目的信息。 有关对象中可能具有父项的详细信息 [!DNL Workfront]，请参阅文章中的“对象的相互依赖关系和层次结构”部分 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解中的对象 [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父项滞后]</td> 
   <td>[!UICONTROL父任务]开始和[!UICONTROL子任务]开始之间必须经过的时间。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL父任务]</td> 
   <td>也称为[!UICONTROL摘要任务]。 这是一项具有子任务（也称为[!UICONTROL子任务]）的任务。 父任务的[!UICONTROL持续时间]、[!UICONTROL工作必需]和[!UICONTROL完成百分比]是从子任务中计算的。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL兼职资源]</td> 
   <td>容量小于系统中定义的默认计划的授权用户。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL完成百分比]</td> 
   <td> <p>项目、任务或问题字段，显示与任务、项目或问题关联的工作完成百分比。</p> <p>您可以为问题和工作任务手动更新此字段。 </p> <p>对于项目和父任务，此字段是所有工作任务的汇总字段，您无法手动更新它。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">项目[!UICONTROL完成百分比]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL权限]</td> 
   <td> <p>向用户授予对象上的权限，通常为用户授予权限，以便他们能够完成对项目的工作或查看项目。 您可以向以下用户授予权限：</p> 
    <ul> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL任务]</li> 
     <li>[!UICONTROL问题]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL程序]</li> 
     <li>[!UICONTROL报表]</li> 
     <li>[!UICONTROL功能板]</li> 
     <li>[!UICONTROL文档]</li> 
     <li>[!UICONTROL自定义Forms]</li> 
     <li>[!UICONTROL视图]</li> 
     <li>[!UICONTROL过滤器]</li> 
     <li>[!UICONTROL分组]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象共享权限概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划]</td> 
   <td> <p>这是 [!DNL Workfront] 系统。 用户必须具有此权限才能访问 [!DNL Workfront].</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划](在 [!DNL Scenario Planner])</td> 
   <td> <p>使用 [!DNL Workfront] 方案计划员。 您可以概述贵公司近期和长期未来的战略，并确定每个高级别结果，并将其作为计划添加到 [!DNL Workfront] 方案计划员。 </p> <p>无法显示 [!DNL Scenario Planner] 计划，您无法通过 [!DNL Workfront] API。 </p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL已计划]</td> 
   <td> <p>计划发生某件事的时间范围。 在中创建项目、任务或问题时 [!DNL Workfront]，则可建立计划的开始和结束日期以及计划的时间范围。 这些值代表您完成工作所需时间的原始意图或估计。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划收益]</td> 
   <td>这是项目经理的手动录入，用于评估完成项目是否会给组织带来任何经济利益。 指定此值可以是为项目构建[!UICONTROL Business Case]的一部分。 您必须对项目具有[!UICONTROL管理]权限才能更新此值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL预算小时数]</td> 
   <td> <p>在[!UICONTROL预算小时数]报表中，此报表显示[!UICONTROL资源规划器]中“项目”或[!UICONTROL任务角色]的预算小时数。 </p> <p>有关[!UICONTROL资源计划器]中预算项目或角色的信息，请参阅文章 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">使用[!UICONTROL Project]和[!UICONTROL Role]视图在[!UICONTROL Resource Planner]中预算资源</a>. 有关[!UICONTROL预算小时数]报表的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">报表：预算小时数</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划完成日期]</td> 
   <td> <p>您可以手动将[!UICONTROL计划完成日期]设置为您选择的日期。 如果未设置[!UICONTROL计划完成日期], [!DNL Workfront] 自动设置。 自动设置后，[!UICONTROL计划完成日期]为： [!UICONTROL计划开始日期] + [!UICONTROL持续时间]</p> <p>有关更多信息，请参阅以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">任务[!UICONTROL计划完成日期]概述</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">设置项目[!UICONTROL计划完成日期]</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划成本]</td> 
   <td> <p>项目的[!UICONTROL计划人工成本]和[!UICONTROL计划支出成本]的合计。 这不包括项目上的[!UICONTROL计划风险成本]。  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划持续时间]</td> 
   <td> <p>任务的[!UICONTROL计划持续时间]通常与任务的[!UICONTROL持续时间]相同。 它表示任务的[!UICONTROL计划开始]和[!UICONTROL计划完成日期]之间的天数差。 </p> <p>当任务的[!UICONTROL持续时间]类型为[!UICONTROL工作驱动]时，根据您为任务分配的资源数，[!UICONTROL计划持续时间]可能与任务的[!UICONTROL持续时间]有所不同。 </p> <p>例如，如果某个任务的[!UICONTROL持续时间]类型为[!UICONTROL工作驱动型]，则该任务的[!UICONTROL持续时间]为3天，并且您为该任务分配了一个具有完整时间计划的资源，则[!UICONTROL计划持续时间]也为3天。 如果您将三个具有全时计划的资源分配给同一任务，则[!UICONTROL持续时间]将保留3天，但[!UICONTROL计划持续时间]将变为1天。 [!UICONTROL计划持续时间]还会更改任务的[!UICONTROL计划开始]和[!UICONTROL计划完成日期]日期，以反映新的[!UICONTROL计划持续时间]。 因此，项目的时间表也会受到影响。 </p> <p>有关任务的[!UICONTROL持续时间]与[!UICONTROL计划持续时间]之间差异的详细信息，请参阅文章 <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">任务的[!UICONTROL计划持续时间]与[!UICONTROL持续时间]之间的差异</a>.</p> <p>项目和问题没有[!UICONTROL计划持续时间]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划持续时间（分钟）]</td> 
   <td> <p>项目或问题的[!UICONTROL计划持续时间分钟数]是项目的[!UICONTROL持续时间]，或问题（以分钟为单位）。 </p> <p>任务没有[!UICONTROL计划持续时间分钟数]字段。 </p> <p>[!UICONTROL模板任务]具有一个[!UICONTROL计划持续时间分钟]字段，该字段以分钟为单位显示任务的[!UICONTROL计划持续时间]。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划费用成本]</td> 
   <td> <p>为项目或任务记录的所有费用的[!UICONTROL计划金额]总和。</p> <p><b>示例</b></p>
   <p>如果为任务1创建费用，并在“[!UICONTROL计划金额]”字段中输入$600.00，则此任务的“[!UICONTROL计划费用成本]”为$600.00。 </p> 
   <p>对于项目， [!DNL Workfront] 使用以下公式计算[!UICONTROL计划费用成本]:</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划时数]</td> 
   <td> <p>此字段显示在[!UICONTROL项目]、[!UICONTROL任务]和问题区域、项目、任务或问题的报表，以及资源管理工具（如[!UICONTROL资源规划器]、[!UICONTROL工作负载平衡器]和[!UICONTROL利用率]报表）中。 </p> <p>它显示项目所有者估计完成每项任务或问题所花费的小时数。 对于项目，它通常是项目任务中的[!UICONTROL计划时数]汇总。 </p> <p>[!UICONTROL计划时数]字段可能会根据您从何处查看它而显示不同的信息。 有关计划时数的信息，请参阅 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">计划时数概述</a>.</p> <p>计划时数以分钟为单位存储，位于 [!DNL Workfront] 数据库。 使用此字段编写计算时，请确保考虑小时数显示为分钟这一事实。<br></p> <p>默认情况下，计划小时数会平均分配给工作项持续时间内的所有日期，并且对于分配给任务的所有资源也会平均分配。 用户可以更新工作项的每日计划小时数，或每个受让人的单个计划小时数。</p> <p>对于项目、任务和问题，更新此字段会有所不同： </p> 
    <ul> 
     <li> <p>对于问题，您可以手动更新此字段。 “发布计划时数”未添加到“项目计划时数”中。 </p> <p>提示：在问题报表中，[!UICONTROL计划时数]字段之一被替换为[!UICONTROL工作]字段。 字段显示问题的计划小时数。 有关更多信息，请参阅此表中的“work”或“[!UICONTROL Work]”字段。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>对于任务，当任务的[!UICONTROL持续时间类型]为[!UICONTROL计算分配]或[!UICONTROL简单]时，您可以手动更新此字段。 此字段的计算方式为 [!DNL Workfront] 当任务的[!UICONTROL持续时间类型]是[!UICONTROL计算工作]或[!UICONTROL工作驱动]时。<br>有关[!UICONTROL任务持续时间]的信息，请参阅文章 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">任务[!UICONTROL持续时间]和[!UICONTROL持续时间类型]概述</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>对于项目， [!DNL Workfront] 通过从项目上的所有任务添加所有计划小时数来计算计划小时数。 </p> </li> 
    </ul> <p><b>笔尖</b></p> <p>您还可以在[!UICONTROL项目]、[!UICONTROL任务]或[!UICONTROL问题]报表中通过使用文本模式并引用其他字段来显示[!UICONTROL计划时数]。 有关更多信息，请参阅<code>work</code>", "[!UICONTROL Work]"和"<code>workRequiredExpression</code>“ ”字段。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划人工成本]</td> 
   <td> 
    <p>对于任务，用户或角色的每小时费率乘以分配给用户或角色的小时数。</p> <p>对于项目，它是所有任务的所有[!UICONTROL计划人工成本]的总和。</p> <p>用户或角色的使用率取决于为给定任务选择的成本类型。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/project-finances/track-costs.md">跟踪成本</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划收入]</td> 
   <td> <p>任务和项目可以在 [!DNL Workfront]. [!UICONTROL计划收入]表示与项目上任务的[!UICONTROL计划时数]关联的金额。 对于项目，它还可以包含项目的[!UICONTROL Fixed Revenue]。 </p> <p>对于任务，这是与[!UICONTROL计划时数]任务关联的收入。 所有任务的计划小时数累计到项目的计划小时数，以帮助计算项目[!UICONTROL计划小时数]。 </p> 
   <p>[!DNL Workfront] 使用以下公式计算任务和项目的[!UICONTROL计划收入]:</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>在[!UICONTROL项目详细信息]区域和项目报表中显示的项目[!UICONTROL计划收入]与在[!UICONTROL Utilization]报表中显示的计划收入不同。 </p> <p>[!UICONTROL项目详细信息]区域中的[!UICONTROL计划收入]反映任务收入以及项目的固定收入。 [!UICONTROL Utilization Report]中的[!UICONTROL Planed Revenue]显示仅与项目中的任务关联的[!UICONTROL Planeded Revenue]。 </p> 
     <p><b>示例</b></p>  
      <p>如果项目有1个任务，10小时，该任务分配给顾问，每小时费率为$20，而项目有$100 [!UICONTROL固定收入]，则[!UICONTROL利用率]报表会显示$200（与任务小时数关联的[!UICONTROL计划收入]）。 “[!UICONTROL项目详细信息]”部分显示任务中的$300（[!UICONTROL计划收入]和项目的固定收入）。 </p> 
    <p>有关跟踪 [!DNL Workfront] 请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">账单和收入概述</a>. </p> 
    <p>有关[!UICONTROL Utilization Report]中[!UICONTROL Planed Revenue]计算的信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看资源利用信息 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划风险成本]</td> 
   <td> <p>项目上所有风险的[!UICONTROL潜在成本]总和，考虑到其发生概率。 此金额未包含在项目的[!UICONTROL计划成本]中。</p> <p>项目的[!UICONTROL计划风险成本]按以下公式计算：</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>管理员定义的选项卡和门户区域集合，显示在 [!DNL Workfront] 应用程序[!UICONTROL主页]和其他功能板。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>功能板或门户页面上选项卡的一个组件。 通常是单个报表、图表、日历或关键信息列表。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal选项卡]</td> 
   <td>门户或功能板上的选项卡，其中最多包含三个门户部分。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROLPortfolio]</td> 
   <td> <p>具有统一特征的项目集合。 这些项目通常会争夺相同的资源、预算或时间档。 在将Portfolio添加到Portfolio之前，您可以将项目划分为项目群，并将项目与项目群相关联。</p> <p>有关组合的更多信息，请参阅 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolio概述 [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio管理]</td> 
   <td>一个注重管理收藏或相关方案和项目工作的实践领域。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio优化程序]</td> 
   <td>A [!DNL Workfront] 帮助评估和确定项目组合中项目的优先顺序的工具。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio所有者]</td> 
   <td>负责确定投资组合的优先次序和预算的利益攸关方。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL潜在风险成本]</td> 
   <td>这是一个项目字段，您可以在列表和报表中找到该字段。 它显示与项目相关的风险的潜在成本（如果发生）。 有关详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL前身]</td> 
   <td> <p>在从属任务完成之前必须完成的任务。 另一个任务标记为[!UICONTROL依赖项]的任务。 前置任务允许计划员设置序列依赖关系逻辑，例如在其他任务完成后启动任务。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">任务前置任务概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>用户所属的公司，在其用户设置中指定。 公司也可以与项目关联。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL主要联系人]</td> 
   <td><p>[!UICONTROL Primary Contact]是问题的创建者，它由 [!DNL Workfront] 当某人创建问题时。 如果您具有 [!DNL Manage] 问题的权限。 问题只能有一个主要联系人。</p> 
   <p>如果更改主联系人，最初被指定为主联系人的用户仍具有[!UICONTROL Manage]对此问题的访问权限。</p>
   <p>将问题转换为任务或项目时，指定为的[!UICONTROL主要联系人]的用户将成为项目或任务的[!UICONTROL已转换的问题发起人]。 如果问题的[!UICONTROL Primary Contact]在问题转换后进行更新，则[!UICONTROL Converted Issue Originator]将保留为问题的[!UICONTROL Primary Contact]，在转换发生之时。 另请参阅本文中的“[!UICONTROL已转换的问题创作者]”。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL优先级]</td> 
   <td>可分配给任务、问题或项目以指定其重要性的值。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此选项会将该对象隐藏到大多数查看器中。 对于专用帮助台队列，只有队列团队的用户才能通过[!UICONTROL帮助台]区域向该队列提交问题。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>有关用户帐户的所有信息。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>组合中的一个子集，在该子集中，可以将相似项目组合在一起，以获得明确定义的好处。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>管理跨项目依赖关系、风险、问题、要求和解决方案，以保持计划的健康并实现明确的计划收益。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL程序所有者]</td> 
   <td>负责监督和组织活动以确保项目目标与公司目标一致的利益相关方。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>在[!UICONTROL目标]报表中，此报表显示完成战略目标的百分比。 进度百分比显示为数字。 有关战略目标的信息，另请参阅此表中的“[!UICONTROL目标]”。</p> <p>仅当贵组织已购买时，此字段才可见 [!DNL Workfront] 目标。 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> 将项目添加到 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL进度状态]</td> 
   <td> <p>在“项目”、“任务”和“目标”报表中，此字段显示项目、任务或战略目标的进度状态。 有关更多信息，请参阅以下文章：</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">项目进度状态概述</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任务进度状态概述</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">中的目标进度和条件概述 [!DNL Adobe Workfront Goals]</a> </p>
     <p>[!UICONTROL目标]报表和的[!UICONTROL进度状态] [!DNL goals] 字段，仅当您的组织已购买时才可见 [!DNL Workfront Goals]. 有关 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL项目]</td> 
   <td> <p>必须在特定时间范围内完成并且必须使用特定预算和资源数量的大量工作。 为了使其易于管理，您可以将项目分成一系列任务。 完成所有任务后，项目即告完成。 有关计划项目的信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">计划项目概述</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目分配计划时数]</td> 
   <td> <p>在[!UICONTROL方案作业角色]报表中，此报表显示与分配给项目中的任务或问题的作业角色相关联的[!UICONTROL计划时数]的数量。 此字段和[!UICONTROL Initiative Job Role]报表类型不显示在 [!DNL Workfront] 实例，除非您的公司购买了 [!DNL Workfront Scenario Planner] 许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md">的 [!DNL Workfront Scenario Planner] 概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目详细信息]</td> 
   <td>项目当前状态的详细信息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目预算成本]</td> 
   <td> <p> 这是项目在列表和报表中显示的[!UICONTROL预算成本]。</p><p>另请参阅本文中的“[!UICONTROL预算成本]”。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>一组策略，用于管理项目创建、分类和命名的阈值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL项目开销]</td> 
   <td>在[!UICONTROL Hour]报表中，此字段为与记录的小时数（小时类型为[!UICONTROL Project Time]）相关的财务信息保留。 项目可以有自己的计费费率，如果一个项目上直接记录了一个小时，则这些费率将用于计算。 根据项目设置，项目也可以使用不同的货币，并且这些时间内可以进行货币换算。 [!UICONTROL项目开销]对象允许 [!DNL Workfront] 来获取这些信息。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目所有者]</td> 
   <td>负责管理项目的范围、时间轴和分配的用户。 更改单、财务更改和交付项的默认审批者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>开发和维护项目计划的流程。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目赞助商]</td> 
   <td>每个用户都应与之关联的指定利益相关者资料。 在 [!DNL Workfront]，则这些级别被指定为[!UICONTROL访问级别]</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目团队]</td> 
   <td> <p>分配给项目的用户或角色的集合</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">项目团队概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL项目跟踪]</td> 
   <td>用于衡量项目运行状况和范围的数据</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL投影]</td> 
   <td> <p>根据任务、问题或项目的计划完成时间和完成百分比估计完成工作的时间时间。</p> <p>这是指任务、问题或项目的日期或[!UICONTROL持续时间]。 通常，它会指定在某些工作已经完成或一段时间过后，更符合工作项生命周期的日期和持续时间。 </p> <p>例如，任务的[!UICONTROL预计完成日期]是 [!DNL Workfront] 根据迄今为止已经完成的工作量、分配给该任务的人数以及自开始日期以来已经过的时间，估计任务将完成。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样截止时间]</td> 
   <td> <p>在包含[!UICONTROL文档版本]对象的报表（例如[!UICONTROL文档版本]报表和[!UICONTROL校样批准]报表）中，此字段显示校样截止日期的一周中的某天、某天、某天和某年。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL验证决策]</td> 
   <td> <p>在包含[!UICONTROL文档版本]对象的报表（例如[!UICONTROL文档版本]报表和[!UICONTROL校样批准]报表）中，此字段显示校样的决策状态（待定、需要更改或已批准）</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样名称]</td> 
   <td> <p>在包含[!UICONTROL文档版本]对象的报表（例如[!UICONTROL文档版本]报表和[!UICONTROL校样批准]报表）中，此字段显示校样名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样页面]</td> 
   <td> <p>在包含[!UICONTROL文档版本]对象的报表（例如[!UICONTROL文档版本]报表和[!UICONTROL校样批准]报表）中，此字段显示校样中包含的页数。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校样进度]</td> 
   <td> <p>在包含[!UICONTROL文档版本]对象的报表（如[!UICONTROL文档版本]报表和[!UICONTROL校样批准]报表）中，显示校样的进度状态（[!UICONTROL已发送]、[!UICONTROL已打开]、[!UICONTROL已评论]、[!UICONTROL Decision Makede]）。</p> <p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">校样进度概述</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">校样进度和状态概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL校对]</td> 
   <td>一个审阅过程，在该过程中，一个或多个用户对图像、文本文档、视频或交互式Web内容中应更改的内容进行标记和评论。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>在[!UICONTROL Note]或[!UICONTROL Document]上，此选项使其他用户甚至外部人员都可以访问该对象 [!DNL Workfront]. 对于[!UICONTROL帮助台队列],[!UICONTROL公共]表示所有能够提交问题的用户都可以通过[!UICONTROL帮助台]区域提交问题。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>组织内对工作质量的感知。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL队列]</td> 
   <td>也称为[!UICONTROL帮助台队列]。 这是一个已发布到[!UICONTROL帮助台]区域的项目，允许用户向其提交问题。 通常会为特定主题（如错误、项目请求等）创建队列。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL队列属性]</td> 
   <td>这些设置为要发布到[!UICONTROL帮助台]的项目定义问题提交规则。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL队列主题]</td> 
   <td> <p>[!UICONTROL帮助台队列]上的一个属性，允许提交问题的用户选择主题。 主题可以：</p> 
    <ul> 
     <li>与自定义数据表单关联。</li> 
     <li>通过选定主题上的路由规则集，将问题自动分配给用户、角色或团队。</li> 
     <li>通过选定主题上的路由规则集，将问题移动到其他项目或队列。</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排名]</td> 
   <td> <p>在[!UICONTROL访问级别]报表中，您可以手动指示[!UICONTROL访问级别]的[!UICONTROL排名]。 这可以帮助您，因为 [!DNL Workfront] 管理员，以便直观地确定与每个访问级别关联的复杂程度级别。 例如，您可以为更复杂（[!UICONTROL计划]级别）的访问级别指定较低的数字，为较复杂（[!UICONTROL请求者]级别）的访问级别指定较高的数字。 您无法对标准访问级别进行排名。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>任务报表中的此字段指示在积压工作中是否将[!UICONTROL Agile]任务标记为[!UICONTROL Ready]。 此标记仅适用于[!UICONTROL Agile]任务，这些任务是分配给[!UICONTROL Agile]团队的任务。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL重复频率]</td> 
   <td> <p>一个字段，显示在循环任务父项的[!UICONTROL任务详细信息]或[!UICONTROL编辑任务]框中。 定期中的任务发生的频率。 有关创建定期任务的信息，请参阅 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">创建定期任务</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL引用编号]</td> 
   <td> <p>项目、任务和问题在创建时会自动与唯一的参考编号关联。 您可以在项目、任务或问题的[!UICONTROL详细信息]页面或列表或报表中查看[!UICONTROL引用编号]。 </p> <p><b>笔尖</b><p><br>当两个项目具有相同的名称时，您可以推迟参考编号，因为参考编号始终唯一。 </p> <p>[!DNL Workfront] 自动在系统级别生成顺序参考编号。 每个项目、任务或问题都会获得序列中的下一个可用编号。 <br></p> <p>例如，如果用户A创建任务， [!DNL Workfront] 可以自动将任务分配为引用编号100。 如果用户B在此之后创建问题， [!DNL Workfront] 将问题分配为“引用编号101”。 不能手动编辑引用编号。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL拒绝问题]</td> 
   <td>在项目或任务报表中，这是在项目或任务的批准被拒绝时创建的问题。 有关拒绝问题的信息，请参阅文章 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL剩余风险成本]</td> 
   <td> <p>一个项目字段，显示项目的[!UICONTROL计划风险成本]与项目上所有风险的所有[!UICONTROL实际成本]的总和之间的差异。 </p> <p>项目的[!UICONTROL剩余风险成本]使用以下公式计算：</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL重新规划]</td> 
   <td>更改项目日期以修复或解决问题。 例如，需要重新计划已搁置数月的项目，以反映准确的日期。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL报表]</td> 
   <td>包含给定信息的图表或表 [!DNL Workfront] 对象及其相关属性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL请求]</td> 
   <td> <p>在单个集中队列中进行筛选的问题类型，与持续的工作无关。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL请求队列]</td> 
   <td>由流量和细分流程管理的积压问题。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL请求速度]</td> 
   <td>接收并完成请求的工作周期总时间。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>通常是许可证类型。 具有请求者许可证的用户可以提交对在系统中发生的新工作的请求。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL保留时间]</td> 
   <td>在用户的个人时间上指定的天数，表示用户将无法工作。 请参阅“[!UICONTROL非工作日]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解决问题]</td> 
   <td> <p>在问题报表中，在视图或过滤器中使用此字段可引用可解决此问题的问题。 </p> <p>有关在报表中显示解析对象的信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报表中查看可解析和可解析的对象信息</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解析项目]</td> 
   <td> <p>在问题报表中，在视图或过滤器中使用此字段可引用解决问题的项目。 </p> <p>有关在报表中显示解析对象的信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报表中查看可解析和可解析的对象信息</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL解析任务]</td> 
   <td> <p>在问题报表中，在视图或过滤器中使用此字段可引用解决问题的任务。 </p> <p>有关在报表中显示解析对象的信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">在报表中查看可解析和可解析的对象信息</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL资源]</td> 
   <td>系统中现有并分配给项目团队和任务的用户和/或角色。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management]是一套企业工具，它允许您根据资源的可用性准确预测资源的使用情况，以便必须按时按预算完成工作。 </p> <p>借助资源管理工具，您可以规划资源的长期容量和短期计划需求。 </p> <p>有关中的资源管理的信息 [!DNL Workfront]，请参阅 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">资源管理入门</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager ID]</td> 
   <td><p>在项目报表中，您可以在创建过滤器以查找特定资源管理器时使用此选项。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL资源管理器]</td> 
   <td> <p>在项目报表或列表视图中，这是一个信息性字段，用于显示指定在项目中执行资源管理活动的用户。  在报表中使用“[!UICONTROL Resource Managers]”时，将显示资源管理器列表，项目中的每个资源管理器都用逗号分隔。 您最多可以为给定项目指定30个资源管理器。</p> <p>有关更多信息，请参阅文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">为项目或模板指定资源管理器 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL资源计划员预算小时数] </td> 
   <td>在[!UICONTROL资源计划器]中为项目及与项目关联的资源编入预算的小时数。 另请参阅本文中的“[!UICONTROL预算小时数]”。 </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>高级 [!DNL Workfront] 可让您跨项目、作业角色或用户查看和管理资源的工具。 有关信息，请参阅 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">资源计划员概述</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL资源计划员预算人工成本]</td> 
   <td> <p>这些成本是与使用资源计划员为项目任务职责预算的小时数关联的成本。 </p> <p>另请参阅本文中的“预算人工成本”。 </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL资源池]</td> 
   <td> <p>资源池是可以与项目关联的用户集合。同一资源池中的用户通常属于同一部门，具有相似或互补的技能，或由同一预算供资。 您可以将多个资源池与一个项目或一个用户相关联。 资源池可以专门分配给项目或由多个项目共享。</p> 
   <p>有关资源池的详细信息，请参阅 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> 资源池概述 </a>.</p> 
   <p>在项目报表中，资源池显示与项目关联的所有池。 此对象不能用于分组。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL资源利用率]</td> 
   <td>报表显示特定时间段内可用的小时数以及报表中每个用户计划的小时数。 此值还计算为[!UICONTROL Average Hours Per Day]和分配百分比。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL结果]</td> 
   <td>在 [!DNL Workfront Goals]，则结果是目标的进度指示器。 它可以是手动更新的数字、百分比值或货币金额。 您无法在报表中显示结果，也无法通过 [!DNL Workfront] API。 有关活动的信息，请参阅 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">在Adobe Workfront目标中开始使用结果和活动</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>任务或项目的可计费金额。 金额可以是每小时、固定金额，也可以是两者的组合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>收入类型确定任务如何应计收入。 一些示例包括[!UICONTROL Fixed Horly]、[!UICONTROL Role Hourly]和[!UICONTROL Role Horly w/Cap]。 有关跟踪 [!DNL Workfront] 请参阅 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">账单和收入概述</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>通常是许可证类型。 具有[!UICONTROL Reviewer]许可证的用户能够审核和批准系统中的工作项。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL风险]</td> 
   <td> <p>这可能是指 [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>项目中用于指示项目风险的字段。 您可以根据风险级别优先执行项目。 项目可能具有以下风险级别：</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL低]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL高]</p> <p>- [!UICONTROL Very High]</p> <p>无法自定义您为项目指明的风险级别。 </p> <p> 有关更新项目风险的信息，请参阅文章的“项目设置”部分 <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">编辑项目</a>. 您可以在报表中显示项目的风险字段。 </p> </li> 
     <li> <p>在项目生命周期中可能发生的事件，可确定对项目成本、范围或计划的潜在影响。 您可以定义项目的潜在风险，并在构建项目业务案例时关联发生这些风险的可能性或成本。 有关为项目业务案例添加风险的信息，请参阅“创建和编辑项目风险”。 </p> <p>您不能在报表中显示在[!UICONTROL Business Case]中定义的风险。 您只能在报表和列表中显示几种类型的风险成本。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL风险成本]</td> 
   <td> <p>与项目风险相关的成本。 以下是与可在报表中显示的项目相关的风险成本：</p> 
    <ul> 
     <li> <p>[!UICONTROL实际成本]:显示已发生风险的实际成本的风险字段。 除了报表和列表之外，在编辑或创建风险时，您还可以在[!UICONTROL编辑风险]框中找到它。 </p> <p>有关项目、任务或问题成本，请参阅本文中的“[!UICONTROL实际成本]”。 </p> </li> 
     <li> <p>[!UICONTROL计划风险成本]:项目上的一个字段，显示项目的所有[!UICONTROL潜在风险成本]。 另请参阅本文中的“[!UICONTROL计划风险成本]”。 </p> <p>有关潜在风险成本的信息，请参阅 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">计算潜在风险成本 </a>. </p> </li> 
     <li> <p>[!UICONTROL剩余风险成本]:项目上的一个字段，显示所有风险的[!UICONTROL实际成本]合计与[!UICONTROL计划风险成本]之差。 另请参阅本文中的“剩余风险成本”。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>识别、缓解和监控风险的流程。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL角色]</td> 
   <td>请参阅本文中的“[!UICONTROL作业角色]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>自动分配或移动问题，通常是由于队列主题或作为队列的默认路由（路由规则）。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL路由规则]</td> 
   <td>项目和队列中的设置，可自动将问题分配给用户、角色或团队，或将问题移动到其他项目或队列。 路由规则通常与帮助台队列一起使用，以自动分配传入的问题。</td> 
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
   <td>[!UICONTROL保存的搜索]</td> 
   <td>已保存搜索条件的搜索。 通过保存搜索，可以轻松地再次运行相同的搜索，而无需再次输入搜索标准。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL方案](在 [!DNL Workfront Fusion]) </td> 
   <td> <p>方案由一系列步骤（模块）组成，这些步骤（模块）指示应如何在应用程序/服务之间传输和转换数据。</p> <p>有关 [!DNL Workfront Fusion]，请参阅 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 方案概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL方案](在 [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>在 [!DNL Scenario Planner]，则情景是计划的副本。 </p> <p>的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">的 [!DNL Scenario Planner] 概述</a>. </p> <p>有关创建方案的信息，请参阅 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">在 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划]</td> 
   <td>每周工作计划，包括工作时间、休息天数（如节假日）和例外天数（如星期六工作日）。 可以将计划应用于项目和用户。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划豁免]</td> 
   <td>也称为[!UICONTROL Modified Shift]。 计划的天数，与计划定义的常规每周工作时间形成对比。 例如，如果将计划设置为仅在星期一到星期五工作，则计划工作的星期六将是[!UICONTROL计划例外]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL计划报表]</td> 
   <td> <p>在生成报表报表时，如果报表已计划使用[!UICONTROL计划报表]字段提交，则可以显示有关报表计划的信息。 此字段在项目符号列表中显示多个值，每个报表的每个计划各显示一个值。 有关计划报表的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">报表交付概述</a>.</p> <p>由于此字段显示多个值，因此不能在分组中使用。 您只能在过滤器或视图中访问它。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL范围更改]</td> 
   <td>[!UICONTROL审核跟踪]，如果处于活动状态，则每当对项目或任务的范围进行更改时都会生成注释，如果[!UICONTROL任务持续时间]或[!UICONTROL前置任务]发生更改。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>屏幕上创建的用于组织自定义数据以用于显示目的的区域，以及其自身的标题。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL节中断]</td> 
   <td>节之间的间隙或边框。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>允许用户与系统中的某些对象而不是其他对象进行交互的设置。 另请参阅本文中的“[!UICONTROL访问级别]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL设置]</td> 
   <td>管理员可以在其中设置系统配置和首选项的区域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL严重性]</td> 
   <td> <p>[!UICONTROL严重性]是指明项目对完成工作的影响程度。 例如，[!UICONTROL严重性]高的问题可能会完全阻止任务的完成，但[!UICONTROL严重性]低的问题可能只是外观。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 更新问题严重性</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL严重性]</td> 
   <td>请参阅本文中的“[!UICONTROL严重性]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL共享]</td> 
   <td>允许其他用户在 [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLSlack日期]</td> 
   <td>在任务视图或报表中，[!UICONTROLSlack日期]显示任务肯定会影响项目[!UICONTROL完成日期]的确切日期。 有关任务的[!UICONTROLSlack日期]的信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">任务Slack日期概述</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>为用户分配任务或问题时， [!DNL Workfront] 根据最佳用户完成工作的时间以及他们与项目的关系，向他们提出建议（[!UICONTROL智能分配]）。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">智能分配概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>指示另一个对象的父对象。 例如，附加到任务的文档在[!UICONTROL Document]报表或视图的[!UICONTROL Source]字段中具有该任务的名称；在“问题”报表或视图的[!UICONTROL Source]字段中，在项目下记录的问题具有项目名称。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL开始日期]</td> 
   <td> <p>项目上的工作设置为开始的日期。 中有几个开始日期 [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL已计划]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL投影] </li> 
    </ul> <p>在[!UICONTROL费率报表]中，这是项目层职务角色的新开单费率开始的日期。 在此日期之后与项目关联的小时数乘以此开单费率，以计算项目收入。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL状态]</td> 
   <td> <p>用于指示工作项或战略目标的工作流位置的指示器。</p> <p>对于项目，[!UICONTROL状态]是项目中的一个设置，用于指示项目是否为：</p> 
    <ul> 
     <li>[!UICONTROL当前]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>有关项目状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">访问系统项目状态列表</a>.</p>
    <p>对于任务，[!UICONTROL Status]是任务中的一个设置，用于指示任务是否为：</p> 
    <ul> 
     <li>[!UICONTROL新建]</li> 
     <li>[!UICONTROL正在进行]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>有关任务状态的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">访问系统任务状态列表</a></p> <p>对于“问题”，[!UICONTROL Status]是“问题”上的一个设置，用于指示此问题是否为：</p> 
    <ul> 
     <li>[!UICONTROL新建]</li> 
     <li>[!UICONTROL正在进行]</li> 
     <li>[!UICONTROL正在等待反馈]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL已解析]</li> 
     <li>[!UICONTROL无法解析]</li> 
     <li>[!UICONTROL无法复制]</li> 
     <li>[!UICONTROL已验证结束]</li> 
     <li>[!UICONTROL重新打开]</li> 
    </ul> <p>有关问题状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>.</p> 
    <p>对于战略目标，[!UICONTROL状态]是目标上的一个设置，用于指示目标是否为：</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL草稿]</li> 
      <li>[!UICONTROL不活动]</li> 
      <li>[!UICONTROL已关闭]</li> 
     </ul> 
     <p>有关战略目标的更多信息，另请参阅本文中的“[!UICONTROL目标]”或“[!UICONTROL目标]”。 </p> 
     <p>对于战略目标，仅当贵组织已购买时，此字段才可见 [!DNL Workfront Goals]. 有关使用 [!DNL Workfront Goals]，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概述</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL状态更改]</td> 
   <td>[!UICONTROL审核记录]。 当用户更改项目、任务或问题的状态时，会生成注释。</td> 
  </tr> 
  <tr> 
   <td>状态图标</td> 
   <td> <p>您可以将内置的[!UICONTROL状态图标]字段添加为视图中的列，以增强对对象关键点的可见性，例如：</p> 
    <ul> 
     <li>对象附加了文档</li> 
     <li>对象与批准流程关联</li> 
     <li>对象具有与其关联的其他注释</li> 
     <li>费用可计费或可偿还 </li> 
     <li>任务在关键路径上</li> 
     <li>用户属于公司、团队，或位于其他时区 </li> 
    </ul> <p>您可以在以下对象的视图中添加[!UICONTROL Status Icons]字段： </p> 
    <ul> 
     <li>[!UICONTROL任务]</li> 
     <li>[!UICONTROL问题]</li> 
     <li>[!UICONTROL项目]</li> 
     <li>[!UICONTROL模板任务]</li> 
     <li>[!UICONTROL模板]</li> 
     <li>[!UICONTROL费用]</li> 
     <li>[!UICONTROL文档]</li> 
     <li>[!UICONTROL用户]</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL状态更新]</td> 
   <td> <p>此字段显示用户在“[!UICONTROL更新状态]”字段中提供的最新状态更新。 对状态更新所做的注释不会显示在[!UICONTROL状态更新]列中。</p> <p>要显示“[!UICONTROL New]”、“[!UICONTROL In Process]”和“[!UICONTROL Complete]”状态，请使用[!UICONTROL Status]列。</p> <p>对状态更新所做的注释不会显示在[!UICONTROL状态更新]列中。</p> <p>有关状态的更多信息，请参阅文章 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任务状态</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL状态]</td> 
   <td>请参阅本文中的“[!UICONTROL状态]”。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL情节提要]</td> 
   <td>一个图表，用于表示文章的状态（敏捷方法中的任务）以及文章的完成进度。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL文章时数]</td> 
   <td>用于衡量文章的难度或复杂性的量度。 敏捷团队可以选择使用小时还是点。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL文章点]</td> 
   <td>用于衡量文章的难度或复杂性的量度。 敏捷团队可以选择使用小时还是点。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>更改组织或组织工作方式的长期工作。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>衡量和调整各项目组合和计划中的公司目标。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL订阅者]</td> 
   <td> <p>订阅项目、任务或问题的用户。</p> <p>在报表中使用此字段时，将显示订阅者列表，每个订阅者以逗号分隔。</p> <p>有关更多信息，请参阅文章 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">订阅 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL摘要任务]</td> 
   <td>请参阅本文中的“[!UICONTROL父任务]”。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL子任务]</td> 
   <td>子任务，位于父任务下。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL系统管理]</td> 
   <td>一组控制系统更改和维护的策略。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL系统集成]</td> 
   <td>将不同的计算系统和软件应用程序物理或功能连接在一起，以便作为一个协调的整体。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任务]</td> 
   <td> <p>活动，必须作为实现最终目标（完成项目）的步骤来执行。</p> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">任务概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任务属性]</td> 
   <td>与任务关联并指明任务某些详细信息的其他字段或对象。 一些示例包括[!UICONTROL计划完成日期]和[!UICONTROL状态]。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL任务约束]</td> 
   <td>请参阅“[!UICONTROL Constraint Type]”和“[!UICONTROL Constraint Date]”。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任务管理]</td> 
   <td>一组策略，用于控制任务创建、分配、关闭和可见性的阈值。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL任务所有者]</td> 
   <td>负责估算工作量和完成任务的团队或用户</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL团队]</td> 
   <td> <p>致力于类似目标或业务目标的用户集合。 通过将团队分配给工作项，可以将这些用户集体分配给工作项。</p> <p>有关团队的更多信息，请参阅 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">团队概述</a>.</p> <p>项目可以具有[!UICONTROL项目团队]，其中包含与项目工作相关的所有用户或角色。</p> <p>有关项目团队的更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">项目团队概述</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL模板]</td> 
   <td> <p>项目模板是最可重复项目的通用概要。 在创建项目模板时，您可以定义任务、队列主题、自定义表单、附加文档或批准，以节省您必须创建新项目的时间。 </p> <p>您可以将模板附加到现有项目，也可以使用它们来构建新项目。 在模板中指定的所有信息都会传输到使用该模板创建的项目。 </p> <p>有关模板的更多信息，请参阅 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">项目模板概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL模板任务]</td> 
   <td>模板中的任务。 模板任务将成为使用模板创建的项目中的任务。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL线程]</td> 
   <td>[!UICONTROL Note]及其与特定主题相关的回复集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL缩略图]</td> 
   <td> <p> 在[!UICONTROL文档]列表或报表中，它以缩略图显示文档的预览。 </p> <p> 选择 <strong>[!UICONTROL缩略图]</strong>  查看报表中33-66像素范围的缩略图。 </p> <p>当您修改列表或报表中列的宽度时，缩略图的大小会随之发生调整。</p> <p>另请参阅本文中的“[!UICONTROL大缩略图]”。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>您可以构建一个[!UICONTROL关闭时间]报表，以查看用户在其配置文件中指示关闭时间的时间。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL时间表]</td> 
   <td> <p>一个工时记录卡，允许用户输入他们在项目、任务或问题上所花费的实际小时数，或者他们在与工作无关的其他活动（如会议或培训）上所花费的小时数。 除了输入工作所花费的时间量外，您还可以通过使用“小时类型”定义时间条目来指示时间是与工作相关还是与间接费用时间相等。 有关工时单的信息，请参阅 <a href="../../../timesheets/timesheets/timesheets-overview.md">工时单概述</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL时间表配置文件]</td> 
   <td> <p>[!UICONTROL时间表配置文件]是一个模板， [!DNL Workfront] 用于为与其关联的用户自动创建工时单。 </p> <p>您可以配置多个设置，这些设置将在创建时应用于每个时间表。 其中一些设置包括：应创建工时单的频率（每周、每两周、每月两次或每月）、工时单的开始日、时间单批准者、用户可与记录工时关联的可用[!UICONTROL Hour Types]。</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL顶级父ID] </td> 
   <td> <p>利用此字段，可识别和过滤列表或报表中有关顶级群组及其子群组的数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL顶级父名称] </td> 
   <td> <p>此字段允许您在[!UICONTROL视图]中识别有关列表或报表的顶级群组及其子群组的数据。</p> <p>您还可以使用[!UICONTROL Top Parent ID]字段执行此操作。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL总时数]</td> 
   <td> <p>在[!UICONTROL项目报表]中，此字段显示项目上所有小时数的四舍五入总和，即上次计算项目财务的时间。 [!UICONTROL实际小时数]反映了项目上记录的确切小时数。 通常，[!UICONTROL实际小时数]应与[!UICONTROL总小时数]匹配。 如果[!UICONTROL总时数]与[!UICONTROL实际时数]字段显着不同，则必须对项目重新计算财务。</p> <p>有关重新计算项目财务的详细信息，请参阅文章 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">重新计算项目财务</a>.</p> <p>在时间表[!UICONTROL Standard]视图中，此字段是指在时间表中显示的日期，针对项目记录的总小时数。 此内置视图中时单的[!UICONTROL Total Hours]字段引用“[!UICONTROL hoursDuration]”字段，该字段可动态计算工时单开始日期和结束日期之间的小时数差。 如果用户记录的时间超过时间表时间范围内的可用小时数，则此列将用红色显示[!UICONTROL总时数]列。 有关更多信息，请参阅 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">查看工时单的总工时数</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL跟踪模式]</td> 
   <td> <p>任务的属性。 这决定了如何更新任务的预计时间表，然后更新任务的预计时间表。 例如：</p> 
    <ul> 
     <li>[!UICONTROL用户必须更新]要求手动更新任务。 否则，它将变为[!UICONTROL Bewind Schedule]，然后变为[!UICONTROL Late]。</li> 
     <li>[!UICONTROL Auto Complete]将在到期日期或[!UICONTROL Planeded Complete Date]过后自动完成任务。</li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">任务跟踪模式概述</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL触发器]</td> 
   <td>启动方案的事件。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL故障任务]</td> 
   <td>条件为[!UICONTROL Late]、[!UICONTROL Bet Schedule]或[!UICONTROL At Risk]的未完成任务。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL未分配任务]</td> 
   <td>未分配给任何用户、角色或团队的任务。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL更新类型]</td> 
   <td> <p>项目中的一个设置，用于确定何时重新计算项目的预计时间轴。 选项包括：</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>有关更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">选择项目更新类型 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用户]</td> 
   <td>在中创建的帐户 [!DNL Workfront] 允许人员登录并与系统交互。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL用户委派]</p> </td> 
   <td> <p>可报告的对象，用于告知您：</p> 
    <ul> 
     <li>哪些用户已委派任务、问题和项目批准</li> 
     <li>哪些用户已将任务、问题和项目批准委派给他们</li> 
     <li>当这些代表团开始和结束时</li> 
    </ul> <p>要了解更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">创建用户委派报表</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用户界面]</td> 
   <td>的所有可视化和交互方面 [!DNL Workfront] 应用程序。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用户界面首选项]</td> 
   <td>[!UICONTROL用户界面设置]。 [!DNL Workfront] 管理员可以更改这些设置以自定义用户界面的各个方面。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL利用率]</td> 
   <td>根据分配的计划、PTO和当前工作量确定的用户或角色的可用性。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL用户利用率]</td> 
   <td> <p>搜索与报表组合在一起，用于显示如何分配或过度分配用户（资源）。 请参阅本文中的“[!UICONTROL Resource Utilization]”。</p> </td> 
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
   <td>[!UICONTROL Velocity]</td> 
   <td>测量总工作周期时间（完成某项工作需要多长时间）以及在最初承诺的时间内完成工作的频率（工作与承诺的比率）。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL视图]</td> 
   <td> <p>视图可用于修改报表或项目、任务或问题列表中的列，也可用于指示用户仅查看访问级别或权限共享级别信息的权限。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL视图图标]</td> 
   <td> <p> 此字段与状态图标相同，但仅适用于以下视图： </p> 
    <ul> 
     <li> [!UICONTROL文档] </li> 
    </ul> <p> 有关更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">视图中的内置状态图标</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上个月的查看次数]</td> 
   <td> <p>在报表列表中，它显示报表在上个月被查看的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL上一季度查看次数]</td> 
   <td>在报表列表中，它显示上个季度内查看报表的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >查看报表使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL去年查看]</td> 
   <td>在报表列表中，它显示报表在过去一年中被查看的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL本月查看]</td> 
   <td> <p>在报表列表中，它显示该月内查看报表的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL本季度查看]</td> 
   <td>在报表列表中，它显示该季度内查看报表的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">查看报表使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL今年的查看次数]</td> 
   <td>在报表列表中，它显示该报表在今年被查看的次数。<br>有关报表列表中使用情况信息的更多信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">查看报表使用情况</a>.</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>在项目、任务或问题报表中，在文本模式下使用以下语句可显示项目、任务或问题的计划时数：</p>
   <p></p><p></p> 
   <p>有关使用文本模式的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>. </p> 
   <p><b>笔尖</b> 
   <p>在问题报表中，添加[!UICONTROL计划时数]字段之一会添加 <code>work </code>字段。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>两种主要许可证类型之一。 这比[!UICONTROL Plan]的访问权限更少，但可以在系统中创建和更新。 这比[!UICONTROL External]、[!UICONTROL Reviewer]或[!UICONTROL Requester]许可证类型的功能更多。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] 许可证概述</a>.</p> <p>工作可能是指项目、任务或问题的[!UICONTROL计划小时数]。 有关更多信息，请参阅此表中的“[!UICONTROL work]”字段。 </p> <p>提示：在问题报表中，添加[!UICONTROL计划时数]字段之一会添加 <code>work </code>字段。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作划分结构]</td> 
   <td>由项目团队基于父/子关系执行的任务的层次结构。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作量] </td> 
   <td> 
    <p>项目经理可能决定使用此字段而不是[!UICONTROL计划时间]来估计完成任务所需的工作量。 仅当满足以下条件时，此字段才可见：</p> 
     <ul> 
      <li> <p>该任务具有[!UICONTROL简单持续时间类型]。 </p> <p>提示：如果将任务[!UICONTROL持续时间类型]更新为任何其他类型，则此字段将变为隐藏。 </p> </li> 
      <li>项目经理已启用[!UICONTROL Use Work Work]字段，以自动计算项目上的任务[!UICONTROL Planed Hours]。 </li> 
     </ul> 
     <p>有关使用[!UICONTROL工作量]而不是[!UICONTROL计划时间]来评估任务工作量的信息，请参阅 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">工作概述</a>. </p> 
     <p>您可以在任务报表和列表中显示此字段。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL工作项]</td> 
   <td> <p>此字段指的是 [!DNL Workfront]. </p> <p>[!UICONTROL工作项]报表显示有关任务和问题的信息。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理组合]</td> 
   <td>[!UICONTROL工作绩效指标](WPI)，其中包含用于运行您的业务与更改您的业务的工作比例。 混合WPI有助于您在组织级别了解您的策略是否对其应用了任何实际工作分配。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>系统中有资格接收工作或跟踪时间的角色的指定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理角色和职责]</td> 
   <td>定义所有者和利益相关方，以管理指定问题、任务、项目、项目或项目组合的范围、执行和批准。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理SLA]</td> 
   <td>所有利益相关方都同意的可量化量度。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理利益相关者]</td> 
   <td>对工作请求结果具有既得利益的用户集合。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作管理接触点]</td> 
   <td>利益攸关方之间交流的数字化记录。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作绩效指标] </td> 
   <td> <p>混合比率、容量、速度、质量和参与度。</p> <p>WPI是[!UICONTROL工作绩效指标]的常见首字母缩略词。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>接收、排定优先级和执行工作的方法。 执行工作的方式通常称为“工作流”或“项目计划”（包含日期、前身关系等的任务列表）。 </p> <p>工作流程的示例可能是生产单个资产或交付多资产营销活动。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作流模板]</td> 
   <td>在[!UICONTROL校样批准]报表中，此字段显示附加到校样的任何工作流模板。 如果没有附加模板，则列为空。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL工作时间]</td> 
   <td>

<p><span class="preview">表示用户可用于实际工作（不包括间接费用）的全职等效(FTE)时间的百分比。 工作时间必须是最多1的小数，并且不能是0。 例如，实际工作的20%可用性为0.2。</span>  </p>
   </p><span class="preview">字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。</span>   </p>
   <p><span class="preview">系统使用此编号来计算用户在实际项目相关工作中的可用性。 </span></p>
   <p> <span class="preview">计划例外和休息时间也可能影响用户容量。</span> </p>
   <p><span class="preview">有关在Workfront中创建计划的更多信息，请参阅创建计划。 （插入链接）</span> </p>
    <p>Workfront会根据“设置”区域中的“资源管理”首选项来计算用户的可用性。 有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">配置资源管理首选项</a>. </p> 
   <p><span class="preview">您可以在编辑或创建用户时更新用户的工作时间。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">编辑用户的配置文件</a></span></p> 
   <b>笔尖</b> 
   <p><span class="preview">将“工作时间”值设置为1，以指示用户可用于与项目相关的工作，且其整个全时对等工作。</span></p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL工作时间]</td> 
   <td>在Workfront文档中，此术语用于描述根据计划分配的工作时间。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>在项目、任务或问题报表中，在文本模式下使用以下语句显示项目、任务或问题的计划小时数，后跟“小时”一词：</p>
   <p></p><p></p>
    <p>有关使用文本模式的信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">文本模式语法概述</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
