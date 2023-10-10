---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：合并来自一个共享列中多个列的信息'
description: 您可以合并显示在多个单独列中的信息，并将其显示在一个共享列中。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 0%

---

# 视图：合并来自一个共享列中多个列的信息

您可以合并显示在多个单独列中的信息，并将其显示在一个共享列中。

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
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 共享或合并列时的注意事项

* 可以合并两个相邻列并显示由换行符分隔的每列信息，也可以合并相邻两列的信息，而不用分隔符分隔每列的信息。
* 通过将本文中描述的相同语法应用于已共享列和相邻列，可以合并来自两个以上列的信息。
* 此 `valueformat=HTML` 行在共享列中是必需的。 否则，从Adobe Workfront导出报告时，列将不包含任何信息（它们将为空白）。
* 合并的列可能不支持条件格式。

  存在以下例外：

   * 在Workfront中查看信息时，如果构成合并列的列彼此的格式不同，则保留第一列的格式并忽略所有其他列的格式。
   * 将视图导出到PDF文件时，条件格式适用于合并列中的第一列。
   * 将视图导出到Excel文件时，合并的列显示为单独的列。 各个列还会显示各自的条件格式规则。

* 具有以下特征的列 **viewalias** 属性可以限制可以合并的列数。 要避免这些限制，请避免使用 **viewalias** 属性。 如果您必须包含 **viewalias** 属性，请确保它是列中列出的最后一个项目。

* 如果将具有共享列的列表导出为Excel或“制表符分隔”格式，则这些列在导出的文件中会被隔开。

* 当其中一列或两列都显示 `tile` 类型字段，则合并列中会自动引入强制换行符。 例如，带格式的文本字段包括 `tile` 键入字段。 在此例中，有一行代码 `type=tile` 在文本模式下查看列时。

## 合并两列的数据，不带换行符

您可以合并来自多个单独列的数据，以在一列中显示该数据，每列的值之间不出现断点或空格。

>[!TIP]
>
>如果合并的两列不能同时显示同一记录的值，则建议使用此方法。 例如，在工作项报告中，可以合并“问题名称”和“任务名称”列，而无需在它们之间插入换行符，因为工作项不能同时具有“问题名称”和“任务名称”。 工作项可以是Workfront中的问题或任务。

为此，请执行以下操作：

1. 使用视图的文本模式，将以下文本添加到要合并的第一列：

   `sharecol=true`

   合并列表或报表的前两列时，Workfront会位于第一列中包含对象信息的每行文本的前面，并包含 `column.0.` 以及包含有关第二列信息的文本行 `column.1.` .

   必须在第一列的列号前面加上该列的编号。 列计数始终以标记为的列表或报表最左侧的列开始 `column.0.`.

   如果共享多列，请确保在包含每列的共享信息的代码行中添加列号。

   **示例：** 下面是包含三个独立列的合并列的文本模式代码，从列表的第二列开始。 合并的值包括项目名称、计划开始日期和项目所有者姓名，并且三个值之间没有间隔：

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. 单击 **保存**，则 **保存视图**.

## 使用换行符合并两列的数据

执行以下操作可合并多列数据，以将其显示在一个公用列中，并在每列的值之间使用换行符：

1. 在要合并的两列之间添加第三列。

   >[!TIP]
   >
   >* 要合并的列必须彼此相邻。
   >* 必须单击要合并的第一列。

1. 单击 **切换到文本模式** 并在步骤1中添加的中间列中添加以下代码：

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. 单击第一列，然后单击 **切换到文本模式**，然后将以下文本添加到列：

   `sharecol=true`

   合并列表或报表的前两列时，Workfront会位于第一列中包含对象信息的每行文本的前面，并包含 `column.0.`，与共享信息的列 `column.1.`，以及包含有关第二列信息的文本行 `column.2.`.

   如果组合列位于视图的中间，则根据列在视图中的位置对其进行编号。 列计数始终以标记为的列表或报表最左侧的列开始 `column.0.`.

   如果共享多列，请确保在包含共享信息的代码行中添加列号。

   **示例：** 以下是共享列的文本模式代码，该列包含项目名称、计划开始日期和项目所有者名称及换行符。 共享列是项目视图的第二列。


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. 单击 **保存**，则 **保存视图**.
