---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：包含所有项目团队用户和角色的项目'
description: 此项目视图显示分配给项目团队的用户和工作角色的列表。
author: Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 查看：包含所有项目团队用户和角色的项目

<!--Audited: 11/2024-->

此项目视图显示分配给项目团队的用户和工作角色的列表。

>[!NOTE]
>
>如果工作角色与用户列在同一行，则这并不意味着用户在项目上填写该角色，也不意味着用户在他们的配置文件中分配了该角色。

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

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

## 查看包含所有项目团队用户和角色的项目

1. 转到项目列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请消除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：




   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.property.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column.0.name.name.abekey=name.abbr.abbr<br>column.abbr 0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.0.valuefield=userID<br>column.link.link.link.property .valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=iterate<br>column.1.valuefield=user：name<br>column.1.valueformat=HTML<br>column.1.wider.250&lbrace;20<br>column.2.description=团队角色<br>列。2.link.linkproperty.0.name=ID<br>列。2.link.linkproperty.0.valuefield=ID<br>列。2.link.linkproperty.0.valueformat=int<br>列。2.link.page=/roleView.cmd<br>列。2.listdelimiter=<br>列。2.listmethod=nested(roles)。lists<br>列。2.namekey=jobrole.plural<br>列。2.stretch=10{3 6}column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.stretch=0<br></pre>

1. 单击&#x200B;**完成** > **保存视图**。
