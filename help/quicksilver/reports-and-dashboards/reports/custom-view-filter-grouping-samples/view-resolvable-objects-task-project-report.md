---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：任务或项目报告中的可解析对象
description: 您可以在项目、任务视图或报表中显示所有可解析对象的列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# 查看：任务或项目报告中的可解析对象

您可以在项目、任务视图或报表中显示所有可解析对象的列表。

有关可解析对象的详细信息，请参阅文章 [解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolubles_in_report_png](assets/list-of-resolvables-in-report-350x54.png)

对于任务和项目，应用此视图的方式相同。

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

## 在任务或项目报告中查看可解析的对象

1. 转到已从问题转换的任务列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** 区域，单击 **添加列**.

1. 单击新列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   <pre>displayname=Resolubles<br>listdelimiter=<br><br>listmethod=nested(resoluveds)。lists<br>textmode=true<br>type=interate<br>valuefield=name<br>valueformat=HTML<br></pre>

1. 单击 **保存视图**.\
   新列中将显示所有可解析对象的列表。 列表中对象的名称不能直接链接到对象。
