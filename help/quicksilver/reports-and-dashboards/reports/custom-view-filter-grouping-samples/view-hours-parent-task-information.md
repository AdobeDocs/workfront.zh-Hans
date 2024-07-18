---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：包含父任务信息的小时数'
description: 此小时视图显示记录小时数的任务的名称以及父任务的名称。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# 查看：包含父任务信息的小时数

此小时视图显示记录小时数的任务的名称以及父任务的名称。

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## 查看包含父任务信息的小时

1. 转到小时列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.0.aggregator.displayformat=doubleAsString<br>column.0.aggregator.function=SUM<br>column.0.aggregator.namekey=hours<br>column.0.aggregator.valuefield=hours<br>column.0.aggregator.valueformat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.link.link.link.linkproperty.0.0.name.name.name.name=ID{ID<br>column.0.valuefield.ID.ID kproperty.0.valueformat=int<br>column.0.link.lookup.link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querys<br>column.0.shortview=fallow.0.shortview=falseFalseFalse=false<br>column.false0.column=false{10.10 0<br>column.0.valuefield=hours<br>column.0.valueformat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup.view <br>column.1.link.valuefield=task：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task)。string(name)<br>column.1.namekey=task<br>column.1.querysort=task：name<br>column.1.stretch=0<br>column.1.valuefield=task<br>column.1 ueformat=HTML<br>列。1.width=150<br>列。2.description=父任务名称<br>列。2.link.linkproperty.0.name=ID<br>列。2.link.linkproperty.0.valuefield=task:parent:ID<br>列。2.link.linkproperty.0.valueformat=int<br>列。2.link.lookup=link.view<br>列。2.link.valuefield=task：objCode{43 {column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task：parent)。string(name)<br>column.2.name=Parent Task Name<br>column.2.querysort=task:parent:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=task:parent:name<br>column.2.valueformat=HTML<br>列.width=150<br><br><br><br></pre>

1. 单击&#x200B;**保存视图**。
