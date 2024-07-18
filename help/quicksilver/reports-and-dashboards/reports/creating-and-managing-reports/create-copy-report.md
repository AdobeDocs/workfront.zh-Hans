---
product-area: reporting;user-management
keywords: 保存，新建，报表，复制
navigation-topic: create-and-manage-reports
title: 创建报告副本
description: 您可以创建您有权访问的任何报表的副本。 您可以创建自定义报表的精确副本，也可以保存默认报表的新版本。 复制报告后，您成为所复制报告的所有者，该报告显示在“我的报告”部分中。
author: Nolan
feature: Reports and Dashboards
exl-id: 84737f48-efc5-45f1-acd1-b9f5d353f80f
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 创建报告副本

您可以创建您有权访问的任何报表的副本。 您可以创建自定义报表的精确副本，也可以保存默认报表的新版本。 复制报告后，您成为所复制报告的所有者，该报告显示在“我的报告”部分中。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 创建报告的精确副本

如果要制作您拥有的报告副本，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**报表**，然后单击&#x200B;**所有报表**。
1. 打开报表。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**复制**。

   >[!TIP]
   >
   >如果报告是默认报告，则复制选项不会出现在报告操作菜单中。\
   >有关如何创建默认报表副本的信息，请参阅[创建新版本报表](#create-a-new-version-of-a-report)。

   ![复制报告](assets/nwe-fulllistofreportactions-2022.png)

   创建原始报告副本时使用的默认名称为&#x200B;*原始报告的[名称]*&#x200B;副本。 例如，报告“第4季度已完成的任务”将使用“第4季度已完成的任务的副本”作为名称。

1. （可选）要重命名报表，请开始键入新名称。

   >[!TIP]
   >
   >如果在键入新名称之前取消选择标题，请选择报表标题，删除名称，然后输入新名称。

1. （可选）要与其他用户共享报告的新版本，请单击&#x200B;**报告操作**，然后单击&#x200B;**共享**。

   >[!NOTE]
   >
   >共享信息不会从原始版本传输到复制的报表。\
   >有关如何查看与谁共享了前一个报告的信息，请参阅[创建报告活动报告](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md#identify)。

1. （可选）如果您拥有原始报表的管理权限，并且不再需要原始报表，则可以将其删除，以在Workfront中删除不必要的重复报表。

   要删除原始报告，请执行以下操作：

   1. 导航到报表。
   1. 单击&#x200B;**报告操作**，然后单击&#x200B;**删除**。

   1. 单击&#x200B;**是，删除**&#x200B;以确认要删除该报表。

## 创建新版本的报表 {#create-a-new-version-of-a-report}

如果要创建默认报表的副本，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)。

1. 单击&#x200B;**报表**，然后单击&#x200B;**所有报表**。
1. 单击默认报表的名称以将其打开。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**编辑**。

   ![编辑报告](assets/nwe-reportactionsfordefaultreport-2022.png)

1. 在报告的以下选项卡中进行所需的任何修改：

   * **列（视图）**：有关自定义视图的更多信息，请参阅Adobe Workfront中的文章[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。
   * **分组**：有关自定义分组的详细信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)一文。
   * **筛选器**：有关自定义筛选器的详细信息，请参阅文章[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
   * **图表**：有关自定义报表图表的详细信息，请参阅文章[将图表添加到报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)。

1. 单击右上角的&#x200B;**报表设置**。
1. 在&#x200B;**报告标题**&#x200B;字段中，为报告提供一个新名称。
1. 单击&#x200B;**完成**。
1. 单击&#x200B;**另存为新报告**。

   ![](assets/nwe-save-as-new-report-350x220.png)

1. （可选）要与其他用户共享报告的新版本，请单击&#x200B;**报告操作**，然后单击&#x200B;**共享**。
