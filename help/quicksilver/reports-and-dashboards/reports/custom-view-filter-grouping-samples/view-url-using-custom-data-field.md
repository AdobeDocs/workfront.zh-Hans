---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：使用自定义数据字段的外部URL'
description: 您可以在任务视图中使用名为“自定义URL”的计算自定义字段显示指向内部自定义URL的链接。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 查看：使用自定义数据字段的外部URL

您可以使用 **计算的自定义字段** 在 **任务视图**.

这有助于您从视图中的特定对象直接从报表快速链接到应用程序的某些区域。

创建计算的自定义字段时，必须先创建该字段，然后创建视图。

以下部分是任务的计算自定义字段示例。 自定义字段称为自定义URL。 自定义视图显示字段的值以及 **URL** 字段。

使用相同的步骤，您可以为系统中具有自定义表单的所有对象创建类似的计算自定义字段和自定义视图。

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

## 创建“Custom URL”计算的自定义字段

有关创建计算自定义字段的信息，请参阅文章 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

如果您有权创建自定义表单，则可以为名为“自定义URL”的任务创建一个计算的自定义字段。 此字段直接链接到 **概述** 子选项卡 **任务详细信息** 选项卡。

1. 创建计算的自定义字段。
1. 在“计算”字段中，输入以下代码：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID，&quot;/overview&quot;)

1. 替换“`<domain>`“ ”，不带括号。

   此

   ```
   /overview
   ```

   部分URL会将链接引导到 **概述** 中的。

1. 创建 **计算的自定义字段**，附加 **自定义表单** 将此字段添加到Adobe Workfront中要在新视图中显示的多个任务。

## 创建显示任务“自定义URL”和“URL”字段的视图

任务 **查看** 在以下示例中，显示 **计算的自定义字段** 称为“自定义URL”，作为指向 **概述** 任务中的子选项卡&#x200B;**详细信息** ，以及 **URL** 字段。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

要自定义此视图，请执行以下操作：

1. 转到任务列表。
1. 展开 **查看** 下拉列表。
1. 单击 **自定义视图**.
1. 除第一列外，删除视图内的所有列。
1. 单击第一列的标题。
1. 单击 **切换到文本模式** 的上角。
1. 单击 **单击以编辑文本**.
1. 将下面的文本模式粘贴到一列中。\
   在本例中为“column.1”。 将“自定义URL”字段中的值显示为指向任务的链接 **概述**. &#39;Column.2.&#39; 显示 **URL字段** 任务。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString（自定义URL）<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(Custom URL)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=Custom URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 单击 **保存视图**.
