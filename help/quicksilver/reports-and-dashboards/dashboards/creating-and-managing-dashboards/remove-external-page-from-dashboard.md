---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 从功能板中删除外部页面
description: 如果不再需要某个外部页面，您可以从功能板中删除该页面。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# 从功能板中删除外部页面

<!-- Audited: 1/2025 -->

如果不再需要某个外部页面，您可以从功能板中删除该页面。

但是，在Adobe Workfront中创建外部页面后，您无法删除该页面。 您只能使用API删除外部页面。 有关Workfront API的信息，请参阅[API基础知识](../../../wf-api/general/api-basics.md)。 有关创建外部页面的信息，请参阅[在仪表板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证</strong></td> 
   <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理仪表板的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从功能板删除外部页面

1. 转到包含要删除的外部页面的仪表板。

1. 单击&#x200B;**仪表板操作**，然后单击&#x200B;**编辑**。

   ![](assets/unshimmed-edit-dashboard.png)

1. 在屏幕右侧，找到要删除的外部页面，然后单击&#x200B;**删除**&#x200B;图标![](assets/delete.png)。

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 单击左下角的&#x200B;**保存+关闭**。

   这会从选定的功能板中删除外部页面。 外部页面保留在Workfront中，并可从报表访问。 有关信息，请参阅[在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)一文中的“在报表中查看外部页面”部分。
