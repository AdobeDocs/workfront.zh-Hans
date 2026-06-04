---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：显示您当前的待审批项目
description: 以下项目筛选器显示处于当前 — 未决批准状态的项目，其中登录用户是项目发起人或Portfolio经理。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sPLW4-QHP5aXEd--UZVsS1WjY5-bJeyoOZ8mzYe7sww
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 8%

---

# 筛选器：显示您当前的待审批项目

<!--Audited: 10/2024-->

以下项目筛选器显示处于当前 — 未决批准状态的项目，其中登录用户是项目发起人或Portfolio经理。

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

## 筛选当前未决批准项目

要应用此过滤器，请执行以下操作：

1. 转到项目列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. 单击&#x200B;**文本模式**。
1. 在显示的区域中，复制并粘贴以下代码：
   <pre>状态=CUR：A<br>sponnerID=$$USER.ID<br>或:a:状态=CUR：A<br>或:a:项目组合：ownerID=$$USER.ID</pre>

1. 单击&#x200B;**应用** > **另存为新项**。
