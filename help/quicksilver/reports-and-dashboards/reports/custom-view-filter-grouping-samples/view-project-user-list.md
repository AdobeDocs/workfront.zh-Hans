---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：具有作业角色的项目用户列表
description: 您可以在项目列表或报表中应用此视图，以显示与项目关联的用户列表，以及他们在项目中执行的作业角色列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 查看：具有作业角色的项目用户列表

您可以在项目列表或报表中应用此视图，以显示与项目关联的用户列表，以及他们在项目中执行的作业角色列表。

此报表中的信息也可在项目的“人员”区域找到。

>[!TIP]
>
>如果用户没有列出作业角色，但您知道他们在其用户配置文件中与作业角色相关联，这可能意味着他们被分配到任务和问题，但他们可能没有与任务或问题上的作业角色相关联，或者报告中列出的用户不是任务和问题的受分配者，而是在项目中履行其他角色（例如，所有者或赞助者）。

![project_with_user_and_role_information_report_png](assets/project-with-user-and-role-information-report-350x100.png)

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

## 查看具有作业角色的项目用户列表

1. 转到项目列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Project用户<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.textmode=true<br>column.1.type=interate<br>column.1.valueexpression={user}。{name}<br>column.1.valueformat=HTML<br>column.2.displayname=项目角色<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles)。lists<br>column.2.textmode=true<br>column.2.type=interate<br>column.2.valueexpression={role}。{name}<br>column.2.valueformat=HTML</pre>

1. 单击 **保存视图**.
