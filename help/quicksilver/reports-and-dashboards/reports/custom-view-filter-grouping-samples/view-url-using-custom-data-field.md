---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：使用自定义数据字段的外部URL'
description: 您可以使用任务视图中名为“自定义URL”的计算自定义字段来显示指向内部自定义URL的链接。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 视图：使用自定义数据字段的外部URL

通过使用&#x200B;**任务视图**&#x200B;中名为“自定义URL”的&#x200B;**计算自定义字段**，您可以显示指向内部自定义URL的链接。

这有助于您直接从报表快速将某个视图中的某些对象链接到应用程序的某些区域。

创建计算自定义字段时，必须首先创建该字段，然后创建视图。

以下部分为任务的已计算自定义字段示例。 该自定义字段称为自定义URL。 自定义视图显示字段的值以及任务的&#x200B;**URL**&#x200B;字段。

使用相同的步骤，您可以为系统中所有具有自定义表单的对象创建相似的计算自定义字段和自定义视图。

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

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 创建“自定义URL”计算自定义字段

有关创建计算自定义字段的信息，请参阅文章[将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)。

如果您有创建自定义表单的权限，则可以为名为“自定义URL”的任务创建计算自定义字段。 此字段直接链接到&#x200B;**任务详细信息**&#x200B;选项卡中的&#x200B;**概述**&#x200B;子选项卡。

1. 创建计算自定义字段。
1. 在计算字段中，输入以下代码：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;，&quot;/&quot;，&quot;task/&quot;，ID，&quot;/overview&quot;)

1. 将“`<domain>`”替换为您的实际域名，不带方括号。

   此

   ```
   /overview
   ```

   此URL的部分将链接指向任务左侧面板中的&#x200B;**概述**&#x200B;部分。

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
1. 单击界面右上角的&#x200B;**切换到文本模式**。
1. 单击&#x200B;**单击以编辑文本**。
1. 将下面的文本模式粘贴到一列中。\
   在此示例中，“column.1.” 将“自定义URL”字段中的值显示为任务&#x200B;**概述**&#x200B;的链接。 &#39;列。2.&#39; 显示存储在任务的&#x200B;**URL字段**&#x200B;中的值。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.link.linkedname=direct<br>column.0.listsort=string(name)<br>column.string(name){name){name.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link=customDataLabelsAsString(String) url)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString（自定义URL）<br>column.1.name=自定义URL<br>column.1.querysort=URL<br>column.1.short=false<br>column.1.valuefield=自定义URL<br>column.1.valueformat=customDataLabelsAsString<br> column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>列2.宽度=150<br><br><br></pre>

1. 单击&#x200B;**保存视图**。
