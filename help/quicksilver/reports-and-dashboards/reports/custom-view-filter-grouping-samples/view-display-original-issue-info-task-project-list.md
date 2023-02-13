---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：显示任务和项目列表上的原始问题信息
description: 在任务和项目列表视图中，在将问题转换为列表中的任务和项目 — 编辑我之后，您可以在任务和项目列表视图上显示原始问题的以下信息。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 235156b6-a9b6-484e-b126-54874da705c8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 4%

---

# 查看：显示任务和项目列表上的原始问题信息

在任务和项目列表视图中，在将问题转换为列表中的任务和项目后，您可以在任务和项目列表中显示原始问题的以下信息：

* 转换的问题名称
* 转换的问题输入日期
* 已转换的问题创作者名称

有关使用标准报表生成器创建视图的信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

![task_and_project_list_with_original_issue_info_png](assets/task-and-project-list-with-original-issue-info-350x59.png)

有关在项目和任务列表中包含其他问题信息的详细信息，另请参阅 [查看：任务和项目的原始问题详细信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-originating-issue-details-tasks-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: no longer needed - all fields are now in the UI</p>
<p>Applying this view is identical for tasks and projects.</p>
<p>To apply this view to a task list:</p>
<ol>
<li value="1">Go to a list of tasks which have been converted from issues</li>
<li value="2">From the <strong>View</strong> drop-down menu, select <strong>New View</strong>.</li>
<li value="3">In the<strong>Column Preview</strong> area, eliminate all columns except for one.</li>
<li value="4">Click the header of the remaining column, then click<strong>Switch to Text Mode</strong>.</li>
<li value="5">Mouse over the text mode area, and click <strong>Click to edit text</strong>.</li>
<li value="6"> <p>Remove the text you find in the <strong>Text Mode</strong> box, and replace it with the following code:</p>
<div class="codeSnippet">
<a class="codeSnippetCopyButton" role="button">Copy</a>
<div class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False">
<pre><code>column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.20.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.displayname=Converted Issue Name<br>column.1.linkedname=convertedOpTask<br>column.1.textmode=true<br>column.1.valuefield=convertedOpTaskName<br>column.1.valueformat=HTML<br>column.2.displayname=Converted Issue Entry Date<br>column.2.textmode=true<br>column.2.valuefield=convertedOpTaskEntryDate<br>column.2.valueformat=HTML<br>column.3.displayname=Originator Name<br>column.3.textmode=true<br>column.3.valuefield=convertedOpTaskOriginator:name<br>column.3.valueformat=HTML</code></pre>
</div>
</div> </li>
<li value="7"> Click <strong>Save View</strong>. </li>
</ol>
</div>
-->
