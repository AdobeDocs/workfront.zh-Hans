---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：前置任务详细信息'
description: 此任务视图使用收藏集视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关处于“一对多”关系中的对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务名称，以及其前置任务名称、前置任务项目名称、前置任务计划完成日期和前置任务状态。
author: Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 查看：前置任务详细信息

<!--Audited: 11/2024-->

此任务视图使用收藏集视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关处于“一对多”关系中的对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务名称，以及其前置任务名称、前置任务项目名称、前置任务计划完成日期和前置任务状态。

有关在报表中引用集合的信息，请参阅[在报表中引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

![前置任务详细信息_task_view.png](assets/predecessor-details-task-view-350x34.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p> 当前： 
   <ul>
   <li>请求修改视图</li> 
   <li>计划修改报告</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改视图的参与者</li> 
   <li>用于修改报告的标准</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看前置任务详细信息

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   column.0.displayname=
   column.0.linkedname=direct
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.1.displayname=Predecessors Numbers & Names
   column.1.listdelimiter=
   column.1.listmethod=nested(predecessors).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})
   column.1.valueformat=HTML
   column.2.displayname=Predecessors Project Names
   column.2.listdelimiter=
   column.2.listmethod=nested(predecessors).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={predecessor}.{project}.{name}
   column.2.valueformat=HTML
   column.3.displayname=Predecessors Completion Dates
   column.3.listdelimiter=
   column.3.listmethod=nested(predecessors).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={predecessor}.{plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Predecessors Status
   column.4.listdelimiter=
   column.4.listmethod=nested(predecessors).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={predecessor}.{status}
   column.4.valueformat=HTML
   ```

1. 单击&#x200B;**完成** > **保存视图**。
