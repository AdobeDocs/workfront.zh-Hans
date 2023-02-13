---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：项目，项目包含所有项目团队用户和角色
description: 此项目视图显示分配给项目团队的用户和作业角色列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 查看：包含所有项目团队用户和角色的项目

此项目视图显示分配给项目团队的用户和作业角色列表。

>[!NOTE]
>
>如果作业角色与用户列在同一行，则并不意味着用户正在项目中填写该角色，也不意味着用户在其配置文件中被分配了该角色。

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

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

## 查看包含所有项目团队用户和角色的项目

1. 转到项目列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：
   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=团队用户<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=interate<br>column.1.valuefield=user.name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=团队角色<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles)lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10<br>column.2.type=interate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.stretch=0</pre>

1. 单击 **保存视图**.
