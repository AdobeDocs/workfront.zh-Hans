---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：在任务视图中显示程序和Portfolio信息'
description: 此任务视图显示与任务项目关联的项目群和Portfolio。 在构建任务视图时，此信息在Report Builder中不可用。 此信息仅在文本模式下可用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 视图：在任务视图中显示程序和Portfolio信息

此任务视图显示与任务项目关联的项目群和Portfolio。 在构建任务视图时，此信息在Report Builder中不可用。 此信息仅在文本模式下可用。

该视图还提供指向任务列表中的项目、项目群和Portfolio的链接。

![](assets/view--program-and-portfolio-350x116.png)

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

## 在任务视图中显示程序和Portfolio信息

要将此视图应用于任务列表，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column(name){name){name.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.link.name.0.name=ID<br>column.link.link.0.valuefield.valuefield.0.valuefield.valuefield=project ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project)。string(name)<br>column.1.namekey=project<br>column.1.querysort=project<br>column.1.project：name{project：{name<br>column.1.column .shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=Program<br>column.2.linkproperty.0.name=ID<br>column.2.link.0.valuefield=project:program:ID<br>列2 LINK.LINKPROPERTY.0.VALUEFORMAT=INT<br>COLUMN.2.LINK.LOOKUP=LINK.VIEW<br>COLUMN.2.LINK.VALUEFIELD=PROJECT:program:OBJCoDE<br>COLUMN.2.LINKEDNAME=PROJECT<br>COLUMN.2.LISTSORT=NESTED(PROJECT：PROGRAM)。STRING(NAME)<br>COLUMN.2.NAMEKEY=PROJECT<br>COLUMN.2.QUERYSORT=PROJECT:program:NAME<br>COLUMN.2 VIEW=FALSE<br>COLUMN.2.STRETCH=0<br>COLUMN.2.VALUEFIELD=PROJECT:program:NAME<br>COLUMN.2.VALUEFORMAT=HTML<br>COLUMN.2.WIDTH=150<br>COLUMN.3.DESCRIPTIONKEY=PORTFOLIO<br>COLUMN.3.DISPLAYNAME=Portfolio<br>COLUMN.3.LINKPROPERTY.0.NAME=ID<br>column.3.link.0.valuefield=project:portfolio:ID<br>COLUMN 3.LINK.LINKPROPERTY.0.VALUEFORMAT=INT<br>COLUMN.3.LINK.LOOKUP=LINK.VIEW<br>COLUMN.3.LINK.VALUEFIELD=PROJECT:portfolio:OBJCoDE<br>COLUMN.3.LINK.VALUEFORMAT=VAL<br>COLUMN.3.LINKEDNAME=PROJECT<br>COLUMN.3.LISTSORT=NESTED(PROJECT：PORTFOLIO)。STRING(NAME)<br>COLUMN.3.NAMEKEY=PROJECT<br>COLUMN.3.QUERYSORT=PROJECT<br>NAME{PROJECT{PROJECT}NAME.3.QUERYSORT=PROJECT{PROJECT:portfolio:NAME{PROJECT3}.SHORTVIEW=FALSE<br>COLUMN.3.STRETCH=0<br>COLUMN.3.VALUEFIELD=PROJECT:portfolio:NAME<br>COLUMN.3.VALUEFORMAT=HTML<br>COLUMN.3.WIDTH=150 </pre>

1. 单击&#x200B;**保存视图**。
