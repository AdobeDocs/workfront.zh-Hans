---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：展开的用户详细信息'
description: 此“用户”视图显示有关用户的信息。 除了他们的姓名、访问级别和公司之外，它还会显示他们的组、团队和工作角色的列表。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# 视图：展开的用户详细信息

<!--Audited: 11/2024-->

此“用户”视图显示有关用户的信息。 除了他们的姓名、访问级别和公司之外，它还会显示他们的组、团队和工作角色的列表。

![expanded_user_view.png](assets/expanded-user-view-350x75.png)

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
   <td> <p>新增：<ul><li>修改视图的参与者</li><li>用于修改报告的标准</li></ul></p><p>或</p>当前：<ul><li>请求修改视图</li><li>计划修改报告</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
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

## 查看展开的用户详细信息

要应用此视图，请执行以下操作：

1. 转到用户列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

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
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=accesslevel
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=accessLevel:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=accessLevel:objCode
   column.1.link.valueformat=val
   column.1.linkedname=accessLevel
   column.1.listsort=string(displayName)
   column.1.namekey=accesslevel
   column.1.querysort=name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=accessLevel:displayName
   column.1.valueformat=HTML
   column.1.viewalias=accessLevel:displayName
   column.1.width=100
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.value=val(objCode)
   column.2.listdelimiter=
   column.2.listmethod=nested(userGroups).lists
   column.2.namekey=group.plural
   column.2.stretch=50
   column.2.type=iterate
   column.2.valuefield=group:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.displayname=Teams
   column.3.listdelimiter=
   column.3.listmethod=nested(teams).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={name}
   column.3.valueformat=HTML
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.value=val(objCode)
   column.4.listdelimiter=
   column.4.listmethod=nested(userRoles).lists
   column.4.namekey=jobrole.plural
   column.4.stretch=50
   column.4.type=iterate
   column.4.valuefield=role:name
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=company
   column.5.link.linkproperty.0.name=ID
   column.5.link.linkproperty.0.valuefield=company:ID
   column.5.link.linkproperty.0.valueformat=int
   column.5.link.lookup=link.view
   column.5.link.valuefield=company:objCode
   column.5.link.valueformat=val
   column.5.linkedname=company
   column.5.listsort=nested(company).string(name)
   column.5.namekey=company
   column.5.querysort=company:name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=company:name
   column.5.valueformat=HTML
   column.5.width=150
   ```

1. 单击&#x200B;**完成** > **保存视图**。
