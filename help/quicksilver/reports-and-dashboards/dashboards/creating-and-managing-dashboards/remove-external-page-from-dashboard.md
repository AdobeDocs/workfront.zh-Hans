---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 从功能板中删除外部页面
description: 如果不再需要某个外部页面，您可以从功能板中删除该页面。
author: Courtney
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 7%

---

# 从功能板中删除外部页面

<!-- Audited: 1/2025 -->

如果不再需要某个外部页面，您可以从功能板中删除该页面。

但是，在Adobe Workfront中创建外部页面后，您无法删除该页面。 您只能使用API删除外部页面。 有关Workfront API的信息，请参阅[API基础知识](../../../wf-api/general/api-basics.md)。 有关创建外部页面的信息，请参阅[在仪表板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

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
      <p>标准</p>
      <p>规划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理仪表板的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从功能板删除外部页面

1. 转到包含要删除的外部页面的仪表板。

1. 单击&#x200B;**仪表板操作**，然后单击&#x200B;**编辑**。

   ![编辑仪表板](assets/unshimmed-edit-dashboard.png)

1. 在屏幕右侧，找到要删除的外部页面，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

   ![删除仪表板中的外部页面图标](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 单击左下角的&#x200B;**保存+关闭**。

   这会从选定的功能板中删除外部页面。 外部页面保留在Workfront中，并可从报表访问。 有关信息，请参阅[在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)一文中的“在报表中查看外部页面”部分。
