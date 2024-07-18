---
product-area: reporting
navigation-topic: text-mode-reporting
title: 比较条件格式中的字段
description: 您可以使用条件格式来比较视图中的2个不同字段，并在这些字段之间满足特定条件时突出显示它们。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 比较条件格式中的字段

您可以使用条件格式来比较视图中的2个不同字段，并在这些字段之间满足特定条件时突出显示它们。

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以编辑报告中的视图</p> <p>管理视图的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 示例：比较实际开始日期和计划开始日期

例如，如果任务的实际开始日期在计划开始日期之后，您可以使用条件格式突出显示“计划开始日期”列。

要使用条件格式比较任务的计划起始日期和实际起始日期，请执行以下操作：

1. 转到任务视图或报告。
1. （视情况而定）如果您正在处理报表，请在&#x200B;**列（视图）**&#x200B;选项卡中，单击要有条件地设置格式的列的标题以将其选中。\
   例如，如果要通过比较“计划开始日期”和“实际开始日期”字段向其添加条件格式，请选择&#x200B;**实际开始日期**&#x200B;列。

1. 单击&#x200B;**高级选项**，然后单击“为此列添加&#x200B;**规则”**。

1. 使用在生成器中找到的现有值输入比较条件，并指定条件格式。\
   例如，我们要突出显示实际开始日期晚于（或大于）计划开始日期的任务。 选择“大于”修改量，然后在日期字段中选择实际日期。\
     ![](assets/cond-format-1-350x84.png)

1. （可选）如果要将格式应用到整行，请选择&#x200B;**应用到整行**。
1. 单击&#x200B;**添加规则**，然后单击&#x200B;**完成**。

1. 选择&#x200B;**实际开始日期**&#x200B;列，然后单击&#x200B;**切换到文本模式**。

1. **单击以编辑文本**&#x200B;模式，然后添加以下文本行：

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   在我们的示例中： 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >如果要比较Workfront本地字段，请使用驼峰式大小写语法来表示该字段的名称。 如果要比较自定义字段，请将&#x200B;**DE：实际字段名称**&#x200B;用于要与第一个字段进行比较的名称字段。\
   >例如，如果要将&#x200B;**实际开始日期**&#x200B;与标记为&#x200B;**交付日期**&#x200B;的自定义字段进行比较，请在文本模式代码中添加以下语句：
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. 确保`righttext`行代码与`rightmethod`行代码中的语句匹配。

   ![](assets/cond-format-2-350x171.png)

1. 单击&#x200B;**保存**。
1. 单击&#x200B;**保存+关闭**。

   列突出显示符合条件的字段。
