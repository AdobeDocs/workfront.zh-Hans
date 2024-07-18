---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：前置任务详细信息'
description: 此任务视图使用收藏集视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关处于“一对多”关系中的对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务名称，以及其前置任务名称、前置任务项目名称、前置任务计划完成日期和前置任务状态。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 查看：前置任务详细信息

此任务视图使用收藏集视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关处于“一对多”关系中的对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务名称，以及其前置任务名称、前置任务项目名称、前置任务计划完成日期和前置任务状态。

有关在报表中引用集合的信息，请参阅[在报表中引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

![前置任务详细信息_task_view.png](assets/predecessor-details-task-view-350x34.png)

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
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 查看前置任务详细信息

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=前置任务编号和名称<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested（前置任务）。lists<br>column.1.textmode=true<br>column.1.type=iterate{1.1.valuterate<br>column.valustamin.valuuuuuustation.1 eexpression=CONCAT({predecessor}.{taskNumber}，' - '，{predecessor}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=前置任务项目名称<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors)。lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecessor}。{project}。{name}<br>column.2.valueformat=HTML<br>column.3.displayname=前置任务完成日期<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors)。lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecessor}。{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=前置任务状态<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested（前置任务）。lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}。{status}<br>column.4.valueformat=HTML</pre>

1. 单击&#x200B;**保存视图**。
