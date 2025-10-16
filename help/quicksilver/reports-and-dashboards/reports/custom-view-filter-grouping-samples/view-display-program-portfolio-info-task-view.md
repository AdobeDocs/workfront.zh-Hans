---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：在任务视图中显示项目群和Portfolio信息
description: 此任务视图显示与任务项目关联的项目群和Portfolio。 在构建任务视图时，此信息在Report Builder中不可用。 此信息仅在文本模式下可用。
author: Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 视图：在任务视图中显示项目群和Portfolio信息

此任务视图显示与任务项目关联的项目群和Portfolio。 在构建任务视图时，此信息在Report Builder中不可用。 此信息仅在文本模式下可用。

该视图还提供了从任务列表指向项目、项目群和Portfolio的链接。

![查看项目和项目组合](assets/view--program-and-portfolio-350x116.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 在任务视图中显示项目群和Portfolio信息

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=project
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=project:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=project:objCode
   column.1.link.valueformat=val
   column.1.linkedname=project
   column.1.listsort=nested(project).string(name)
   column.1.namekey=project
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=program
   column.2.displayname=Program
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=project:program:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=project:program:objCode
   column.2.link.valueformat=val
   column.2.linkedname=project
   column.2.listsort=nested(project:program).string(name)
   column.2.namekey=project
   column.2.querysort=project:program:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=project:program:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=portfolio
   column.3.displayname=Portfolio
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=project:portfolio:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=project:portfolio:objCode
   column.3.link.valueformat=val
   column.3.linkedname=project
   column.3.listsort=nested(project:portfolio).string(name)
   column.3.namekey=project
   column.3.querysort=project:portfolio:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=project:portfolio:name
   column.3.valueformat=HTML
   column.3.width=150 
   ```

1. 单击&#x200B;**完成** > **保存视图**。
