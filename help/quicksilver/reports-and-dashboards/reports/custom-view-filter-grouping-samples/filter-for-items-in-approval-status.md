---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：仅显示处于审批状态的项目
description: 您只能显示处于特定状态（当前处于“未决批准”中）的项目。 这同样适用于具有审批状态的任何其他对象。
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 筛选器：仅显示处于审批状态的项目

<!--Audited: 10/2024-->

您只能显示处于特定状态（当前处于“未决批准”中）的项目。 这同样适用于具有审批状态的任何其他对象。

您可以将以下对象置于批准状态：

* 任务
* 问题
* 项目

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

## 仅显示处于审批状态的项目

1. 转到项目列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。
1. 选择按&#x200B;**项目：状态**&#x200B;筛选，然后从列表中选择要按其筛选的状态。

   例如，在项目报表中，添加&#x200B;**Status Equal Planning**，以便只显示处于&#x200B;**Planning - Pending Approval**&#x200B;状态的项目。
1. 单击&#x200B;**文本模式**。
1. 通过将`status`添加到状态的3个字母键来修改&#x200B;**:A**&#x200B;行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 单击&#x200B;**应用** > **另存为新项**。

   该列表仅显示处于“计划 — 未决批准”状态的项目。
