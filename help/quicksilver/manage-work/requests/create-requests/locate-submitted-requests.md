---
product-area: requests
navigation-topic: create-requests
title: 查找已提交的请求
description: 了解Adobe Workfront的各个区域，您可以在这些区域找到您或其他人提交的请求，或者您从未提交并另存为草稿的请求。
author: Becky
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: ebdb1803fe57386a84d3d882b02a53ec4344b225
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 2%

---

# 查找已提交的请求


您可以找到您或其他人提交的以下类型的请求，或者您已开始但从未完成提交的请求。 您可以在Adobe Workfront的以下区域中找到这些请求：

* Workfront中“请求”区域的&#x200B;**Workfront**&#x200B;选项卡：请在以下部分中查找提交到Workfront请求队列的请求：
   * **已提交节**：您或其他人提交的所有请求，您至少有权查看。
   * **草稿部分** ：您已开始但从未完成且从未提交的所有请求。 有关草稿请求的更多信息，请参阅[创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

  >[!TIP]
  >
  >您只能查看自己的草稿请求。

* Workfront中“请求”区域的&#x200B;**计划**&#x200B;选项卡：找到提交到Workfront计划请求表单的请求。 贵组织必须购买Workfront规划包。 有关信息，请参阅以下文章：

   * [在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)
   * [提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>编辑对问题的访问权限</p></td> 
  </tr>
  <tr>
   <td role="rowheader">对象权限</td> 
   <td><p>查看请求中的权限或更高版本</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 产品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必须拥有Adobe Workfront Planning才能查看Planning请求或请求表单</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查找已提交的请求

根据您使用的是新请求体验还是旧请求体验，查找已提交的请求会有所不同。

### 在新请求体验中找到已提交的请求

要查找您或其他用户在新的请求体验中提交的请求，请执行以下操作：

{{step1-to-requests}}

1. 请确保已启用屏幕右上角的&#x200B;**使用新体验**&#x200B;切换开关。

   此时将显示“请求”列表。

1. （可选）要搜索请求，请开始在列表右上角的搜索栏中键入。 搜索结果会随键入内容一起显示。
1. （可选）单击&#x200B;**筛选器**&#x200B;并开始为要查找的请求添加条件。

   您可以按以下字段进行筛选：

   * **Workspace**：与请求表单关联的工作区。
   * **记录类型**：与请求表单关联的记录类型。
   * **输入日期**：提交请求的日期。
   * **请求表单**：用于提交请求的请求表单的名称。
   * **状态**：请求的状态。
   * **输入者**：添加请求的用户的名称。 如果请求是由Workfront之外的人员添加的，则&#x200B;**输入者**&#x200B;字段显示`N/A`。

   您可以有多个&#x200B;**And**&#x200B;或&#x200B;**Or**加入的筛选器。
在添加筛选条件时，将自动筛选请求列表。
1. （可选）使用视图来关注要查找的请求。

   有关说明，请参阅[在请求区域](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md)中创建或编辑视图。

>[!NOTE]
>
>* 如果您有Workfront Planning，则Workfront和Planning请求将显示在同一列表中。 Workfront请求在“对象类型”列中显示值`Issue`。
>* 此时将显示请求列表，其中显示50个请求。 要查看更多请求，请滚动到列表底部。

### 在旧版请求体验中查找已提交的请求

要查找您或其他用户在旧版请求体验中提交的请求，请执行以下操作：

{{step1-to-requests}}

1. （视情况而定）如果您的组织购买了Workfront规划包，请单击&#x200B;**Workfront**&#x200B;选项卡以查看Workfront请求。
1. 单击左侧面板中的&#x200B;**已提交**&#x200B;以查看所有已提交的请求。

   您最多可以查看2000个请求，并且这些请求可以显示在多个页面上。

   >[!TIP]
   >
   >您无法自定义已提交的请求列表中的列。

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. 默认情况下，将显示以下列：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">名称</td> 
         <td> <p>请求的名称。</p> <p>单击请求的名称以将其打开。 </p> <p><b>提示</b>

   如果问题在转换为任务或项目时未保留，则问题的名称会变暗且无法再单击。 有关转换问题的信息，请参阅<a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">在Adobe Workfront中转换问题的概述</a>。 </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">已转换为</td> 
         <td> <p>解析对象的名称，该对象可以是请求已转换为的任务或项目。 </p> <p>单击任务或项目的名称以将其打开。 </p> <p>如果未转换请求，则此字段为空。 </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">路径</td> 
         <td>最初提交请求的请求队列、主题组和队列主题的名称。 </td> 
      </tr> 
      <tr> 
         <td role="rowheader">状态</td> 
         <td>请求或解析对象（任务或项目）的当前状态</td> 
      </tr> 
      <tr> 
         <td role="rowheader">输入日期</td> 
         <td>提交请求的日期或解决对象的创建日期（如果请求在转换时被删除）。 </td> 
      </tr> 
      <tr> 
         <td role="rowheader">上次更新日期</td> 
         <td> <p>上次更新请求的日期。</p> <p>默认情况下，提交的请求列表将按此字段排序。 </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. （可选）单击列的标题可按列进行排序。

   >[!TIP]
   >
   >当您离开提交的请求列表时，所选的排序选项会保留。

1. （可选）在列表中选择请求，然后单击&#x200B;**打开摘要**&#x200B;图标![](assets/open-summary-with-text-nwe.png)以打开“摘要”面板并显示有关该请求的其他信息、添加注释、文档或分配它。 有关摘要面板的信息，请参阅[摘要概述](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)。

   >[!TIP]
   >
   >如果“摘要”面板已经打开，则“打开摘要”图标将变为“关闭摘要”。

1. （可选且有条件）单击右上角的&#x200B;**X**&#x200B;图标或&#x200B;**关闭摘要**&#x200B;图标![](assets/close-summary-with-text-nwe.png)以关闭摘要面板。

   如果问题被转换为任务或项目，并且该问题在转换过程中被删除，则“摘要”面板为空白。 有关转换问题的信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. 从列表右上角的&#x200B;**筛选器图标** ![](assets/filter-nwepng.png)中，选择下表中列出的任何筛选器。

   >[!TIP]
   >
   >您不能在请求区域的已提交分区中修改筛选器。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部</td> 
      <td>所有已提交的请求，无论状态或提交者如何。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Open</td> 
      <td> <p>当前打开的所有已提交请求，无论这些请求的提交者是谁。 只有您至少拥有查看权限的请求才会显示在此处（如果您没有自己提交这些请求）。 </p> <p>不具有实际完成日期或其解析对象不具有实际完成日期的请求将列在打开子选项卡中。</p> <p><b>提示</b>

   处于任何不等于“已关闭”状态的请求均被视为未完成。</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">我的请求</td> 
      <td>您提交的请求，不考虑其状态。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">我的未结请求</td> 
      <td> <p>您提交的请求仍然处于打开状态。 </p> <p>不具有实际完成日期或其解析对象不具有实际完成日期的请求将列在我的打开请求子选项卡中。 </p> <p><b>提示</b>

   未处于已关闭状态的请求会被视为未完成。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. （可选）单击列表顶部的&#x200B;**筛选器页面**&#x200B;图标![](assets/search-icon.png)以按名称搜索请求。 列表会更新为符合搜索条件的结果。

1. （视情况而定）要仅显示Workfront请求队列，请搜索或筛选`Issue`对象类型。</span>


   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. 单击&#x200B;**草稿**&#x200B;查看所有草稿的请求。 Workfront会为此文件夹中的每个请求队列保存无限数量的草稿。 为已具有草稿的队列主题输入新请求时，系统将提示您使用现有的草稿。 有关详细信息，请参阅[从草稿创建请求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)。

1. （可选且有条件）如果贵组织购买了Workfront Planning包，请单击&#x200B;**Planning**&#x200B;选项卡，然后单击左侧面板中的&#x200B;**Submitted**&#x200B;以查看Workfront Planning请求。

   使用&#x200B;**筛选器**&#x200B;和&#x200B;**列**&#x200B;更新Planning请求列表中的信息。

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   有关信息，请参阅[提交Adobe Workfront计划请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)。


