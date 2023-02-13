---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：前置详细信息
description: 此任务视图使用集合视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关“一对多”关系中对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务的名称及其前置任务名称、前置任务项目名称、前置任务的计划完成日期和前置任务状态。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 查看：前置详细信息

此任务视图使用集合视图显示任务的前置任务的详细信息。 在收藏集视图中，您可以显示有关“一对多”关系中对象的信息。 在这种情况下，每个任务（一个）可以有多个前置任务（多个）。 该视图显示任务的名称及其前置任务名称、前置任务项目名称、前置任务的计划完成日期和前置任务状态。

有关在报表中引用收藏集的信息，请参阅 [在报表中引用集合](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![prepisent_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 查看前置任务详细信息

1. 转到任务列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Precessors Numbers &amp; Names<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(precessors)。lists<br>column.1.textmode=true<br>column.1.type=interate<br>column.1.valueexpression=CONCAT({pricessment})。{taskNumber},' - ',{prepisent}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Precessors项目名称<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(precessors)。lists<br>column.2.textmode=true<br>column.2.type=interate<br>column.2.valueexpression={pricessent}。{项目}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Precessors完成日期<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(precessors)。lists<br>column.3.textmode=true<br>column.3.type=interate<br>column.3.valueexpression={pricessment}。{planedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Precessors Status<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(precessors)。lists<br>column.4.textmode=true<br>column.4.type=interate<br>column.4.valueexpression={pricessent}。{status}<br>column.4.valueformat=HTML</pre>

1. 单击 **保存视图**.
