---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：按分组中所有对象共有的计算值组织列表结果
description: 您可能希望查看按完成百分比分组的任务，范围为0-25、26-50、51-75、75-99和100。 可以使用文本模式创建分组以执行此操作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# 分组：按分组中所有对象共有的计算值组织列表结果

您可能希望查看按完成百分比分组的任务，范围为0-25、26-50、51-75、75-99和100。 可以使用文本模式创建分组以执行此操作。

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

## 按分组中所有对象共有的计算值组织列表结果

要将此分组应用于任务列表，请执行以下操作：

1. 转到任务列表。
1. 从 **分组**&#x200B;下拉菜单，选择 **新建分组**.

1. 单击 **切换到文本模式**.
1. 在可用空间中，添加以下代码：

   ```
   textmode=true<br>group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({
   ```

   ```
   percentComplete
   ```

   ```
   }>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))<br>group.0.linkedname=direct<br>group.0.valueformat=doubleAsString<br>group.0.namekey=percentComplete
   ```

1. 单击 **完成**，则 **保存分组**.
