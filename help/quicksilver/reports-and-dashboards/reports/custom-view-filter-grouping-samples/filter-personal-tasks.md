---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：个人任务
description: 此任务过滤器返回发送给用户的临时工作请求，或者返回用户在其“主页”区域添加的待办事项。 个人任务未连接到项目，但如果需要，可将其移动到项目。
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# 筛选器：个人任务

<!--Audited: 10/2024-->

此任务过滤器返回发送给用户的临时工作请求，或者返回用户在“主页”区域的待办事项小部件中添加的待办事项。

临时工作请求和待办事项将作为个人任务保存在Adobe Workfront中。

个人任务未连接到项目，但如果需要，可将其移动到项目。 有关信息，请参阅[创建个人任务](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)。

![个人任务报告](assets/personal-tasks-report.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>修改过滤器的参与者或请求 </p>
   <p>用于修改报告的标准或计划</p>
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

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 筛选个人任务

要创建此过滤器，请执行以下操作：

1. 转到任务列表或任务报告。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，单击&#x200B;**新建筛选器**。
1. （视情况而定）单击&#x200B;**添加一个筛选器规则**，您正从报表访问筛选器；或者，如果您正从列表访问筛选器，请在第一个字段开始选择您的筛选器条件。
1. （视情况而定）选择以下筛选条件：

   * 从列表筛选器： **任务** > **个人** **Is True**
   * 从报表筛选器中： **任务** > **个人** > **相等（区分大小写）** > **真**。
1. 保存过滤器。

   该列表仅显示不在任何项目上的个人任务。
