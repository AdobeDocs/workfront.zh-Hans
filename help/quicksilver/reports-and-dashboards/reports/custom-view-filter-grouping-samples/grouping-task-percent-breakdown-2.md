---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：任务百分比划分2''
description: “在此自定义任务分组中，您可以显示按任务完成百分比值范围分组的任务。 划分显示10%点增量的完整百分比值：1-10%、11-20%等。”
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# 分组：任务百分比划分2

在此自定义任务分组中，您可以显示按任务完成百分比值范围分组的任务。 划分显示10%点增量的完整百分比值：1-10%、11-20%等。

以下分组按完成百分比值将项目组织到这些分组之一中：

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10__breakdown_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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

## 按任务百分比细分分组

要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从 **分组** 下拉菜单，选择 **新建分组**.

1. 单击 **切换到文本模式**.
1. 删除 **对报表进行分组** 的上界。
1. 将文本替换为以下代码：

   <pre>group.0.linkedname=direct<br>group.0.name=百分比划分<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %",IF({percentComplete}&lt;=31,"21-30 %",IF(percentComplete}&lt;41,"31-40 %",IF&lt;1-40%",IF&lt;1%,"50 %",IF({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71,"61-70 %",IF({percentComplete}&lt;81,"71-80 %",IF({percentComplete}&lt;91,"81-90 %",IF(percentComplete}&lt;100,"91-90%),"%10%))))))))<br>textmode=true</pre>

1. 单击 **保存分组**.
