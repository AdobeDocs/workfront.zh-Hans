---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：编辑分组中的显示名称'
description: 可将列表和报告中的分组重命名为用户更熟悉的类型。
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: 138181de2ad8257785773a5296bc5bcfc144a801
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# 分组：编辑分组中的显示名称

<!--Audited: 01/2024-->

您可以将分组重命名为用户更熟悉的分组。

例如，将标准Portfolio名称分组应用于项目列表时，分组的名称显示为&#x200B;*Portfolio：名称：`<name of portfolio>`*。

![](assets/grouping-unedited-name-350x167.png)

您可以使用文本模式修改此分组，以显示更易于阅读的名称。

![](assets/grouping-edited-name-350x160.png)

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
   <td>

<p>新增： </p>
   <ul>
   <li> <p>修改分组的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li></ul>

<p> 当前：</p>
   <ul>  
   <li><p>请求修改分组 </p></li>
   <li><p>计划修改报告</p></li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改分组</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 编辑分组中的显示名称

要更改项目分组中的显示名称，请执行以下操作：

1. 转到项目列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**添加分组**，然后在&#x200B;**首先由：**&#x200B;字段中开始输入“Portfolio名称”，然后当它显示在列表中时将其选定。

1. 单击&#x200B;**切换到文本模式**。
1. 执行以下操作之一：

   * 将以下代码添加到&#x200B;**为您的报告分组**&#x200B;框中可用的现有文本中：


     `group.0.displayname=Your Value`


     或者，在本例中：

     `group.0.displayname=Portfolio`

   * 移除分组文本模式界面中包含“name”一词的所有行，然后添加该行：

     `group.0.name=Your Value`

     或者，在本例中：

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >您还可以将`group.0.name=`和`group.0.displayname=`行保留为空，在这种情况下，分组将显示您作为分组依据的值。


     ![](assets/grouping-edited-name-no-name-350x162.png)

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存分组**。

   根据您的文本模式信息修改分组的默认名称。
