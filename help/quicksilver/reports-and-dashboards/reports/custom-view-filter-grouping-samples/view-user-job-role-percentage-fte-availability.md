---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：用户职务角色占FTE可用性的百分比
description: 您可以在用户列表视图中添加一列，以显示与用户关联的职务角色的列表以及每个职务角色的FTE可用性百分比（如用户配置文件中所定义）。
author: Courtney
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 6%

---

# 视图：用户职务角色占FTE可用性的百分比

<!--Audited: 11/2024-->

您可以在用户列表视图中添加一列，以显示与用户关联的职务角色的列表以及每个职务角色的FTE可用性百分比（如用户配置文件中所定义）。

有关为用户定义FTE可用性的百分比的信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

![user_with_percent_availability_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>投稿人或修改视图的请求 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑对筛选器、视图、组的访问权限以修改视图</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


+++

## 查看用户职务角色的FTE可用性百分比

1. 转到用户列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域中，单击&#x200B;**添加列**。

1. 单击新列的标题，然后单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，并将其替换为以下代码：

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。

1. （可选）更新视图名称，然后单击&#x200B;**保存视图**。
