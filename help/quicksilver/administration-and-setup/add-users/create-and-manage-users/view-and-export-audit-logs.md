---
title: 查看和导出审核日志
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以查看系统中的所有审核日志，或符合特定筛选条件的审核日志。 您还可以导出审核日志。 审核日志列出过去90天内系统中触发的用户更改。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 6d02397a15b0b06c3c60fb5d71dfeb3cb0b0a30d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# 查看和导出审核日志

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

您可以查看系统中的所有审核日志，或符合特定筛选条件的审核日志。 您还可以将审核日志导出到CSV文件。

审核日志列出过去90天内系统中触发的用户更改。

有关所有审核日志类型以及生成这些类型的内容的信息，请参阅[审核日志概述](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>系统管理员</p></td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看审核日志

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统>审核日志**。
1. 在&#x200B;**操作类型**&#x200B;下拉列表中，选择要查看的审核类型。

   >[!NOTE]
   >
   >“Action Type（操作类型）”下拉菜单中的选项因所选的审核日志而异。

1. 在&#x200B;**日志类型**&#x200B;下拉菜单中，选择要查看的审核日志类型。

   默认情况下选择&#x200B;**所有日志类型**。

   有关可以查看的所有审核日志类型及其包含信息的列表，请参阅[审核日志概述](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md)。

1. （可选）为以下字段设置任何可用过滤器：

   * **用户**：键入进行更改的用户的名称。
   * **从**：进行更改的时间范围的开始日期。
   * **至**：进行更改时时间范围的结束日期。

   ![审核日志](assets/audit-logs.png)

1. 单击&#x200B;**应用**。
1. （可选）单击&#x200B;**清除**&#x200B;以重置对筛选器所做的更改。

## 导出审核日志

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**系统** > **审核日志**。

1. 在&#x200B;**日志类型**&#x200B;下拉菜单中，选择一个审核日志。

   默认情况下选择&#x200B;**所有日志类型**。

1. 设置任何可用的筛选器，然后单击&#x200B;**应用**。

   >[!IMPORTANT]
   >
   >您无法一次导出超过50,000个日志。 Workfront会根据您设置的过滤器导出日志，而不是根据页面上显示的日志数量。 您可以在页面的右下角查看已过滤日志的总数。

1. 单击&#x200B;**导出**。

   这将打开保存文件框，您可以将导出的文件保存在计算机上。

   只能以CSV格式保存审核日志。

   完成保存导出的文件。 您现在可以在计算机上找到该代码并与他人共享。
