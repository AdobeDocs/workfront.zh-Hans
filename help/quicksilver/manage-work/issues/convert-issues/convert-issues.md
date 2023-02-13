---
product-area: projects
navigation-topic: convert-issues
title: 转换Adobe Workfront中的问题概述
description: 如果在提交问题后需要完成更多工作才能完成问题，您可以将问题转换为项目或任务。
author: Alina
feature: Work Management
exl-id: 97c83b65-208b-4e3f-b4cc-681237d82aa3
source-git-commit: 24cc3ece515fd778a9bc9e8afbcd534f48b24230
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 2%

---

# 转换Adobe Workfront中的问题概述

如果在提交问题后需要完成更多工作才能完成问题，您可以将问题转换为项目或任务。

有关将问题转换为任务的信息，请参阅 [在Adobe Workfront中将问题转换为任务](../../../manage-work/issues/convert-issues/convert-issue-to-task.md).

有关将问题转换为项目的信息，请参阅 [在Adobe Workfront中将问题转换为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## 转换问题时的注意事项

* 您的Workfront管理员或组管理员已经为问题发生的情况、其解决方式以及将问题转换为项目或任务时主要联系人的访问权限设置首选项，如 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Workfront会删除在转换过程中与问题相关的任何批准。
* Workfront在您将问题的解决对象转换为任务或项目时会覆盖该对象。 新任务或问题在转换后成为问题的新解决对象。
* 请考虑以下事项：

   * 在转换过程中，可能会询问您是否希望将问题及其解决方案与您创建的项目或任务绑定。
   * 如果保留问题，则当项目、任务或问题发生任何更改或Workfront重新计算时间轴时，项目或任务的状态和完成百分比会自动更新问题的状态和完成百分比。

* 在使用模板将问题转换为项目时，模板中的大多数信息都会传输到新项目。 但是，问题中的某些信息也可以转移到新项目。 有关更多信息，请参阅 [使用模板将问题转换为项目时的项目字段概述](#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template) 章节。
* 在转换问题时，并非所有文档或其信息都会移动到将问题转换为的新对象。 在转换附加了文档或文档链接的问题时，将包括以下项目：

   * 文档
   * 将链接记录到第三方服务，如Google Drive或SharePoint。
   * 版本
   * 仅当选项 **保留原始问题，并将其解决办法与此任务挂钩** 中。
   * 在转换附加了文档和文档链接的问题时，不包括文档批准。

* 如果您决定将问题保留在转换中，并且附加了文档，则文档及其版本将会复制到项目或任务中。 校样和文档批准不会复制到项目或任务中。
* 如果您决定不将问题保留在转换中，并且它附有文档、文档、其版本以及校样传输到项目或任务。 文档批准不会转移到项目或任务。
* 如果您的文档和文件夹链接到来自第三方服务(如Google Drive)的原始问题，无论您在转换过程中是否保留该问题，这些链接都将复制到新对象。
* 系统还会将问题评论复制到从问题转换的任务或项目中，但标记的用户将不会转移。
* 如果要将自定义表单信息从问题传输到要转换到的项目或任务，请确保您有一个项目或任务自定义表单，其中包含要从问题中传输的相同字段。 有关更多信息，请参阅 [转换对象时传输自定义表单数据](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md).

## 使用模板将问题转换为项目时的项目字段概述 {#overview-of-project-fields-when-converting-an-issue-to-a-project-using-a-template}

将问题转换为项目时，您可以将其转换为空白项目或使用模板。

有关信息，请参阅 [在Adobe Workfront中将问题转换为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

使用模板时，模板中填充的某些字段会传输到由转换后的问题创建的项目。 其他字段会从转换后的问题传输到项目。

下表列出了项目信息以及项目信息是从模板还是从问题进行传输：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>描述</td> 
   <td> <p>问题描述会转移到新项目。 </p> <p> 如果没有有关该问题的说明，则模板中的说明会传输到项目。 </p> <p>对于问题和模板，如果“描述”字段都为空，则项目中的字段为空。 </p> </td> 
  </tr> 
  <tr> 
   <td>状态</td> 
   <td>为模板上的组选择的默认状态。 如果模板未与组关联，则项目状态将设置为Workfront管理员在“设置”的“项目首选项”区域中设置的默认状态。 有关信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">配置系统范围的项目首选项</a>.</td> 
  </tr> 
  <tr> 
   <td>优先级</td> 
   <td>从模板进行传输。 </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td> <p>问题中的URL会传输到新项目。 </p> <p> 如果问题上未指定URL，则模板中的URL将传输到项目。 </p> <p>如果问题和模板的URL字段都为空，则项目中的字段为空。 </p> </td> 
  </tr> 
  <tr> 
   <td>项目条件类型</td> 
   <td>从模板进行传输。</td> 
  </tr> 
  <tr> 
   <td>项目条件</td> 
   <td>与Workfront管理员在“设置”区域中确定的系统级别默认首选项匹配。 有关信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">将自定义条件设置为项目的默认条件</a></td> 
  </tr> 
  <tr> 
   <td>时间表开始日期</td> 
   <td>从模板进行传输。</td> 
  </tr> 
  <tr> 
   <td>项目日期</td> 
   <td> 
    <ul> 
     <li> <p><b>计划开始日期</b>:应根据模板计划的时区，预先选择基于模板计划工作时间的最近工作时间。 如果将“计划自”字段设置为“从完成”，则禁用此字段。 </p> </li> 
     <li> <p><b>计划完成日期</b>:应根据模板计划的时区，预先选择基于模板计划工作时间的最近工作时间。 如果将“计划起始”字段设置为“起始”，则禁用此字段。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>从模板进行传输。 否则，此字段为空。</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>从模板进行传输。 否则，此字段为空。</td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>从模板进行传输。 如果模板上没有组，则会将其设置为问题所属的项目组。</td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>从模板进行传输。 否则，此字段为空。</td> 
  </tr> 
  <tr> 
   <td>项目所有者</td> 
   <td>从模板上的“模板所有者”字段进行传输。 否则，它将设置为正在执行转换的登录用户。 </td> 
  </tr> 
  <tr> 
   <td>项目赞助者</td> 
   <td>从模板上的“模板赞助商”字段进行传输。 否则，此字段为空。</td> 
  </tr> 
  <tr> 
   <td>资源管理器</td> 
   <td>从模板进行传输。 否则，此字段为空。</td> 
  </tr> 
  <tr> 
   <td>任务设置</td> 
   <td>从模板中传输。</td> 
  </tr> 
  <tr> 
   <td>问题设置</td> 
   <td>从模板中传输。 </td> 
  </tr> 
  <tr> 
   <td>访问权限</td> 
   <td> <p>从模板上的访问部分传输。 </p> </td> 
  </tr> 
  <tr> 
   <td>审批</td> 
   <td>从模板中传输。 在转换期间，将删除与问题关联的批准。 </td> 
  </tr> 
 </tbody> 
</table>

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a project</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the <strong>Issues</strong> icon on a project. <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/qs-issues-icon-highlighted-on-project.png"> </p> </li>
<li value="2"> <p>Click the issue to be converted to access the issue.</p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu, then click <strong>Convert to Project</strong>. </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>In the submenu that displays, do one of the following:</p>
<ul>
<li>Click <strong>New Project</strong></li>
<li>Under <strong>New from Template</strong>, click the name of a project template you want to use</li>
</ul> </li>
<li value="5"> <p>Specify a name for the project.</p> <p>The default name is the name of the issue you are converting.</p> </li>
<li value="6">(Optional and conditional) If you are creating this project from a template, update the available fields in the Convert to Project box.<br>For more information about editing fields on projects, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the available options:</p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this project</strong>When deselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li><strong>Allow <User Name> to have access to this project</strong>If unselected, the user who entered the issue has no access to the new task.</li>
</ul> <note type="note">
<div>
<p>The options that are available here depend on how the Workfront administrator has configured them for everyone in the system or for your group. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options available here depend on which group you selected for the new project in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a><span class="preview">.</span></p>
</div>
</note> </li>
<li value="8">(Optional) In the <strong>Custom Forms</strong> section, attach any custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new project, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.</li>
<li value="9"> <p>Click <strong>Save Changes.</strong></p> <p> <img src="assets/qs-issue-convert-to-project-before-saving-ui-350x366.png" style="width: 350;height: 366;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> <p>The issue is now a project, if you decided to delete the original issue.<br>Or<br>The issue is now linked to the new project and it will complete when the project completes, if you decided to keep the original issue. </p> <p>Some issue fields transfer to the project. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. </p> </li>
<li value="10"> <p>(Optional) Set any further project details ​(project owner, project dates) and tasks as necessary.</p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Convert an issue to a task</h2> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: moved to its own article)</p>
-->
<!--
<ol>
<li value="1"> Click the Issues icon on a project.  </li>
<li value="2"> <p>Click the issue you want to convert to go to the issue's landing page. </p> </li>
<li value="3"> <p> Click the <strong>More</strong> menu on the issue, then <strong>Convert to Task</strong>.  </p> <p> <img src="assets/qs-issue-more-menu-highlighted-350x469.png" style="width: 350;height: 469;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="4"> <p>Name the task.</p> </li>
<li value="5"> <p>Identify the project where the task will reside. </p> <p>You can select a different project from the project that the issue is on.</p> </li>
<li value="6"> <p>In the <strong>Project</strong> box, start typing the name of the project where you want to put the new task, then press <strong>Enter</strong> when it appears.</p> <p>By default, this box the name of the project containing the issue that you are converting.</p> </li>
<li value="7"> <p>(Optional and conditional) Under <strong>Options</strong>, select any of the following options. </p> <p>The Workfront administrator or group administrator must enable these preferences before they are visible during the conversion of issues: </p>
<ul>
<li> <p><strong>Keep the original issue and tie its resolution to the this task</strong> </p> <p>If unselected, the original issue is deleted.</p> <note type="note">
<p>Users without access or permissions to delete issues will not be able to delete the issue as they are converting it, regardless of the status of this setting. For information about access and permissions to issues, see:</p>
<ul>
<li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a> </p> </li>
<li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a> </p> </li>
</ul>
</note> </li>
<li> <p><strong>Allow <User Name> to have access to this task</strong> </p> <p>If unselected, the user who entered the issue has no access to the new task.</p> </li>
<li> <p><strong>Keep the planned completion date of the issue</strong> </p> <p>If unselected, the Planned Completion Date of the new task is calculated from the Planned Start Date of the task. The Planned Start Date of the new task is set according to the system preferences for new tasks.</p> </li>
</ul> <note type="note">
<div>
<p>The options that display here depend on how the Workfront administrator configured them for everyone in the system. For more information, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p>
<p>Or, if the top-level groups in your organization configured them separately, the options that display here depend on which group is associated with the project you selected in step 6. For more information, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md" class="MCXref xref">Configure task and issue preferences for a group</a>.</p>
</div>
</note> </li>
<li value="8">(Optional) Attach custom forms.<br>For more information about transferring information from the custom form of the issue to that of the new task, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md" class="MCXref xref">Transfer custom form data when converting an object</a>.<br><p><img src="assets/qs-issue-convert-to-task-before-saving-ui-350x367.png" style="width: 350;height: 367;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p></li>
<li value="9"> <p>Click <strong>Save Changes</strong> when all task settings are set.</p> <p>The issue is now a task on the designated project, if you decided to delete the original issue.</p> <p>Or</p> <p>The issue is now linked to the new task on the project you chose, and it will complete once the task completes, if you decided to keep the original issue.</p> <p>Some issue fields transfer to the task. For information, see the <a href="#view-original-issue-information-on-projects-and-tasks" class="MCXref xref">View original issue information on projects and tasks</a> section in this article. <br></p> </li>
<li value="10"> <p>(Optional) Continue editing the task (assignments, dates) as necessary. </p> </li>
</ol>
</div>
-->

## 查看有关项目和任务的原始问题信息 {#view-original-issue-information-on-projects-and-tasks}

您可以在项目和任务列表和报表中或在“项目详细信息”区域中查看原始问题信息。 有关构建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

下表说明了在转换的项目和任务中显示哪些问题字段。

| 问题字段 | 项目或任务字段 | 项目列表或报表 | 项目详细信息区域 | 任务列表或报表 | 任务详细信息区域 |
|---|---|---|---|---|---|
| 问题名称 | 转换的问题名称 | ✔ | ✔ | ✔ | ✔ |
| 主要联系人 | 已转换的问题创作者名称 | ✔ | `✔` | ✔ |   |
| 输入日期 | 已转换的发行条目日期 | ✔ |   | ✔ |   |


>[!CAUTION]
>
>如果问题的主要联系人发生更改，或者问题在问题转换后从项目或任务中取消链接，则转换的问题发起者名称不会更新，它会在问题转换时显示问题的原始主要联系人。
