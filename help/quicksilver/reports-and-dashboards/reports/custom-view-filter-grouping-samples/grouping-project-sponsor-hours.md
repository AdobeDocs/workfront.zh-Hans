---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：项目赞助人数小时
description: 此小时分组由记录小时数的项目赞助商组织小时数。 小时分组的标准报表生成器界面不提供到项目赞助商字段的映射。 必须使用文本模式界面访问此字段。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 分组：项目赞助人数小时

此小时分组由记录小时数的项目赞助商组织小时数。 小时分组的标准报表生成器界面不提供到项目赞助商字段的映射。 必须使用文本模式界面访问此字段。

![hour_report_grouped_by_ponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 按项目赞助商分组数小时

要应用此分组，请执行以下操作：

1. 去查查一下小时列表。
1. 从 **分组** 下拉菜单，选择 **新建分组**.

1. 单击&#x200B;**切换到文本模式**.
1. 删除 **对报表进行分组** 的上界。

1. 将文本替换为以下代码：

   <pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. 单击 **保存分组**.
