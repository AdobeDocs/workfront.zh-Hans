---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '视图：任务或项目报告中的可解析对象'
description: 您可以在项目、任务视图或报告中显示所有可解析对象的列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 视图：任务或项目报告中的可解析对象

您可以在项目、任务视图或报告中显示所有可解析对象的列表。

有关可解析对象的详细信息，请参阅文章[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

对于任务和项目，应用此视图的过程是相同的。

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

## 在任务或项目报告中查看可解析对象

1. 转到已从问题转换的任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域中，单击&#x200B;**添加列**。

1. 单击新列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre>displayname=Resolvables<br>listdelimiter=<br><br>listmethod=nested(resolvables)。lists<br>textmode=true<br>type=iterate<br>valuefield=name<br>valueformat=HTML<br></pre>

1. 单击&#x200B;**保存视图**。\
   新列中将显示所有可解析对象的列表。 列表中的对象名称不能直接链接到这些对象。
