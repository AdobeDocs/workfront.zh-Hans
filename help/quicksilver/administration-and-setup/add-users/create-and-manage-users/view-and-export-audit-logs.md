---
title: 查看和导出审核日志
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以查看系统中的所有审核日志，或符合特定筛选条件的审核日志。 您还可以导出审核日志。 审核日志列出过去90天内系统中触发的用户更改。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 20cb940de1d42057ed11e4e7d59f1875cdba38bb
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 查看和导出审核日志

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

您可以查看系统中的所有审核日志，或符合特定筛选条件的审核日志。 您还可以导出审核日志。

审核日志列出过去90天内系统中触发的用户更改。

有关所有审核日志类型以及生成这些类型的原因的信息，请参阅[审核日志](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>计划 </p> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 查看审核日志

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统>审核日志**。
1. 在&#x200B;**日志类型**&#x200B;下拉菜单中，选择要查看的审核日志类型。

   默认情况下选择&#x200B;**所有日志类型**。

   有关可以查看的所有审核日志类型及其包含信息的列表，请参阅[审核日志](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

1. （可选）设置任何可用的过滤器。

   >[!NOTE]
   >
   >“Action Type（操作类型）”下拉菜单中的选项因所选的审核日志而异。

   ![](assets/audit-logs.jpg)

1. 单击&#x200B;**应用**。
1. （可选）单击&#x200B;**清除筛选器**&#x200B;以重置对筛选器所做的更改。

## 导出审核日志

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统>审核日志**。

1. 在&#x200B;**日志类型**&#x200B;下拉菜单中，选择一个审核日志。

   默认情况下选择&#x200B;**所有日志类型**。

1. 设置任何可用的筛选器，然后单击&#x200B;**应用**。

   >[!IMPORTANT]
   >
   >您无法一次导出超过50,000个日志。 Workfront会根据您设置的过滤器导出日志，而不是根据页面上显示的日志数量。 您可以在页面的右下角查看已过滤日志的总数。

1. 单击&#x200B;**导出**。
