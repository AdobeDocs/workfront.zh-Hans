---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：使用自定义数据字段的外部URL'
description: 您可以使用任务视图中名为“自定义URL”的计算自定义字段来显示指向内部自定义URL的链接。
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 4247f2b437a5627ac4cba5289573eb4f1c18c583
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 视图：使用自定义数据字段的外部URL

<!--Audited: 11/2024-->

通过使用&#x200B;**任务视图**&#x200B;中名为“自定义URL”的&#x200B;**计算自定义字段**，您可以显示指向内部自定义URL的链接。

这有助于您直接从报表快速将某个视图中的某些对象链接到应用程序的某些区域。

创建计算自定义字段时，必须首先创建该字段，然后创建视图。

以下部分为任务的已计算自定义字段示例。 该自定义字段称为自定义URL。 自定义视图显示字段的值以及任务的&#x200B;**URL**&#x200B;字段。

使用相同的步骤，您可以为系统中所有具有自定义表单的对象创建相似的计算自定义字段和自定义视图。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p> 当前： 
   <ul>
   <li>请求修改视图</li> 
   <li>计划修改报告</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改视图的参与者</li> 
   <li>用于修改报告的标准</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建“自定义URL”计算自定义字段

有关创建计算自定义字段的信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

如果您有创建自定义表单的权限，则可以为名为“自定义URL”的任务创建计算自定义字段。 此字段直接链接到&#x200B;**任务详细信息**&#x200B;选项卡中的&#x200B;**概述**&#x200B;子选项卡。

1. 创建计算自定义字段。
1. 在计算字段中，输入以下代码：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;，&quot;/&quot;，&quot;task/&quot;，ID，&quot;/overview&quot;)

1. 将“`<domain>`”替换为您的实际域名，不带方括号。 此URL的`/overview`部分将链接指向任务左侧面板中的&#x200B;**概述**&#x200B;部分。

1. 创建&#x200B;**计算自定义字段**&#x200B;后，将带有此字段的&#x200B;**自定义表单**&#x200B;附加到Adobe Workfront中要在新视图中显示的多个任务。

## 创建显示任务的“自定义URL”和“URL”字段的视图

以下示例中的任务&#x200B;**视图**&#x200B;显示名为“自定义URL”的&#x200B;**计算自定义字段**&#x200B;作为直接链接，指向任务&#x200B;**详细信息**&#x200B;选项卡中的&#x200B;**概述**&#x200B;子选项卡以及任务的&#x200B;**URL**&#x200B;字段。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

要自定义此视图，请执行以下操作：

1. 转到任务列表。
1. 展开任务列表顶部的&#x200B;**视图**&#x200B;下拉列表。
1. 单击&#x200B;**自定义视图**。
1. 移除视图中的所有列（第一列除外）。
1. 单击第一列的标题。
1. 单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除&#x200B;**编辑文本模式**&#x200B;框中的文本并将其替换为以下代码：


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   在此示例中，“column.1.” 行将“自定义URL”字段中的值显示为任务&#x200B;**概述**&#x200B;部分的链接；“列。2”。 显示存储在任务的&#x200B;**URL字段**&#x200B;中的值。

1. 单击&#x200B;**完成** > **保存视图**。
