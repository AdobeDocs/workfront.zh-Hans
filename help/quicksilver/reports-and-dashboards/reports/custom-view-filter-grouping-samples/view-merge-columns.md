---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：合并来自一个共享列中多列的信息''
description: 您可以合并多个单独列中显示的信息，并将其显示在一个共享列中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# 查看：一个共享列中多个列的合并信息

您可以合并多个单独列中显示的信息，并将其显示在一个共享列中。

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

## 共享或合并列时的注意事项

* 可以合并两个相邻列，并显示每列中由换行符分隔的信息，也可以合并两个相邻列中的信息，在每列的信息之间没有分隔符。
* 您可以将来自两个以上列的信息合并，方法是将本文中描述的相同语法应用到已共享列和相邻列。
* 此

   ```
   valueformat=HTML
   ```

   行在共享列中是必填项。 否则，从Adobe Workfront导出报表时，这些列不包含任何信息（将为空）。
* 合并的列中可能不支持条件格式。

   存在以下例外：

   * 在Workfront中查看信息时，如果构成合并列的列之间的格式不同，则会保留第一列的格式，并忽略所有其他列的格式。
   * 将视图导出到PDF文件时，条件格式将应用于合并列中的第一列。
   * 将视图导出到Excel文件时，合并的列显示为单独的列。 单个列还显示其各自的条件格式规则。

* 列 **viewalias** 属性可以限制可合并的列数。 要避免这些限制，请避免使用 **viewalias** 属性。 如果必须包含 **viewalias** 属性，请确保它是列中列出的最后一个项目。

* 如果将包含共享列的列表导出为Excel或制表符分隔格式，则这些列在导出的文件中会分开。

## 合并来自两列的数据，不带换行符

您可以合并多个单独列中的数据，以将其显示在一列中，每列的值之间没有中断或空格。

>[!TIP]
>
>当合并两个永远无法同时显示同一记录值的列时，建议使用此方法。 例如，在工作项报表中，“问题名称”和“任务名称”列可以合并，而不会在它们之间产生换行符，因为工作项绝不能同时具有“问题名称”和“任务名称”。 工作项可以是“问题”或“Workfront中的任务”。

要执行此操作，请执行以下操作：

1. 使用视图的文本模式，将以下文本添加到要合并的第一列：

   ```
   sharecol=true
   ```

   当您合并列表或报表的前两列时，Workfront会先于包含第一列中对象信息的每行文本

   ```
   column.0.
   ```

   和包含第二列信息的文本行

   ```
   column.1.
   ```

   。\
   必须在第一列的列号前加该列的编号。 列计数始终以列表或报表最左侧的列开头，标记为

   ```
   column.0.
   ```

   。

   如果共享多列，请确保在包含每列共享信息的代码行中添加列号。

   **示例：** 以下是合并列的文本模式代码，该列包含三个单独的列，从列表的第二列开始。 合并的值包括项目名称、计划起始日期和项目所有者的名称，并且这三个值之间没有中断：

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.2.valuefield=plannedStartDate
   ```

   ```
   column.2.valueformat=atDate
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=owner:name
   ```

   ```
   column.3.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-no-line-breaks-350x142.png" style="width: 350;height: 142;"></pre>

1. 单击 **保存**，则 **保存视图**.

## 使用换行符合并来自两列的数据

执行以下操作以合并来自多列的数据，以将其显示在一个公共列中，并在每列的值之间添加换行符：

1. 在要合并的两列之间添加第三列。

   >[!TIP]
   * 要合并的列必须彼此相邻。
   * 必须单击要合并的第一列。


1. 单击 **切换到文本模式** 并在步骤1中添加的中间列中添加以下代码：

   ```
   value=<br>
   ```

   ```
   valueformat=HTML
   ```

   ```
   width=1
   ```

   ```
   sharecol=true
   ```

1. 将以下文本添加到第一列：

   ```
   sharecol=true
   ```

   当您合并列表或报表的前两列时，Workfront会先于包含第一列中对象信息的每行文本

   ```
   column.0.
   ```

   ，该列包含共享信息

   ```
   column.1.
   ```

   ，以及包含有关第二列信息的文本行(使用

   ```
   column.2.
   ```

   . 如果组合列在视图的中间，则会根据列在视图中的位置对列进行编号。 列计数始终以列表或报表最左侧的列开头，标记为

   ```
   column.0.
   ```

   。

   如果共享多列，请确保在包含共享信息的代码行中添加列号。

   **示例：** 下面是共享列的文本模式代码，该列包含“项目名称”、“计划起始日期”和带有换行符的项目所有者名称。 共享列是项目视图的第二列。

   ```
   column.1.displayname=Project_StartDate_Owner
   ```

   ```
   column.1.sharecol=true
   ```

   ```
   column.1.textmode=true
   ```

   ```
   column.1.valuefield=name
   ```

   ```
   column.1.valueformat=HTML
   ```

   ```
   column.2.value=<br>
   ```

   ```
   column.2.width=1
   ```

   ```
   column.2.valueformat=HTML
   ```

   ```
   column.2.sharecol=true
   ```

   ```
   column.3.valuefield=plannedStartDate
   ```

   ```
   column.3.valueformat=atDate
   ```

   ```
   column.3.sharecol=true
   ```

   ```
   column.4.value=<br>
   ```

   ```
   column.4.width=1
   ```

   ```
   column.4.valueformat=HTML
   ```

   ```
   column.4.sharecol=true
   ```

   ```
   column.5.textmode=true
   ```

   ```
   column.5.valuefield=owner:name
   ```

   ```
   column.5.valueformat=HTML
   ```

   <pre><img src="assets/shared-column-with-line-breaks-350x199.png" style="width: 350;height: 199;"></pre>

1. 单击 **保存**，则 **保存视图**.
