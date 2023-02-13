---
navigation-topic: use-lists
title: 开始使用 [!DNL Adobe Workfront]
description: 您可以在 [!DNL Adobe Workfront] 以获取有关这些对象的信息，如它们的开始日期和到期日期、分配给它们的用户以及与其关联的其他对象。
feature: Get Started with Workfront
author: Lisa
exl-id: d4262b8e-bbe0-4ac2-8f1f-5d32541311c8
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '2370'
ht-degree: 0%

---

# 开始使用 [!DNL Adobe Workfront]

<!--
{{highlighted-preview}}
-->

您可以在 [!DNL Adobe Workfront] 以获取有关这些对象的信息，如它们的开始日期和到期日期、分配给它们的用户以及与其关联的其他对象。

以下是 [!DNL Workfront]:

* 列表每五分钟自动刷新一次，以更新系统中其他用户正在在其他位置更新的信息。
* 中的某些区域 [!DNL Workfront] 预配置了默认对象列表。

   您可以自定义这些预配置列表中的大多数。

* A [!DNL Workfront] 管理员可以创建自定义列表以应用于各个区域 [!DNL Workfront].

   有关创建系统级别列表的详细信息，请参阅文章 [创建、编辑和共享默认过滤器、视图和分组](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL请求]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL视图]或更高版本对过滤器、视图、分组的访问权限</p> <P>对于[!UICONTROL设置]区域中的项目，您需要对该项目或[!UICONTROL系统管理员]访问级别拥有管理访问权限。</P> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。<br>有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>[!UICONTROL视图]或拥有共享访问权限的更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 对象列表

下面是一些类型的对象列表，您可以在 [!DNL Workfront] 以及您有权查看对象时默认显示的某些区域。

>[!NOTE]
>
>* 此列表不完整。 其中每个对象列表也可显示在报表或功能板上。 例如，项目报表或包含项目报表的功能板也会显示项目列表。
>* 在此列表中，“select”表示您需要单击项目的名称，而不是名称左侧的复选框。



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!DNL Workfront] 列表</strong></th> 
   <th><strong>对象列表的位置</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>组合列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROLPortfolio]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>方案列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROLPortfolio] &gt;[!UICONTROL选择一个项目组合] &gt;[!UICONTROL程序]</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL程序]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>项目列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目]</p> </li> 
     <li> <p>[!UICONTROLPortfolio] &gt;[!UICONTROL选择一个项目组合] &gt;[!UICONTROL项目]</p> </li> 
     <li> <p>[!UICONTROLPortfolio] &gt;[!UICONTROL选择项目组合] &gt; [!UICONTROL程序] &gt;[!UICONTROL选择项目] &gt;[!UICONTROL项目]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>任务列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt;[!UICONTROL子任务]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt; [!UICONTROL前置任务*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>问题列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目] &gt; [!UICONTROL选择]项目&gt;[!UICONTROL问题]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt; [!UICONTROL问题]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt; [!UICONTROL子任务] &gt;[!UICONTROL选择任务] &gt; [!UICONTROL问题]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>报告列表</td> 
   <td> 
    <ul> 
     <li> <p>  [!UICONTROL报表]  </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>功能板列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL功能板]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>迭代列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams] &gt; [!UICONTROL Iterations]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>用户列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL用户]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>文件列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL文档]</p> </li> 
     <li> <p>[!UICONTROLPortfolio] &gt;[!UICONTROL选择组合] &gt; [!UICONTROL文档]</p> </li> 
     <li> <p>[!UICONTROLPortfolio] &gt; [!UICONTROL选择项目组合] &gt; [!UICONTROL程序] &gt;[!UICONTROL选择程序] &gt;[!UICONTROL文档]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt;[!UICONTROL文档]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt; [!UICONTROL文档]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt; [!UICONTROL选择]项目&gt; [!UICONTROL问题] &gt;[!UICONTROL选择问题] &gt; [!UICONTROL文档]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>工时单列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL时间表] s &gt; [!UICONTROL所有时间表]*</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>计费费率列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL选择一个项目] &gt;[!UICONTROL开单费率*]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>帐单记录列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目] &gt; [!UICONTROL选择项目] &gt; [!UICONTROL账单记录]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>风险列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL选择一个项目] &gt;[!UICONTROL Risks]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>费用清单</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projects] &gt;[!UICONTROL选择]项目&gt;[!UICONTROL Expenses]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt; [!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt;[!UICONTROL费用]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>小时条目列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择]项目</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择项目] &gt; [!UICONTROL任务] &gt;[!UICONTROL选择任务] &gt;[!UICONTROL小时]</p> </li> 
     <li> <p>[!UICONTROL项目] &gt;[!UICONTROL选择]项目&gt;[!UICONTROL问题] &gt;[!UICONTROL选择]问题&gt;[!UICONTROL小时]</p> </li>
    </ul> </td> 
  </tr>
  <tr> 
   <td class="preview">自定义表单列表</td> 
   <td> 
    <ul> 
     <li class="preview"> <p>[!UICONTROL设置] &gt;[!UICONTROL自定义Forms]</p>
     <!--Remove the following note box when this goes to Production. Or do this when the Preview highlighting becomes available.-->
     <p><b>注意</b>:当前仅在预览环境中可用</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>组或子组列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL设置] &gt;[!UICONTROL组]</p> </li>
     <li> <p>[!UICONTROL设置] &gt;[!UICONTROL组] &gt;[!UICONTROL选择父组] &gt;[!UICONTROL子组] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>团队列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Teams]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>公司列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Setup] &gt;[!UICONTROL Companys]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>计划列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL设置] &gt;[!UICONTROL计划]</p> </li> 
    </ul> </td> 
  </tr>
  <tr> 
   <td>布局模板列表</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL设置] &gt;[!UICONTROL布局模板]</p> </li> 
    </ul> </td> 
  </tr>
 </tbody> 
</table>

无法在指定区域上自定义列表。 A [!DNL Workfront] 管理员可以在系统级别构建自定义列表，或者如果您的访问级别允许您访问编辑报表，则可以为此对象构建报表。

## 列表元素

列表包含定义其格式的某些元素以及显示的信息。 您可以找到几个默认可用的系统列表元素。 您还可以创建自定义元素以满足您的需求。

>[!NOTE]
>
>从列表中选择新过滤器、查看或分组时，即使您注销，该选择也会保留 [!DNL Workfront] 或关闭浏览器。

以下是列表的元素：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>元素</strong></th> 
   <th><strong>说明</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL过滤器]</strong></td> 
   <td> <p>过滤器会根据您指定的条件将不必要的信息排除在列表之外。 </p> <p>有关更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">过滤器概述 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL视图]</strong></td> 
   <td> <p>视图定义在屏幕上显示的字段（列）。</p> <p>有关更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">视图概述 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL分组]</strong></td> 
   <td> <p>根据您指定的条件，按区域对列表中的对象进行分组。</p> <p>例如，列表中的问题可以按状态或优先级以部分显示。</p> <p>在标准分组中最多可以有三层分组，如果在文本模式下配置分组，则可以添加第四层。</p> <p>有关分组的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">中的分组概述 [!DNL Adobe Workfront]</a>.</p> <p>有关文本模式的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文本模式概述</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

默认情况下，这些元素会显示在每个列表的顶部。 它们是粘滞的，在您滚动列表时不会移动。 将鼠标悬停在每个元素的图标上以标识它们。

![](assets/nwe-list-elements.png)

您可以在以下区域中自定义列表元素，并将其与其他用户共享：

* 在部分中找到任何系统默认列表 [开始使用 [!DNL Adobe Workfront]](#default-workfront-lists) 在本文中
* 与您共享的任何报表

列表的构建元素与报表的构建元素相同。

有关创建和自定义列表和报表构建元素的更多信息，请参阅 [报表元素：过滤器、视图和分组](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## 列出操作

您可以在列表中完成以下操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong></th> 
   <th><strong>信息</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>内联编辑</strong> </td> 
   <td> <p>直接在列表中编辑对象及其信息。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md" class="MCXref xref">在 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><strong>使用[!UICONTROL摘要]进行更新</strong> </td> 
   <td> <p>使用[!UICONTROL Summary]面板更新项目级别的任务和问题。</p> <p>提示：摘要并非适用于所有对象，也在“任务”或“问题”报表中不可用。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">概要概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>自定义列表显示</strong> </td> 
   <td> <p>自定义列表、列排列、项目排序顺序或显示项目数的外观。</p> <p>注意：当您注销时，您对页面上要显示的项目数量所做的更改将会恢复 [!DNL Workfront] 或关闭浏览器。 更改也可能会在8小时后恢复。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/use-lists/modify-list-display.md" class="MCXref xref">修改列表的显示方式</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>快速筛选</strong> </td> 
   <td> <p>应用快速过滤器，以仅查找对您很重要的项目，以便您可以快速查看、更新或与他人共享这些项目。</p> <p>重要信息：您可以使用快速过滤器查找包含搜索词的项目，无论该项目是在屏幕上可见，还是在您滚动到页面底部后会显示。 使用浏览器的搜索功能时，您只能找到屏幕上已显示的项目。 如果您的列表包含多个页面，则快速过滤器只会查找当前页面上的项目。</p> <p>有关更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">将快速过滤器应用到列表</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>导出</strong> </td> 
   <td> <p>从导出对象列表 [!DNL Workfront]. 当列表包含的项目超过2000个时，导出列表是查看某个页面上所有项目的唯一方法。</p> <p>有关导出列表的更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/use-lists/export-lists.md" class="MCXref xref">导出列表</a>. 有关导出格式和限制的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">导出数据</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 列表工具栏

下表列出了工具栏中的许多可用图标，并指明了单击这些图标后会出现的情况：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>图标</strong></td> 
   <td><strong>描述</strong></td> 
   <td><strong>单击</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/add-icon-plus-in-circle.png"> </td> 
   <td>[!UICONTROL添加项目或用户]</td> 
   <td>打开更多选项，包括添加新项目或用户。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-above-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL在上面插入任务]</td> 
   <td> <p>在选定任务上方插入任务。</p> <p>此设置仅适用于任务。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-insert-task-below-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL在下面插入任务]</td> 
   <td> <p>在选定任务下方插入任务。</p> <p>此设置仅适用于任务。 </p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/edit-icon.png"> </td> 
   <td>[!UICONTROL编辑]</td> 
   <td>编辑所选项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/copy-icon.png"> </td> 
   <td>[!UICONTROL Copy]</td> 
   <td>复制所选项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/delete.png"> </td> 
   <td>[!UICONTROL Delete]</td> 
   <td>删除选定项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-add-to-iteration-icon-in-new-toolbar-for-issues.png"> </td> 
   <td>[!UICONTROL添加到]</td> 
   <td> <p>打开对话框，将所选问题添加到小版本。</p> <p>此选项仅适用于问题。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/share-icon.png"> </td> 
   <td>[!UICONTROL共享]</td> 
   <td>共享选定项目。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-indent-outdent-tasks-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL缩进和偏移任务] </td> 
   <td> <p>缩进或退出所选任务。 </p> <p>此设置仅适用于任务。 </p> </td> 
  </tr> 
  <tr> 
   <td><img src="assets/more-icon.png"></a> </td> 
   <td>[!UICONTROL更多]</td> 
   <td>打开选定项目的其他选项。</td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/search-icon.png"> </p> </td> 
   <td> <p>[!UICONTROL快速过滤器] </p> </td> 
   <td> <p>打开快速过滤器搜索框，查找显示列表中的项目。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/export.png"> </td> 
   <td>[!UICONTROL导出]</td> 
   <td>将列表导出为PDF、Excel或制表符分隔的文件。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-agile-icon-in-new-toolbar-task-list.png"> </td> 
   <td>[!UICONTROL Agile View]</td> 
   <td>在Agile视图中显示列表。<br>此设置仅适用于任务。</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/qs-gantt-chart-icon-in-new-toolbar.png"> </td> 
   <td>[!UICONTROL甘特图]</td> 
   <td> <p>在[!UICONTROL甘特图]视图中显示列表。</p> <p>该设置仅适用于项目和任务。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-filter-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-filter-in-new-toolbar-with-blue-dot---small.png"> </p> </td> 
   <td>[!UICONTROL过滤器]下拉菜单</td> 
   <td> <p>显示过滤器列表以及用于管理过滤器的其他选项，包括创建过滤器。 </p> <p>在小屏幕上，过滤器名称将被替换为过滤器图标。 当您应用“[!UICONTROL All]”以外的任何过滤器时，“过滤器”图标上会显示一个蓝色圆点。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-view-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-view-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL视图]下拉菜单</td> 
   <td> <p>显示用于管理视图的视图列表和其他选项，包括创建一个视图。 </p> <p>在小屏幕上，视图名称将被替换为[!UICONTROL视图]图标。 当您应用“[!UICONTROL Standard]”以外的任何视图时，[!UICONTROL视图]图标上会显示一个蓝色圆点。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-grouping-in-new-toolbar-with-name.png"> <p> <img src="assets/qs-grouping-in-new-toolbar-with-blue-dot.png"> </p> </td> 
   <td>[!UICONTROL Grouping]下拉菜单</td> 
   <td> <p>显示分组列表以及用于管理分组的其他选项，包括创建分组。 </p> <p>在小屏幕上，“分组”名称将被替换为[!UICONTROL分组]图标。 当您应用“[!UICONTROL Nothing]”以外的任何分组时，[!UICONTROL Grouping]图标上会显示一个蓝色圆点。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <img src="assets/qs-autosave-icon-in-new-toolbar-for-tasks.png"> </td> 
   <td> <p>[!UICONTROL计划模式]</p> </td> 
   <td> <p>选择要自动还是手动保存在任务列表中所做的更改。 </p> <p>有关在列表中编辑任务的信息，请参阅 <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">在列表中编辑任务</a>. </p> <p>此设置仅适用于任务。</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/summary-panel-icon.png"> </td> 
   <td>[!UICONTROL摘要]</td> 
   <td> <p>显示或隐藏选定项目的[!UICONTROL摘要]框。</p> <p>此功能仅适用于任务和问题。</p> <p>有关新 [!DNL Adobe Workfront] 体验，请参阅 <a href="/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md" class="MCXref xref">概要概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/remove-icon---x-in-circle.png"> </td> 
   <td>[!UICONTROL Remove]</td> 
   <td>从列表中删除某些内容。 例如，作为管理组或子组成员关系的组管理员，请删除组成员，如 <a href="/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md" class="MCXref xref">查看和管理群组成员关系</a>.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/comment-icon.png"> </td> 
   <td>[!UICONTROL Comment] /[!UICONTROL Update]</td> 
   <td> <p>键入评论或更新。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 列表和报表之间的差异

列表和报表都是包含对象类型信息的网格。

下表概述了列表和报表之间的相似之处和差异：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>功能</strong> </th> 
   <th><strong>列表</strong> </th> 
   <th><strong>报告</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>任何人都可以创建它们</p> </td> 
   <td><span>✓*</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>仅a [!DNL Workfront] 拥有[!UICONTROL Plan]许可证的管理员和用户可以创建他们</p> </td> 
   <td> </td> 
   <td>✓**</td> 
  </tr> 
  <tr> 
   <td> <p>默认集可从 [!DNL Workfront]</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>可在标准模式下自定义</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>可在文本模式下自定义</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以与其他用户共享它们</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以在系统范围内共享它们</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>您可以在系统外部共享这些内容</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>您可以导出为.pdf， [!DNL Excel]和制表符分隔格式</p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
  </tr> 
  <tr> 
   <td> <p>您可以计划在电子邮件中进行提交</p> </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p>您可以向布局模板添加</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>您可以将它们添加到自定义部分 </p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以将其添加到功能板</p> </td> 
   <td> ✓*** </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以使用提示自定义显示的内容</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以在图表中显示它们</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>您可以在其中内联编辑对象</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

您必须有权访问过滤器、视图和分组才能创建它们。 有关更多信息，请参阅 [授予对过滤器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

您必须有权访问过滤器、视图和分组以及报表、功能板和日历，才能创建它们。 有关更多信息，请参阅 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

仅当报表的创建者已将列表元素配置为在功能板上可见时，才能自定义置于功能板中的报表的列表。

>[!NOTE]
>
>如果没有创建报表并先将其添加到功能板，则无法向功能板添加列表。

有关构建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). 有关创建自定义部分的信息，请参阅 [创建自定义选项卡或区域](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

## 更新列表与旧版列表之间的差异

在 [!DNL Workfront]:

* 旧版列表

   ![](assets/legacy-list-screen-shot-blue-groupings-350x101.png)

* 更新的列表

   ![](assets/updated-list-screen-shot-gray-groupings-350x71.png)

这两种类型的列表都显示在 [!DNL Adobe Workfront].

中的所有列表和报表 [!DNL Adobe Workfront] 列表已更新，但以下情况除外：

* 列表 [!UICONTROL 设置] 面积
* 列表 [!UICONTROL 报表] 面积

下表显示了 [!DNL Workfront]:

<!--
<span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> [Legacy does not equal Classic. Legacy lists appear in NWE and Classic. Updated lists appear in NWE and Classic.]</span>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>旧版列表</b></td> 
   <td><b>更新的列表</b></td> 
  </tr> 
  <tr> 
   <td> <p>旧字体、列标题、蓝色分组颜色方案</p> </td> 
   <td> <p>更新了字体、列标题、灰色分组颜色方案</p> </td> 
  </tr> 
  <tr> 
   <td> <p>内联编辑速度较慢</p> </td> 
   <td> <p>更快的内联编辑</p> </td> 
  </tr> 
  <tr> 
   <td> <p>显示 <strong>100</strong> 默认情况下为项目</p> </td> 
   <td> <p>显示 <strong>全部</strong> 或 <strong>2000年</strong> 默认情况下为项目</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用CTRL+F在列表中查找项目</p> </td> 
   <td> <p>使用快速过滤器快速查找大型列表中的信息</p> <p>有关在列表中使用快速过滤器的信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md" class="MCXref xref">将快速过滤器应用到列表</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>不能使用富文本格式在内联编辑自定义字段。</td> 
   <td> <p>可以将具有格式的自定义字段中的文本配置为允许粗体、斜体、下划线、项目符号、编号、超链接和块引号。</p> <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>条件格式可以更改列表中链接的文本颜色</td> 
   <td>无法将文本颜色更改应用于列表中的链接</td> 
  </tr> 
 </tbody> 
</table>
