---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：具有工作角色的项目用户列表'
description: 您可以在项目列表或报告中应用此视图，以显示与项目相关联的用户列表，以及他们在项目上执行的工作角色列表。
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 视图：具有工作角色的项目用户列表

<!--Audited: 11/2024-->

您可以在项目列表或报告中应用此视图，以显示与项目相关联的用户列表，以及他们在项目上执行的工作角色列表。

此报告中的信息也可在项目的“人员”区域找到。

>[!TIP]
>
>如果未为用户列出工作角色，但您知道这些工作角色与其用户配置文件中的工作角色相关联，这可能意味着这些工作角色已分配给任务和问题，但它们可能未与任务或问题上的工作角色相关联，或者报告中列出的用户不是任务和问题的受分配者，但履行项目上的其他角色（例如，所有者或发起人）。

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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


## 查看具有工作角色的项目用户列表

1. 转到项目列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。
1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请消除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. 单击&#x200B;**完成** > **保存视图**。
