---
title: 查看和导出审核日志
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以查看系统中的所有审核日志，或那些符合特定筛选条件的审核日志。 您还可以导出审核日志。 审核日志列出了过去90天内在系统中触发的用户更改。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# 查看和导出审核日志

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

您可以查看系统中的所有审核日志，或那些符合特定筛选条件的审核日志。 您还可以导出审核日志。

审核日志列出了过去90天内在系统中触发的用户更改。

有关所有审核日志类型及其生成原因的信息，请参阅 [审核日志](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>计划 </p> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 查看审核日志

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统>审核日志**.
1. 在 **日志类型** 下拉菜单中，选择要查看的审核日志类型。

   **所有日志类型** 默认情况下，处于选中状态。

   有关可以查看的所有审核日志类型及其包含的信息列表，请参阅 [审核日志](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. （可选）设置任何可用的过滤器。

   >[!NOTE]
   >
   >操作类型下拉菜单中的选项因所选的审核日志而异。

   ![](assets/audit-logs.jpg)

1. 单击 **应用**.
1. （可选）单击 **清除过滤器** 重置对过滤器所做的更改。

## 导出审核日志

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **系统>审核日志**.

1. 在 **日志类型** 下拉菜单中，选择审核日志。

   **所有日志类型** 默认情况下，处于选中状态。

1. 设置任何可用的过滤器，然后单击 **应用**.

   >[!IMPORTANT]
   >
   >一次无法导出的日志数超过50,000个。 Workfront会根据您设置的过滤器导出日志，而不是根据页面上显示的日志数量导出日志。 您可以在页面的右下角查看过滤的日志总数。

1. 单击 **导出**.
