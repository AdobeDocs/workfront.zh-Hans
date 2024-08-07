---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：显示未包含在标准界面中的对象'
description: 可在视图中显示未包含在标准模式界面中的对象。 您只能通过文本模式引用它们。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 视图：显示未包含在标准界面中的对象

可在视图中显示未包含在标准模式界面中的对象。 您只能通过文本模式引用它们。\
您可以通过以下任一方式确定哪些字段可以包含在视图中：

* 使用[API资源管理器](../../../wf-api/general/api-explorer.md)发现可以通过文本模式引用的其他对象。\
  并非所有在API资源管理器中记录的字段对于文本模式都是有效字段。 某些字段只能通过API报告。

* 在列中查找对象的ID字段。 大多数具有字段ID的对象也具有相应的列或字段名称，可能无法通过标准模式界面访问。

  您可以使用文本模式将`fieldnameID`替换为`fieldname:name`，以在视图中包含列名或字段名而不是ID。

  例如，在标准模式界面中，**Portfolio所有者ID**&#x200B;字段可用于项目视图，但&#x200B;**Portfolio所有者名称**&#x200B;字段不可用。 您可以使用文本模式在视图的列中显示&#x200B;**Portfolio所有者名称**。

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

## 示例：将“Portfolio所有者名称”列添加到项目视图

1. 转到项目列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，单击&#x200B;**新建视图**。

1. 单击&#x200B;**添加列**，然后在&#x200B;**显示在此列**&#x200B;字段中开始键入“Portfolio所有者ID”，然后当它显示在列表中时将其选中。

1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 将`valuefield`行(`valuefield=portfolio:ownerID`)替换为以下行：

   ```
   valuefield=portfolio:owner:name
   ```

   或

   删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   在此特定示例中，报告将按Portfolio所有者ID对报告进行排序，如`querysort`行所示。

   >[!TIP]
   >
   >要使用文本模式将任何字段`ID`替换为字段`name`，请始终将`valuefield`行中的`ID`替换为`:name`。

1. 单击&#x200B;**保存**，然后单击&#x200B;**保存视图**。
