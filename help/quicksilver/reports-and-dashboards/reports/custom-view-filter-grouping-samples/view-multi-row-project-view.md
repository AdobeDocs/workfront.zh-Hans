---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：多行项目视图
description: 在此项目视图中，您可以 — 编辑我。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# 查看：多行项目视图

在此项目视图中，您可以：

* 以多行格式显示项目信息。\
   视图使用

   ```
   sharecol=true
   ```

   标记来组合同一列标题下的多个字段。 要了解有关此标记的更多信息，请参阅 [查看：一个共享列中多个列的合并信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* 使用占位符列来保存HTML换行标记(

   ```
   <br>
   ```

   )强制将描述显示在项目名称的下方，例如。
* 在项目名称后面的括号中显示项目所有者。
* 将项目名称显示为指向项目的链接。

![](assets/project-multi-row-stacked-view-350x219.png)

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

## 构建多行项目视图

1. 创建新项目视图。 有关如何创建新视图的更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
1. 在生成视图时，请删除除一列之外的所有列。
1. 选择剩余的列并单击 **切换到文本模式**.
1. 复制并粘贴列下方的文本模式：
   <pre>column.0.linkedname=direct<br>column.0.link.valueformat=val<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.valuefield=objCode<br>column.0.link.lookup=link.view<br>column.0.sharecol=true<br>column.0.descriptionkey=name<br>column.0.width=150<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.name=项目名称/管理器/描述<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.textmode=true<br>column.0.listsort=string(name)<br>column.0.valueformat=HTML<br>column.1.valueexpression=CONCAT("",{owner}。{name},")")<br>column.1.listsort=nested(owner)。string(name)<br>column.1.width=1<br>column.1.linkedname=direct<br>column.1.querysort=owner:name<br>column.1.textmode=true<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valueformat=HTML<br>column.1.sharecol=true<br>column.2.width=1<br>column.2.value=<br><br>column.2.shortview=false<br>column.2.sharecol=true<br>column.2.stretch=0<br>column.2.textmode=true<br>column.2.valueformat=HTML<br>column.3.styledef.style=font-color:#ccc;<br>column.3.descriptionkey=description<br>column.3.linkedname=direct<br>column.3.valuefield=description<br>column.3.listsort=string(description)<br>column.3.querysort=description<br>column.3.namekey=description.abbr<br>column.3.textmode=true<br>column.3.sharecol=true<br>column.3.stretch=0<br>column.3.shortview=false<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.shortview=false<br>column.4.value=<br><br>column.4.sharecol=true<br>column.4.width=1<br>column.4.textmode=true<br>column.4.valueformat=HTML\<br>column.4.strect=0<br>column.5.name=计划日期/持续时间<br>column.5.width=150<br>column.5.querysort=planedStartDate<br>column.5.sharecol=true<br>column.5.stretch=0<br>column.5.textmode=true<br>column.5.shortview=false<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(planedStartDate)<br>column.5.valuefield=plannedStartDate<br>column.5.valueformat=atDate<br>column.6.sharecol=true<br>column.6.stretch=0<br>column.6.width=1<br>column.6.textmode=true<br>column.6.value=-<br>column.6.valueformat=HTML<br>column.6.shortview=false<br>column.7.namekey=plannedcompletedate.abbr<br>column.7.width=1<br>column.7.sharecol=true<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.listsort=atDateAsAtDate(planedCompletionDate)<br>column.7.linkedname=direct<br>column.7.descriptionkey=plannedcompletedate<br>column.7.textmode=true<br>column.7.querysort=planedCompletionDate<br>column.7.valueformat=atDate<br>column.7.valuefield=plannedCompletionDate<br>column.8.value=<br><br>column.8.width=1<br>column.8.textmode=true<br>column.8.sharecol=true<br>column.8.valueformat=HTML<br>column.8.stretch=0<br>column.9.textmode=true<br>column.9.listsort=intAsInt(durationMinutes)<br>column.9.strect=0<br>column.9.valuefield=durationFieldLong<br>column.9.descriptionkey=duration<br>column.9.viewalias=duration<br>column.9.querysort=durationMinutes<br>column.9.sharecol=true<br>column.9.width=100<br>column.9.shortview=false<br>column.9.namekey=duration.abbr<br>column.9.linkedname=direct<br>column.9.valueformat=compound<br>column.10.textmode=true<br>column.10.strect=0</pre>

1. 单击 **保存视图**.
