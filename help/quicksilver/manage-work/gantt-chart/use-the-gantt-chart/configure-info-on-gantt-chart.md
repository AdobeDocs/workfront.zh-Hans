---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: 配置信息在 [!UICONTROL 甘特图] 图表
description: 您可以配置任务列表甘特图和项目列表甘特图中显示的信息。
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# 配置信息在 [!UICONTROL 甘特图]

您可以配置在两个任务列表中显示的信息 [!UICONTROL 甘特图] 和项目列表 [!UICONTROL 甘特图].

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[!UICONTROL视图]或更高版本对项目和任务的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>[!UICONTROL视图]或更高级别访问项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 了解显示选项

下表详细列出了 [!UICONTROL 甘特图]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL实际日期]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL实际开始日期]和[!UICONTROL实际完成日期]将显示一个三角形图标。 如果[!UICONTROL实际完成日期]为空，则只显示[!UICONTROL实际开始日期]。</p> <p>有关开始和完成日期的更多信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">项目[!UICONTROL实际完成日期]概述 </a> 和 <a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">项目[!UICONTROL实际开始日期]概述 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL分配]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>显示任务分配者。 将鼠标悬停在 <strong>[!UICONTROL详细信息]</strong> 链接至受分派人名称旁，以查看有关受分派人的更多详细信息，包括其分配给任务的百分比。</p> <p>将[!UICONTROL甘特图]导出到PDF时，分配项不会显示在[!UICONTROL甘特图]中。 将[!UICONTROL甘特图]导出到PDF后，任务列表中仅显示受分配者。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL基线]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gantt.png"> </td> 
   <td> <p>表示初始项目计划中包含的项目相关关键数据段的项目快照。 在项目的整个生命周期中都可以采用基线。 启用在[!UICONTROL甘特图]中显示基线时，选择要显示的基线。 一次只能在[!UICONTROL甘特图]上查看一个基线，该基线将以灰色条的形式显示。</p> <p>有关基线的更多信息，请参阅 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">创建项目基线</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL提交日期]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>在[!UICONTROL甘特图]中，将使用标记显示任务完成时被分派人作为其承诺的日期。 </p> <p>有关提交日期的更多信息，请参阅 <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL提交日期]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td>  任务行中会显示已完成任务的百分比。<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL关键路径]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>可能影响项目时间轴的任务被视为关键路径的一部分，并且明显以红色标记。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]钻石</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>在与里程碑关联的任务之后会显示一个菱形图标。 将鼠标悬停在里程碑上可查看里程碑的名称和日期。 的 [!DNL Workfront] 管理员确定每个里程碑钻石的颜色。</p> <p>有关里程碑的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">创建里程碑路径</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL里程碑]行</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gantt_png" style="width: 270;height: 209;"> </td> 
   <td> <p>在与里程碑关联的任务之后会显示一个行。 将鼠标悬停在里程碑上可查看里程碑的名称和日期。 的 [!DNL Workfront] 管理员确定每个里程碑行的颜色。</p> <p> 有关里程碑的更多信息，请参阅  <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">创建里程碑路径</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL前置版]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="prepisent_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>从一个任务到另一个任务的行，显示两个任务之间的前置任务关系。 要突出显示单个前置行，请将鼠标悬停在该行上。 单击该图标以使其高亮显示。 一次只能突出显示一条前置行。</p> <p>A <strong>[!UICONTROL前身]</strong> 图标显示在任何具有前置任务关系的任务旁边，该前置任务关系跨越甘特图上的多个页面，或显示在具有跨项目前置任务的任何任务上。</p> <p>单击 <strong>[!UICONTROL前身]</strong> 图标以查看所有前置任务和后置任务，以及有关每个任务的详细信息，如任务名称、前置任务关系类型和关键日期。</p> <p>注意：项目列表中的[!UICONTROL甘特图]显示了有关跨项目前置任务的信息。 有关如何在不同项目之间创建前置任务关系的更多信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">创建跨项目前置项</a></p> <p>有关前置任务的详细信息，请参阅 <a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">强制前置任务</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL进度状态]</td> 
   <td> <p>[!UICONTROL On Time] <img src="assets/task-on-time--oct.-2017.png" alt="task_on_time__10月_2017.png"></p> <p>[!UICONTROL Beind]    <img src="assets/task-behind--oct.-2017.png" alt="task_bidten__10月_2017.png"></p> <p>[!UICONTROL面临风险]    <img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>延迟        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>给定任务的当前进度状态。 </p> <p>有关每种[!UICONTROL进度状态]类型的更多详细信息，请参阅 <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任务[!UICONTROL进度状态]概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL预计日期]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>根据当前已完成的工作以及剩余的工作，标记[!UICONTROL预计开始]和[!UICONTROL完成日期]的预期预计时间线。 </p> <p>有关预计完成日期的详细信息，请参阅 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">项目、任务和问题的[!UICONTROL预计完成日期]概述</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置显示选项

1. 转到任务列表 [!UICONTROL 甘特图] 或项目列表 [!UICONTROL 甘特图].\
   有关 [!UICONTROL 甘特图] 位于，请参阅 [开始使用 [!UICONTROL 甘特图]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

1. （可选）选择 **[!UICONTROL 切换到预计日期]** 设置以按 [!UICONTROL 预计日期]. 默认情况下，任务会按 [!UICONTROL 计划日期] 在 [!UICONTROL 甘特图].
1. 单击选项图标以显示 **[!UICONTROL 选项]** 对话框。\
   ![Options.png](assets/options-350x129.png)

1. 选择要在 [!UICONTROL 甘特图].

   >[!NOTE]
   > 并非所有配置选项都在项目列表中可用 [!UICONTROL 甘特图].

1. 单击 [!UICONTROL 甘特图] 关闭 **[!UICONTROL 选项]** 对话框。
