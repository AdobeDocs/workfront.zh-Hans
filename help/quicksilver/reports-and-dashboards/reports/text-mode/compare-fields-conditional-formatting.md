---
product-area: reporting
navigation-topic: text-mode-reporting
title: 比较条件格式中的字段
description: 您可以使用条件格式来比较视图中的2个不同字段，并在字段之间满足特定条件时突出显示它们。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# 比较条件格式中的字段

您可以使用条件格式来比较视图中的2个不同字段，并在字段之间满足特定条件时突出显示它们。

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
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限以编辑报表中的视图</p> <p>管理视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 示例：比较实际开始日期和计划开始日期

例如，如果任务的实际开始日期晚于计划开始日期，则可以使用条件格式突出显示“计划开始日期”列。

要使用条件格式比较任务的计划起始日期和实际起始日期，请执行以下操作：

1. 转到任务视图或报表。
1. （视情况而定）如果您正在处理报表，请从&#x200B;**列（视图）** 选项卡上，单击要有条件地设置格式的列标题以选择它。\
   例如，选择 **实际开始日期** 列。

1. 单击 **高级选项**，然后单击添加 **此列的规则**.

1. 使用在生成器中找到的现有值输入比较条件，并指定条件格式。\
   例如，我们要突出显示实际开始日期晚于（或大于）计划开始日期的任务。 选择“大于”修改量，然后在日期字段中选择实际日期。\
     ![](assets/cond-format-1-350x84.png)

1. （可选）选择 **应用于整行** 要将格式应用到整行。
1. 单击 **添加规则**，则 **完成**.

1. 选择 **实际开始日期** 列，然后单击 **切换到文本模式**.

1. **单击以编辑文本** 模式，然后添加以下文本行：

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   在本例中： 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >如果要比较Workfront本地字段，请使用驼峰式大小写语法来表示字段名称。 如果要比较自定义字段，请使用 **DE：字段的实际名称** 对于要与第一个字段比较的名称字段。\
   >例如，如果要将 **实际开始日期** 标有自定义字段 **提交日期**，在文本模式代码中添加以下语句：
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 确保 `righttext` 代码行与 `rightmethod` 代码行。

   ![](assets/cond-format-2-350x171.png)

1. 单击&#x200B;**保存**。
1. 单击 **保存并关闭**.

   列会突出显示符合您标准的字段。
