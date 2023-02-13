---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 运行并提交具有其他用户访问权限的报表
description: 默认情况下，用户只能在报表中看到他们有权查看的对象。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 269340bc6a0c237edf44f5aa325d4ff95b647df8
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# 运行并提交具有其他用户访问权限的报表

默认情况下，用户只能在报表中看到他们有权查看的对象。

您可以允许所有用户在报表中看到与其他用户相同的结果，而不管他们对报表内对象的访问权限级别或权限级别如何。

如果您运行的报表具有其他具有较高访问权限的用户的访问权限(例如，Adobe Workfront管理员的访问权限)，则所有具有查看报表权限的用户都可以像在报表生成器中指定的用户一样查看报表中的信息。 您可以为用户在Workfront界面中找到的两个报表或作为电子邮件附件发送给用户的报表设置此设置。

>[!TIP]
>
>您应将 **使用以下访问权限运行此报表：** 字段中，仅当您希望显示具有该用户访问权限的报表时，才会显示活动用户。 例如，工作许可证用户可能无权查看由计划许可证用户或系统管理员构建的报表中的所有项目，除非该报表显示具有计划员或系统管理员的访问权限。\
如果与在 **使用以下访问权限运行此报表：** 字段，您可以将此字段留空。

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
   <td> <p>查看报表的权限（查看已提交的报表）</p> <p>管理报表的权限（用于运行报表）</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 显示具有其他用户访问权限的报表

填充 **运行具有以下访问权限的此报表：** 字段，可确保报表包含相同的数据，而不管哪个用户正在访问该报表。 报表会像为指定用户显示一样显示。

访问报表的用户必须至少拥有报表的“查看”权限，才能查看报表。 如果用户在 **运行具有以下访问权限的此报表：** 字段，则对于与之共享该报表的任何其他用户，将不再显示该报表。

要运行具有其他用户访问权限的报表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.

1. 选择要显示且具有其他用户访问权限的报表。
1. 单击 **报表操作**，然后单击 **编辑**.

1. 单击 **报表设置**.

1. 在 **使用以下访问权限运行此报表：** 字段，开始键入您希望报表显示为的用户名称，然后在列表中看到该用户名称时将其选中。\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   具有较低访问级别且允许生成报表的用户无法为 **运行具有以下访问权限的此报表：** 字段。

1. 单击 **完成**.
1. 单击 **保存并关闭**.\
   现在，在与共享了报表的所有用户中，都会显示该报表，就像该报表是由 **使用以下访问权限运行此报表：** 字段。

>[!IMPORTANT]
在 **使用以下访问权限运行此报表：** 如果报表包含引用登录用户的通配符的过滤器，则字段会影响报表中显示的信息。 报表将根据 **使用以下访问权限运行此报表：** 字段，而不是通配符筛选器中定义的内容。
有关用户字段的通配符的更多信息，请参阅 [通配符过滤器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 提交具有其他用户访问权限的报表

您可以设置要作为电子邮件的附件提交的报表。 您可以设置这些传送的报表，以在其显示时向访问级别较高的用户显示，以便所有用户都可以在传送的报表中看到相同的信息。 要查看电子邮件中投放的报表的用户必须添加到报表投放内收件人列表的“发送”中。 有关设置报表以进行提交的更多信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

要提交具有其他用户访问权限的报表，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.

1. 选择要使用其他用户的访问权限交付的报表。
1. 单击报表的名称以将其选中。
1. 单击 **报表操作**.
1. 单击 **发送报表**.

1. 在 **使用以下访问权限提交此报表：** 字段中，开始键入您希望报表在电子邮件中发送时显示的用户名称，然后在列表中看到该名称时选择该名称。 默认值是生成报表的用户的名称。\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   具有较低访问级别且允许生成报表的用户无法为 **提交此报表时具有以下访问权限：** 字段。

1. 选择 **格式** 您希望报表显示在电子邮件中：

   * HTML
   * PDF
   * MS Excel
   * MS Excel(.xlsx)
   * TSV

1. 单击 **立即发送** 立即发送。\
   或\
   单击 **进行重复投放** 计划报表的定期提交。\
   有关报告投放的更多信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).