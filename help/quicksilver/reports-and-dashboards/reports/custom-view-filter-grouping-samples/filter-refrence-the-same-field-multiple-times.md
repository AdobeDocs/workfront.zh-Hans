---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：创建引用同一字段（“AND”语句）的多个筛选器规则
description: 在标准模式界面中，如果尝试创建多个引用同一字段的筛选器（使用AND限定符），则在保存报表并退出Report Builder时，会删除其中一个筛选器。
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 过滤器：创建引用同一字段（“AND”语句）的多个过滤器规则

<!--Audited: 10/2024-->

在标准模式界面中，如果尝试创建多个引用同一字段的筛选器（使用AND限定符），则在保存报表并退出Report Builder时，会删除其中一个筛选器。

**示例：**&#x200B;您可能只想查看包含“绿色”一词但不包含“红色”一词的任务。 Adobe Workfront不允许您使用标准模式界面保存以下过滤器规则，因为它引用了相同的字段（任务名称），但使用了不同的修饰符并引用了不同的值：

* 任务名称>包含>绿色
* 任务名称>不包含>红色

但是，您可以使用文本模式创建此过滤器。

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

## 创建引用同一字段的多个筛选规则

1. 转到任务列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。
1. 单击&#x200B;**文本模式**。
1. 在显示的框中，添加以下代码：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >要构建类似的过滤器，请先构建第一条语句。 例如：
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >根据需要多次复制并粘贴语句。 然后，您可以添加所需数量的语句，以引用同一字段（在本例中为“name”），并对其他语句进行以下修改：
   >
   >1. 对于每个新字段可能值，在复制的两行前面加上“AND:1:”、“AND:2:”、“AND:3:”等。
   >1. 将字段行替换为新的字段值（在“=”符号之后）。
   >1. 将修改量行(_Mod)替换为新的修改量。
   >   
   >这些语句区分大小写。

1. 单击&#x200B;**应用**，然后单击&#x200B;**另存为新项**。
