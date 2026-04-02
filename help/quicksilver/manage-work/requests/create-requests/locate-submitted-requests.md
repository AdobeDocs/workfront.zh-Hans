---
product-area: requests
navigation-topic: create-requests
title: 查看已提交的请求
description: 了解Adobe Workfront的各个区域，您可以在其中查看您或其他人提交的请求，或者您从未提交并另存为草稿的请求。
author: Alina
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: f4d7484145226eb85bc547e582438e5202dec023
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 3%

---

# 查看提交的请求

<!--
Remove production and preview references at release
-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以查看自己或其他人提交的请求，或者查看您已开始但从未完成提交的请求。 未完成的请求将另存为草稿。

您可以在Adobe Workfront的以下区域找到已提交的请求：

* Workfront的“请求”区域
* 主页中的“我的请求”构件

请求区域根据您选择的查看方式显示以下请求：

* 使用旧版Experience时的Workfront请求
* 使用新Experience时Workfront以及Planning请求。

  >[!NOTE]
  >
  >* 您只能查看自己的草稿请求。
  >* 在新的请求体验中，提交的请求和草稿可在同一列表中找到。
  >* 在旧版Experience中创建的草稿不会显示在新的“请求体验”中。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何Adobe Workfront或Adobe Workflow包</p> 
   <p>任何Adobe Workfront规划包</p>
   </td> 
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
  <!--
  tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
  -->
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在请求区域查看已提交的请求

您可以在请求区域或主页的“我的请求”小组件中查看已提交的请求。

有关我的请求的信息，请参阅[使用我的请求小组件](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

根据您使用的是新请求体验还是旧请求体验，查看已提交的请求会有所不同。

* [在新的请求体验中查看已提交的请求](#view-submitted-requests-in-the-new-requesting-experience)
* [在旧版中查看已提交的请求请求体验](#view-submitted-requests-in-the-legacy-requesting-experience)

### 在新的请求体验中查看已提交的请求

>[!NOTE]
>
>* 如果您有Workfront Planning，则Workfront和Planning请求将显示在同一列表中。 Workfront请求在`Issue`对象类型&#x200B;**列中显示**&#x200B;值。
>* 默认情况下，请求区域的列表中最多显示50个请求。 要查看更多请求，请滚动到列表底部。

您可以在请求区域以及主页的“我的请求”小组件中查看已提交的请求。

>[!NOTE]
>
>当您启用新的请求体验时，以下对象具有来自请求区域和我的请求小组件中的请求列表的链接：
>
>* “主题”字段中的Planning和Workfront请求。
>* 从“创建的对象”字段中的Planning请求创建的Planning记录。
>* 在预览环境的对象创建字段中，从Workfront请求转换的<span class="preview">Workfront任务和问题。</span>

要查看您或其他用户在新的请求体验中提交的请求，请执行以下操作：

{{step1-to-requests}}

1. 确保打开了屏幕右上角的&#x200B;**使用新体验**&#x200B;设置。

   此时将显示请求列表。

1. （可选）要搜索请求，请开始在列表右上角的搜索栏中键入。 搜索结果会随键入内容一起显示。
1. （可选）要管理信息在请求列表中的显示方式，请更新列表的以下视图元素：

   * 视图
   * 筛选条件
   * 列

   <div class="preview">

   * 组
   * 设置单元格的格式
   * 行高

   </div>

   有关管理请求列表中的信息的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

1. （可选）通过检查&#x200B;**状态**&#x200B;列来检查请求的状态。 新请求体验中提供了以下状态：

   * **草稿**：此请求尚未提交。
   * **等待审阅**： （仅限Planning）此请求具有批准者，并且没有批准者打开该请求。
   * **审核中**：（仅限Planning）此请求有批准者，且至少有一个批准者已打开该请求，但尚未做出任何决定。
   * **已拒绝**： （仅限Planning）此请求具有审批者且已被拒绝。 此请求将不会创建记录。
   * **正在进行**：
      * Workfront请求：请求已转换，工作正在进行。
      * Workfront Planning请求：请求完成映射至特定的Planning字段，并且该字段值与完成值不匹配。

        有关详细信息，请参阅在Adobe Workfront Planning中创建和管理请求表单一文中的[设置配置详细信息](/help/quicksilver/planning/requests/create-request-form.md#set-up-configuration-details)。
   * **完成**：请求已完成。

### 在旧版中查看已提交的请求请求体验

要查看您或其他用户在旧版请求体验中提交的请求，请执行以下操作：

{{step1-to-requests}}

1. （视情况而定）如果您的组织购买了Workfront规划包，请单击&#x200B;**Workfront**&#x200B;选项卡以查看Workfront请求。
1. 单击左侧面板中的&#x200B;**已提交**&#x200B;以查看所有已提交的请求。

   您最多可以查看2000个请求，并且这些请求可以显示在多个页面上。

   >[!TIP]
   >
   >您无法自定义已提交的请求列表中的列。

   ![已提交请求新列表](assets/nwe-submitted-requests-new-list-350x57.png)


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

1. （可选）在列表中选择请求，然后单击&#x200B;**打开摘要**&#x200B;图标![打开包含文本的摘要](assets/open-summary-with-text-nwe.png)以打开“摘要”面板并显示有关该请求的其他信息、添加注释、文档或分配该请求。 有关摘要面板的信息，请参阅[摘要概述](../../../workfront-basics/the-new-workfront-experience/summary-overview.md)。

   >[!TIP]
   >
   >如果“摘要”面板已经打开，则“打开摘要”图标将变为“关闭摘要”。

1. （可选且有条件）单击右上角的&#x200B;**X**&#x200B;图标或&#x200B;**关闭摘要**&#x200B;图标![关闭包含文本的摘要](assets/close-summary-with-text-nwe.png)以关闭摘要面板。

   如果问题被转换为任务或项目，并且该问题在转换过程中被删除，则“摘要”面板为空白。 有关转换问题的信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. 从列表右上角的&#x200B;**过滤器图标** ![过滤器图标](assets/filter-nwepng.png)中，选择下表中列出的任何过滤器。

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

1. （可选）单击列表顶部的&#x200B;**筛选器页面**&#x200B;图标![搜索图标](assets/search-icon.png)以按名称搜索请求。 列表会更新为符合搜索条件的结果。

   <!--

   1. (Conditional) To display only Workfront Request queues, search or filter for `Issue` object types.</span>
   -->

   <!--
   <li> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li>(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
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

   <!--
   Planning tab has been removed and no longer visible in legacy Requests area: 
   (Optional and conditional) If your organization purchased a Workfront Planning package, click the **Planning** tab, then click **Submitted** in the left panel to view Workfront Planning requests. 
      Use **Filters** and **Columns** to update the information in the Planning request list. 
      ![Planning tab submitted section in Requests area](assets/workfront-planning-tab-submitted-section-in-requests-area.png)
      For information, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md).
   -->


1. （可选）通过检查&#x200B;**状态**&#x200B;列来检查请求的状态。 新请求体验中提供了以下状态：

   * **草稿**。 此请求尚未提交。
   * **正在进行中**
   * **完成**


