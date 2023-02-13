---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “查看：任务和项目的原始问题详细信息
description: 将问题转换为任务或项目时，任务或项目与问题之间会建立解决对象关系。 此视图显示任务或项目完成时自动完成的问题的以下字段 — 编辑我。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# 查看：任务和项目的原始问题详细信息

将问题转换为任务或项目时，任务或项目与问题之间会建立解决对象关系。 此视图显示任务或项目完成时自动完成的问题的以下字段：

* 名称
* 输入日期
* 计划完成日期
* 实际完成日期
* 请求类型
* 创作者名称
* 分配给用户

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

有关更多信息，另请参阅 [查看：显示任务和项目列表上的原始问题信息](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## 查看任务和项目的原始问题详细信息

1. 转到任务列表或项目列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 在&#x200B;**列预览** ，则排除除一列之外的所有列。
1. 单击剩余列的标题，然后单击 **切换到文本模式**.
1. 将鼠标悬停在文本模式区域上，然后单击 **单击以编辑文本**.
1. 删除您在 **文本模式** ，并将其替换为以下代码：

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 单击 **保存视图**.
