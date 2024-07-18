---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：创建引用同一字段（'AND'语句）的多个过滤器规则”
description: 在标准模式界面中，如果尝试创建多个引用同一字段的筛选器（使用AND限定符），则在保存报表并退出Report Builder时，会删除其中一个筛选器。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 过滤器：创建引用同一字段（“AND”语句）的多个过滤器规则

在标准模式界面中，如果尝试创建多个引用同一字段的筛选器（使用AND限定符），则在保存报表并退出Report Builder时，会删除其中一个筛选器。

**示例：**&#x200B;您可能只想查看包含“绿色”一词但不包含“红色”一词的任务。 Adobe Workfront不允许您使用标准模式界面保存以下过滤器规则，因为它引用了相同的字段（任务名称），但使用了不同的修饰符并引用了不同的值：

* 任务名称>包含>绿色
* 任务名称>不包含>红色

但是，您可以使用文本模式创建此过滤器。

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
   <td> <p>请求修改筛选器 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建引用同一字段的多个筛选规则

1. 转到任务列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。
1. 单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 在报表的“设置过滤规则”区域中，添加以下代码：

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

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存筛选器**。
