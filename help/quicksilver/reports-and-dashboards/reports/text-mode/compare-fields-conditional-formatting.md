---
product-area: reporting
navigation-topic: text-mode-reporting
title: 比较条件格式中的字段
description: 您可以使用条件格式来比较视图中的2个不同字段，并在这些字段之间满足特定条件时突出显示它们。
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# 比较条件格式中的字段

<!-- Audited: 1/2025 -->

您可以使用条件格式来比较视图中的2个不同字段，并在这些字段之间满足特定条件时突出显示它们。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板和日历的访问权限以编辑报告中的视图</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以编辑报告中的视图</p> <p>管理视图的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 示例：比较实际开始日期和计划开始日期

例如，如果任务的实际开始日期在计划开始日期之后，您可以使用条件格式突出显示“计划开始日期”列。

要使用条件格式比较任务的计划起始日期和实际起始日期，请执行以下操作：

1. 转到任务视图或报告。
1. （视情况而定）如果您正在处理报表，请在报表编辑器的&#x200B;**列（视图）**&#x200B;选项卡中，单击要有条件地设置格式的列的标题以将其选中。\
   例如，如果要通过比较“计划开始日期”和“实际开始日期”字段向其添加条件格式，请选择&#x200B;**实际开始日期**&#x200B;列。

1. 单击&#x200B;**高级选项**，然后单击“为此列添加&#x200B;**规则”**。

1. 使用在生成器中找到的现有值输入比较条件，并指定条件格式。\
   例如，我们要突出显示实际开始日期晚于（或大于）计划开始日期的任务。 选择“大于”修改量，然后在日期字段中选择实际日期。

   ![实际开始日期的条件格式](assets/cond-format-1-350x84.png)

1. （可选）如果要将格式应用到整行，请选择&#x200B;**应用到整行**。
1. 单击&#x200B;**保存**。

1. 选择&#x200B;**实际开始日期**&#x200B;列，然后单击&#x200B;**切换到文本模式**。

1. 单击&#x200B;**编辑文本模式**，然后添加以下文本行：

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

   ![条件格式](assets/cond-format-2-350x171.png)

1. 单击&#x200B;**保存**。
1. 单击&#x200B;**保存+关闭**。

   列突出显示符合条件的字段。
