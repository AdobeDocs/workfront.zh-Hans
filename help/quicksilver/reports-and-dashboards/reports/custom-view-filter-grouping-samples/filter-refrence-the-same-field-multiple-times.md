---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：创建引用相同字段（“AND”语句）的多个筛选规则”
description: 在标准模式界面中，当尝试创建多个引用相同字段的过滤器（使用AND限定符）时，当您保存报表并退出报表生成器时，其中一个过滤器会被删除。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 过滤器：创建引用相同字段（“AND”语句）的多个筛选规则

在标准模式界面中，当尝试创建多个引用相同字段的过滤器（使用AND限定符）时，当您保存报表并退出报表生成器时，其中一个过滤器会被删除。

**示例：** 您可能只想查看包含“green”一词但名称中不包含“red”一词的任务。 Adobe Workfront不允许您使用标准模式界面保存以下过滤器规则，因为它引用了相同的字段（任务名称），但使用了不同的修饰符，并引用了不同的值：

* 任务名称>包含>绿色
* 任务名称>不包含>红色

但是，您可以使用文本模式创建此过滤器。

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

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建引用同一字段的多个过滤器规则

1. 转到任务列表。
1. 从 **过滤器** 下拉菜单，选择 **新建过滤器**.
1. 单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 在“为报表设置过滤器规则”区域，添加以下代码：

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >要构建类似的过滤器，请先构建第一个语句。 例如：
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >根据需要多次复制并粘贴该语句。 然后，您可以添加所需数量的语句以引用同一字段（在我们的示例中为“name”），并对附加语句进行以下修改：
   >
   >1. 在两个复制的行之前添加“AND”:1:&quot;, &quot;和:2:&quot;, &quot;和:3:“ ”等。
   >1. 将字段行替换为新字段值（在“=”符号之后）。
   >1. 将修饰符行(_Mod)替换为新修饰符。

   >   
   >这些语句区分大小写。

1. 单击 **完成**，则 **保存过滤器**.
