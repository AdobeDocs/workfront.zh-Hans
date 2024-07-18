---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：用户作业角色占 FTE 可用性的百分比”
description: 您可以向用户列表的视图添加一列，以显示与用户关联的工作角色的列表以及用户配置文件中定义的每个工作角色的 FTE 可用性百分比。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# 视图：用户工作角色占FTE可用性的百分比

您可以在用户列表视图中添加一列，以显示用户关联的工作角色的列表以及每个工作角色的FTE可用性百分比（如用户配置文件中所定义）。

有关定义用户FTE可用性百分比的信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

![user_with_percent_avialbility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报表</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请询问您的 Workfront 管理员是否在您的访问级别中设置了其他限制。 有关 Workfront 管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象 </a>的访问权限 。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的 Workfront 管理员。

## 查看用户 Job Role FTE 可用性的百分比

1. 转到用户列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域中，单击&#x200B;**添加列**。

1. 点按新列的标题，然后点按“ **切换到文本模式**”。
1. 将鼠标悬停在文本模式区域上，然后单击“**单击以编辑文本**”。
1. 删除在“**文本模式**”框中找到的文本，并将其替换为以下代码：
   <pre>displayname=角色时间百分比<br>listdelimiter=<p><br>listmethod=nested（userRoles）.lists<br>textmode=true<br>type=迭代<br>valueexpression=CONCAT（{role}，'-'，{timePercentage}，'%'）<br>valueformat=HTML</pre>

1. 单击“保存&#x200B;**”，然后单击**“**保存视图**”。

1. （可选）为视图指定一个名称，然后单击“ **保存视图**”。
