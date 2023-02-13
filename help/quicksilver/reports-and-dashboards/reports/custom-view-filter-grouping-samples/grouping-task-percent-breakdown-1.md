---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “分组：任务百分比划分1'
description: “在此自定义项目分组中，您可以显示按项目完成百分比值范围分组的项目。 划分显示完整百分比值，以25%为增量：0-25%、25-50%等。”
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: ddb9496c-9347-4dc9-a4ce-b9017abd0bb2
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 2%

---

# 分组：任务百分比划分1

在此自定义项目分组中，您可以显示按项目完成百分比值范围分组的项目。 划分显示完整百分比值，以25%为增量：0-25%、25-50%等。 

以下分组按完成百分比值将任务组织为6个不同的分组：

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![task_25__breakdown_grouping.png](assets/task-25--breakdown-grouping-350x412.png)

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

1. 单击&#x200B;**切换到文本模式**.
1. 删除 **对报表进行分组** 的上界。
1. 将文本替换为以下代码：

   <pre>group.0.linkedname=direct<br>group.0.name=百分比划分<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=26,"0-25 %",IF({percentComplete}&lt;=51,"25-50 %",IF({percentComplete}&lt;=76,"50-75 %",IF(percentComplete}&lt;100,"75-99%,"10")%)<br>group.0.valueformat=string</pre>

1. 单击 **保存分组**.
