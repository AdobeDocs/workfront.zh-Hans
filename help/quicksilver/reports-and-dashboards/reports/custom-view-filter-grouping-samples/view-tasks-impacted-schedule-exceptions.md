---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：受计划例外影响的任务'
description: 此任务视图标识由于周末、个人休息时间或其他计划例外而必须延迟完成的任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 0%

---

# 视图：受计划例外影响的任务

此任务视图标识由于周末、个人休息时间或其他计划例外而必须延迟完成的任务。

此视图显示以下内容：

* 任务持续时间
* 任务的计划开始日期和计划完成日期
* 任务的持续时间，根据任务的计划开始日期和计划完成日期之间的天数（日历持续时间）
* 任务开始时，项目计划内的天数（日历开始日期）
* 任务的周日期长根据任务的计划开始日期和计划完成日期之间的工作日数（周日期长）
* 如果“工作日”持续时间大于任务的持续时间（这表示任务持续时间中存在例外天数），则任务将标记为“例外”。\
  ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## 查看受计划例外影响的任务

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column(name){name){name.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.listsort=intAsInt(duration)<br>分钟column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.widationkey=80<br>column.2.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br> column.2.listsort=atDateAsAtDate(plannedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=plannedStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=plannedStartDate<br>column.2.widate=at<br>column.2.width=80<br> descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=plannedCompletionDate<br>column.3.short=false<br>column.3.3.valuefield=plannedComplection<br>column 3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({plannedCompletionDate}，<br>{plannedStartDate})+1<br>column.4.aggregaggregator.valueformat.valueformat=intAsIntAsInt<br>column.4}column.4.descrin.descript ptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({plannedCompletionDate}，{plannedStartDate})+1<br>column.4.valueformat=int<br>column.column.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({plannedStartDate}，{project}。<br><br><br>{plannedStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=日历开始日期<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF({plannedStartDate}，{project}。{plannedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({plannedStartDate}，<br>{plannedCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey.descriptionkey.descriptionkey.descriptionkey.key.descriptionkey.description=id=id=id=id{id{id{id{12 {column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.widain.8.wida 0<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate}))&gt;({duration}/480)，"Exception"，")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.valueformat=HTML{3.linkedname=direct{direct 2}column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({plannedStartDate}，{plannedCompletionDate}))&gt;({duration}/480)，“异常”，“”)<br>column.7.valueformat=HTML 42}column.7.width=80<br><br><br><br></pre>

1. 单击&#x200B;**保存视图**。
