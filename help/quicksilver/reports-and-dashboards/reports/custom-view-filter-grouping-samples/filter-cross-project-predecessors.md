---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '筛选器：显示不完整的跨项目前置任务'
description: 此任务筛选器返回不完整的跨项目前置任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# 筛选器：显示不完整的跨项目前置任务

<!--Audited: 10/2024-->

此任务筛选器返回不完整的跨项目前置任务。

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

## 筛选跨项目前置任务

要应用此过滤器，请执行以下操作：

1. 转到任务列表或任务报告。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. （视情况而定）如果您从列表访问筛选器，请单击&#x200B;**文本模式**；如果您从报表访问筛选器，请单击&#x200B;**切换到文本模式**。
1. 在新区域中，粘贴以下代码：
   <pre>前置任务MM：projectID=FIELD：projectID<br>前置任务MM：projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. （视情况而定）如果您从报表访问筛选器，请单击&#x200B;**保存筛选器**；如果您从任务列表访问筛选器，请单击&#x200B;**应用**，然后单击&#x200B;**另存为新筛选器**。
