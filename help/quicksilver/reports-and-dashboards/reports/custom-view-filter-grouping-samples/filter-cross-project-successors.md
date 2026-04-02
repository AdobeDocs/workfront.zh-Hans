---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：显示不完整的跨项目后置任务
description: 此任务筛选器返回不完整的跨项目后置任务。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 11%

---

# 筛选器：显示不完整的跨项目后置任务

此任务筛选器返回不完整的跨项目后置任务。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
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

## 筛选跨项目后置任务

要应用此过滤器，请执行以下操作：

1. 转到任务列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. 单击&#x200B;**文本模式**。
1. 在显示的区域中，粘贴以下代码：
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>successorsMM：projectID=FIELD：projectID<br>successorsMM：projectID_Mod=ne</pre>

1. 单击&#x200B;**应用** > **另存为新项**。
