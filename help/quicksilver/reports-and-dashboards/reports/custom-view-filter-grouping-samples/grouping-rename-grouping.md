---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 分组：编辑分组中的显示名称
description: 可将列表和报告中的分组重命名为用户更熟悉的类型。
author: Nolan
feature: Reports and Dashboards
exl-id: 072d3c2b-9ede-4bb9-9a27-dc77ceb732c4
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# 分组：编辑分组中的显示名称

<!--Audited: 01/2024-->

您可以将分组重命名为用户更熟悉的分组。

例如，将标准Portfolio名称分组应用于项目列表时，分组的名称将显示为&#x200B;*Portfolio：名称：`<name of portfolio>`*。

![按未编辑的名称分组](assets/grouping-unedited-name-350x167.png)

您可以使用文本模式修改此分组，以显示更易于阅读的名称。

![按编辑后的名称分组](assets/grouping-edited-name-350x160.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 编辑分组中的显示名称

要更改项目分组中的显示名称，请执行以下操作：

1. 转到项目列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**添加分组**，然后在&#x200B;**分组依据：**&#x200B;字段中开始输入“Portfolio名称”，然后当它显示在列表中时将其选定。

1. 单击&#x200B;**切换到文本模式**。
1. 执行以下操作之一：

   * 将以下代码添加到&#x200B;**为您的报告分组**&#x200B;框中可用的现有文本中：


     `group.0.displayname=Your Value`


     例如，添加以下代码将显示名称更改为“Portfolio”：

     `group.0.displayname=Portfolio`

   * 移除分组文本模式界面中包含“name”一词的所有行，然后添加该行：

     `group.0.name=Your Value`

     例如，添加以下代码将显示名称更改为“Portfolio”：

     `group.0.name=Portfolio`

     >[!TIP]
     >
     >您还可以将`group.0.name=`和`group.0.displayname=`行保留为空，在这种情况下，分组将显示您作为分组依据的值。


     ![按无名称的已编辑名称分组](assets/grouping-edited-name-no-name-350x162.png)

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存分组**。
1. （可选）更新分组名称，然后单击&#x200B;**保存分组**。

   根据您的文本模式信息修改分组的默认名称。
