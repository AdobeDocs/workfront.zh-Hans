---
product-area: reporting
navigation-topic: using-built-in-reports
title: 视图中的内置状态图标
description: 可在视图中添加内置的状态图标字段作为列，以增强关于对象关键点的可见性。
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 2%

---

# 视图中的内置状态图标

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

可在视图中添加内置的状态图标字段作为列，以增强关于对象关键点的可见性。 通过使用状态图标，您可以一眼看出是否存在以下情况：

* 对象已附加文档
* 对象与审批流程相关联
* 对象具有与其关联的其他注释
* 费用是应计费的或应偿还的
* 任务位于关键路径上
* 用户属于公司、团队或位于其他时区

请考虑以下事项：

* “状态图标”字段中的大多数指示器都是指向它们所表示的实际对象或对象区域的快速链接。

* 如果对象中缺少由图标表示的任何项目，则表示缺少项目的图标在“状态图标”列中将显示为灰色，而不是彩色图像。

  ![task_status_icons.png](assets/task-status-icons.png)

  有关详细信息，请参阅本文中的[状态图标和标志概述](#overview-of-status-icons-and-flags)部分。

* 在某些视图中，**状态图标**&#x200B;字段名为&#x200B;**标志**&#x200B;或&#x200B;**视图图标**。\
  您无法自定义“状态图标”字段中包含的图标的外观。

* 您无法编辑状态图标字段中的图标数。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以将列添加到报告中</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理现有视图的权限</p> <p>管理报表的权限以向其添加列</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 将状态图标字段添加到视图

某些内置视图和报告已包含状态图标字段。

不能将“状态图标”字段添加到所有视图。

要将状态图标字段添加到您从头开始构建的自定义视图中，请执行以下操作：

1. 转到以下任意对象的列表：

   * 任务
   * 问题
   * 项目
   * 模板任务
   * 模板
   * 费用
   * 文档
   * 用户\
     只有这些对象具有&#x200B;**状态图标**&#x200B;字段可用。\
     有关对象列表的信息，请参阅[Adobe Workfront中的列表入门](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**。
1. 在&#x200B;**显示在此列**&#x200B;框中，开始键入以下任何字段名称，然后当该字段出现在列表中时将其选定：

   * *状态图标*
   * *标志*
   * *查看图标*（仅在文档视图中）。

   内置图标会列在任意这些名称下。\
   模板视图包含&#x200B;**状态图标**&#x200B;和&#x200B;**标志**&#x200B;字段。 在这种情况下，两列包含相同的图标。\
   文档视图包含&#x200B;**视图图标**&#x200B;字段。

1. 单击&#x200B;**保存视图**。
1. （可选）为您的视图指定新名称，然后单击&#x200B;**保存视图**。\
   这会将&#x200B;**状态图标**&#x200B;列添加到您的视图中。
1. （可选）将鼠标悬停在图标上以了解其代表的含义。
1. （可选）单击图标以转到由其表示的对象的区域。\
   并非所有图标都是指向对象的链接。\
   有关每个图标的完整属性列表，请参阅[状态图标和标志概述](#overview-of-status-icons-and-flags)部分。

## 状态图标和标志概览 {#overview-of-status-icons-and-flags}

下表列出了Workfront中可用的所有状态图标、可以与其关联的对象类型以及在单击这些图标时发生的情况。

您必须至少具有查看对象的权限，才能单击以下某些图标并访问这些对象。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>状态图标或标志</strong> </th> 
   <th><strong>描述</strong> </th> 
   <th><strong>对象</strong> </th> 
   <th>单击</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">或<img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;">或<img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;">或 <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>指示项目的完成情况符合目标（绿色）、存在问题（红色）或处于风险中（黄色）。<br>有关项目完成情况的信息，请参阅<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">项目完成情况和完成情况类型概述</a>。</td> 
   <td>项目</td> 
   <td>单击以打开项目的任务列表。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>指示对象在“更新”选项卡中有注释（更新）。</td> 
   <td> <p>项目<br>任务<br>问题<br>模板<br>模板任务</p> </td> 
   <td> <p>单击以打开对象的“更新”选项卡。 </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">或 <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>指示对象已附加文档。 </td> 
   <td> 项目<br>任务<br>问题<br>模板<br>模板任务 </td> 
   <td>单击以打开对象的“文档”选项卡。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">或 <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>指示项目或任务中存在未完成的问题。</td> 
   <td> 项目<br>任务 </td> 
   <td>单击以打开对象。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> 或 <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>表示对象已获得批准。</td> 
   <td> 项目<br>任务<br>问题<br>模板<br>模板任务 </td> 
   <td>单击以打开对象。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="expenses_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>您可以在视图中添加费用图标列以显示此图标。 这表示项目或任务具有与其关联的费用。</p> </td> 
   <td> <p>项目</p> <p>任务</p> </td> 
   <td>单击以打开项目或任务的“费用”选项卡。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>指示任务的进度状态是以下状态之一：</p> 
    <ul> 
     <li>开始时间（绿色方块）</li> 
     <li>延迟（红色圆形）</li> 
     <li>处于风险中（蓝色菱形）</li> 
     <li>后置（黄色三角形）</li> 
    </ul> <p>有关任务进度状态的信息，请参阅<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">任务进度状态概述</a>。</p> </td> 
   <td>任务</td> 
   <td>单击以打开任务。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> 或 <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>指示任务当前位于关键路径上。 <br>有关项目关键路径上的任务的信息，请参阅<a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">项目关键路径概述</a>。</td> 
   <td>任务</td> 
   <td>单击以打开任务。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>指示任务与里程碑相关联。 系统管理员可以自定义环境中菱形的颜色。<br>有关里程碑的信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">创建里程碑路径</a>。</td> 
   <td>任务</td> 
   <td>单击以打开任务。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>链接到问题的源对象。 问题的源对象是记录问题的对象。 任务或项目可以是问题的源对象。 </td> 
   <td>问题</td> 
   <td>单击以打开问题的源对象（任务或项目）。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>表示存在最终解决该问题的解决对象。 在这种情况下，您无法完成问题。 解析对象完成时完成。 <br>有关解析对象的信息，请参阅<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述</a>。</td> 
   <td>问题</td> 
   <td>单击以打开问题的解决对象。 </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>查看文档。</td> 
   <td>文档</td> 
   <td>单击以下载文档。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>下载文档。</td> 
   <td>文档</td> 
   <td>单击以下载文档。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>指示文档类型。</td> 
   <td>文档</td> 
   <td>单击以下载文档。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_belists_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>指示用户与公司相关联。 </td> 
   <td>用户</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>指示用户与团队相关联。</td> 
   <td>用户</td> 
   <td>单击以打开用户配置文件。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>用户分配选项卡的快捷方式。 </td> 
   <td>用户</td> 
   <td>单击以打开用户的分配选项卡，并了解为用户分配的工作项。</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>指示用户与系统的时区不同。</td> 
   <td>用户</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_expense_icon.png" style="width: 44;height: 45;"> </td> 
   <td>指示费用可记帐。<br>有关费用的信息，请参阅<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理项目费用</a>。</td> 
   <td>费用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="expense_lemensable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> 指示费用是可退还。<br>有关费用的信息，请参阅<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理项目费用</a>。</td> 
   <td>费用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="replaced_expense_icon.png" style="width: 44;height: 43;"></td> 
   <td> 指示费用已退还。<br>有关费用的信息，请参阅<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">管理项目费用</a>。</td> 
   <td>费用</td> 
   <td>不可用</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
