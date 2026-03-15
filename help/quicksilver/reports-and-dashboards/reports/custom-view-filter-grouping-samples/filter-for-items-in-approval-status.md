---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：仅显示处于审批状态的项目
description: 您只能显示当前处于待审批状态的特定状态的项目。 对于具有批准状态的任何其他对象，其作用相同。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 7%

---

# 筛选器：仅显示处于审批状态的项目

<!--Audited: 10/2024-->

您只能显示当前处于待审批状态的特定状态的项目。 对于具有批准状态的任何其他对象，其作用相同。

您可以将以下对象置于批准状态：

* 任务
* 问题
* 项目

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
   <p>投稿人或请求修改筛选器 </p>
   <p>标准或计划修改报告</p>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑报表、仪表板、日历的访问权限以修改报表</p> <p>编辑筛选器、视图、组的访问权限以修改筛选器</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 仅显示处于审批状态的项目

1. 转到项目列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。
1. 选择按&#x200B;**项目：状态**&#x200B;筛选，然后从列表中选择要按其筛选的状态。

   例如，在项目报表中，添加&#x200B;**Status Equal Planning**，以便只显示处于&#x200B;**Planning - Pending Approval**&#x200B;状态的项目。
1. 单击&#x200B;**文本模式**。
1. 通过将`status`添加到状态的3个字母的键来修改&#x200B;**:A**&#x200B;行：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 单击“**应用**”>“**另存为新文件**”。

   该列表仅显示状态为“计划 — 待审批”的项目。
