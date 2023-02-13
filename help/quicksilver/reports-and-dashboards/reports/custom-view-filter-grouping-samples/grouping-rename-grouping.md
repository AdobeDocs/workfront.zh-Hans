---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：编辑分组中的显示名称”
description: 您可以将分组重命名为用户更熟悉的内容。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 分组：编辑分组中的显示名称

您可以将分组重命名为用户更熟悉的内容。

例如，将标准Portfolio名称分组应用于项目列表时，分组的名称将显示为 *Portfolio:名称：`<name of portfolio>`*.

![](assets/grouping-unedited-name-350x167.png)

您可以使用文本模式修改此分组，以显示更易读的名称。

![](assets/grouping-edited-name-350x160.png)

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

## 编辑分组中的显示名称

要更改项目分组中的显示名称，请执行以下操作：

1. 转到项目列表。
1. 从 **分组**&#x200B;下拉菜单，选择 **新建分组**.

1. 单击 **添加分组**，然后在 **首先由：** 字段，然后在其列表中显示时将其选中。

1. 单击 **切换到文本模式**.
1. 执行下列操作之一：

   * 将以下代码添加到 **对报表进行分组** 框：

      ```
      group.0.displayname=Your
      ```

      ```
      Value
      ```

      或者，在本例中：

      ```
      group.0.displayname=Portfolio
      ```

   * 删除分组文本模式界面中带有“name”字样的所有行，然后添加以下行：

      ```
      group.0.name=Your Value
      ```

      或者，在本例中：

      ```
      group.0.name=Portfolio
      ```

      您还可以将

      ```
      group.0.name
      ```

      行空白，在这种情况下，分组会显示要分组的值的名称。

      ![](assets/grouping-edited-name-no-name-350x162.png)

1. 单击 **完成**，则 **保存分组**.
