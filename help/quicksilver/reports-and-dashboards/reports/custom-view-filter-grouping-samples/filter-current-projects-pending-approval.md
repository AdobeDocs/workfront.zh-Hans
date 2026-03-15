---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 筛选器：显示您当前的待审批项目
description: The following project filter displays projects in the Current - Pending Approval status, where the logged-in user is either the Project Sponsor or the Portfolio Manager.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 8%

---

# 筛选器：显示您当前的待审批项目

<!--Audited: 10/2024-->

The following project filter displays projects in the Current - Pending Approval status, where the logged-in user is either the Project Sponsor or the Portfolio Manager.

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

## Filter current projects pending approval

要应用此过滤器，请执行以下操作：

1. 转到项目列表。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择&#x200B;**新建筛选器**。

1. 单击&#x200B;**文本模式**。
1. In the area displayed, copy and paste the following code:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. 单击&#x200B;**应用** > **另存为新项**。
