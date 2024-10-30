---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '分组：任务列表的项目发起人'
description: 此任务分组允许您按项目发起人分组任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# 分组：任务列表的项目发起人

此任务分组允许您按项目发起人分组任务。

![](assets/grouping--project-sponsor-for-a-task-350x189.png)

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
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
    <p>新增：</p>
   <ul><li><p>修改过滤器的参与者 </p></li>
   <li><p>用于修改报告的标准</p></li> </ul>

<p>当前：</p>
   <ul><li><p>请求修改筛选器 </p></li>
   <li><p>计划修改报告</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 按项目发起人分组任务列表


要应用此分组，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**分组**&#x200B;下拉菜单中，选择&#x200B;**新建分组**。

1. 单击&#x200B;**切换到文本模式**。
1. 移除所显示区域中的文本，然后使用以下代码替换该文本：

   `group.0.name=Project Sponsor<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=string`

1. 单击&#x200B;**完成**。
1. 更新分组名称，然后单击&#x200B;**保存分组**。

