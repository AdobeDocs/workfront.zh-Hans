---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：显示未包含在标准界面中的对象
description: 您可以在视图对象中显示未包含在标准模式界面中的对象。 您只能通过通过文本模式引用它们来执行此操作。 您可以通过以下任一方式确定视图中可以包含哪些字段 — 编辑我。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 视图：显示未包含在标准界面中的对象

您可以在视图对象中显示未包含在标准模式界面中的对象。 您只能通过通过文本模式引用它们来执行此操作。\
您可以通过以下任一方式确定视图中可以包含哪些字段：

* 使用 [API Explorer](https://one.workfront.com/s/api-explorer) 以发现可通过文本模式引用的其他对象。\
   API资源管理器中记录的所有字段并非都是文本模式的有效字段。 某些字段仅通过API进行报告。

* 在列中查找对象的ID字段。 大多数具有字段ID的对象还具有相应的列或字段名称，这些名称可能无法通过标准模式界面访问。

   您可以使用文本模式在视图中包含列或字段名称，而不是ID，方法是将 `fieldnameID` 和 `fieldname:name`.

   例如，在标准模式界面中， **Portfolio所有者ID** 字段，但 **Portfolio所有者名称** 字段的值。 您可以使用文本模式来显示 **Portfolio所有者名称** 的列中。

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

## 示例：将“Portfolio所有者名称”列添加到项目视图

1. 转到项目列表。
1. 从 **查看** 下拉菜单中，单击 **新建视图**.

1. 单击 **添加列** 然后，在 **在此列中显示** 字段，然后在其列表中显示时将其选中。

1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 替换 `valuefield` 行(`valuefield=portfolio:ownerID`)，并且包含以下行：

   ```
   valuefield=portfolio:owner:name
   ```

   或

   删除您在 **文本模式** ，并将其替换为以下代码：

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   在此特定示例中，报表将按Portfolio所有者ID对报表进行排序，如 `querysort` 行。

   >[!TIP]
   >
   >替换任何字段 `ID` 字段 `name` 使用文本模式时，始终替换 `ID` with `:name` 在 `valuefield` 行。

1. 单击 **保存**，则 **保存视图**.
