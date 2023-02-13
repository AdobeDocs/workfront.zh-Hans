---
product-area: reporting;user-management
keywords: 保存，新建，报表，复制
navigation-topic: create-and-manage-reports
title: 创建报表副本
description: 您可以创建您有权访问的任何报表的副本。 您可以创建自定义报表的确切副本，也可以保存默认报表的新版本。 复制报表后，您将成为复制报表的所有者，并会显示在我的报表部分。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 创建报表副本

您可以创建您有权访问的任何报表的副本。 您可以创建自定义报表的确切副本，也可以保存默认报表的新版本。 复制报表后，您将成为复制报表的所有者，并会显示在我的报表部分。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建报表的确切副本

如果要复制您所有者的报表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **报表**，则&#x200B;**所有报表**.
1. 打开报表。
1. 单击 **报表操作**，则 **复制**.

   >[!TIP]
   >
   >如果报表是默认报表，则“报表操作”菜单中不会显示“复制”选项。\
   >有关如何创建默认报表副本的信息，请参阅 [创建报表的新版本](#create-a-new-version-of-a-report).

   ![复制报表](assets/nwe-fulllistofreportactions-2022.png)

   将创建原始报表的副本，其默认名称为 *副本 [原始报表的名称]*. 例如，报表“Q4 Completed Tasks”将以“Q4 Completed Tasks的副本”作为名称。

1. （可选）要重命名报表，请开始键入新名称。

   >[!TIP]
   >
   >如果在键入新名称前取消选择标题，请选择报表标题，删除名称，然后输入新名称。

1. （可选）要与其他用户共享新版本的报表，请单击 **报表操作**，则 **共享**.

   >[!NOTE]
   >
   >共享信息不会从原始版本传输到复制的报表。\
   >有关如何查看与谁共享了上一个报表的信息，请参阅 [创建报告活动报告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify).

1. （可选）如果您拥有原始报表的“管理”权限，并且不再需要原始报表，则可以删除该权限，以在Workfront中删除不必要的重复报表。

   要删除原始报表，请执行以下操作：

   1. 导航到报表。
   1. 单击 **报表操作**，则 **删除**.

   1. 单击 **是，删除它** 以确认要删除报表。

## 创建报表的新版本 {#create-a-new-version-of-a-report}

如果要创建默认报表的副本，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **报表**，则&#x200B;**所有报表**.
1. 单击默认报表的名称以将其打开。
1. 单击 **报表操作**，则 **编辑**.

   ![编辑报表](assets/nwe-reportactionsfordefaultreport-2022.png)

1. 在报表的以下选项卡中进行任何需要的修改：

   * **列（视图）**:有关自定义视图的更多信息，请参阅文章 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).
   * **分组**:有关自定义分组的更多信息，请参阅文章 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
   * **过滤器**:有关自定义过滤器的更多信息，请参阅文章 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
   * **图表**:有关自定义报表图表的更多信息，请参阅文章 [将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. 在右上角，单击 **报表设置**.
1. 在 **报表标题** 字段中，为报表提供一个新名称。
1. 单击 **完成**.
1. 单击 **另存为新报表**.

   ![](assets/nwe-save-as-new-report-350x220.png)

1. （可选）要与其他用户共享新版本的报表，请单击 **报表操作**，则 **共享**.
