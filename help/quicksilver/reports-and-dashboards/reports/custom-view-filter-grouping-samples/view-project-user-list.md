---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：具有工作角色的项目用户列表'
description: 您可以在项目列表或报告中应用此视图，以显示与项目相关联的用户列表，以及他们在项目上执行的工作角色列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 视图：具有工作角色的项目用户列表

您可以在项目列表或报告中应用此视图，以显示与项目相关联的用户列表，以及他们在项目上执行的工作角色列表。

此报告中的信息也可在项目的“人员”区域找到。

>[!TIP]
>
>如果未为用户列出工作角色，但您知道这些工作角色与其用户配置文件中的工作角色相关联，这可能意味着这些工作角色已分配给任务和问题，但它们可能未与任务或问题上的工作角色相关联，或者报告中列出的用户不是任务和问题的受分配者，但履行项目上的其他角色（例如，所有者或发起人）。

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## 查看具有工作角色的项目用户列表

1. 转到项目列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=2000<br>column.displayname=100000{100项目用户<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers)。lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}。{name}<br>列。1.valueformat=HTML<br>列。2.displayname=项目角色<br>列。2.listdelimiter=&lt;br&gt;<br>列。2.listmethod=nested(projectUserRoles)。lists<br>列。2.textmode=true<br>列。2.type=iterate<br>列。2.valueexpression={role}。{name}<br>column.2.valueformat=HTML</pre>

1. 单击&#x200B;**保存视图**。
