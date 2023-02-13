---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：用户职务角色占FTE可用性的百分比
description: 您可以在用户列表的视图中添加列，以显示用户关联的作业角色列表，以及每个作业角色的FTE可用性百分比（如用户配置文件中所定义）。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# 查看：用户职务角色占FTE可用性的百分比

您可以在用户列表的视图中添加列，以显示用户关联的作业角色列表，以及每个作业角色的FTE可用性百分比（如用户配置文件中所定义）。

有关定义用户FTE可用性百分比的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_avibility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## 查看FTE可用性的用户作业角色百分比

1. 转到用户列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** 区域，单击 **添加列**.

1. 单击新列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   <pre>displayname=角色时间百分比<br>listdelimiter=<p><br>listmethod=nested(userRoles)。lists<br>textmode=true<br>type=interate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. 单击 **保存**，则 **保存视图**.

1. （可选）指定视图的名称，然后单击 **保存视图**.
