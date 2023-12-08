---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 运行并交付具有其他用户访问权限的报告
description: 默认情况下，用户只能查看他们有权查看的报表中的对象。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# 运行并交付具有其他用户访问权限的报告

默认情况下，用户只能查看他们有权查看的报表中的对象。

您可以允许所有用户以其他用户身份在报表中查看相同的结果，无论他们对报表中对象的访问级别或权限级别如何。

如果您使用具有更高访问权限的其他用户的访问权限(例如，Adobe Workfront管理员的访问权限)来运行报表，则所有有权查看报表的用户都可以以Report Builder中指定的用户的身份查看报表中的信息。 您可以为用户在Workfront界面中找到的报表设置此项，也可以为作为电子邮件附件发送给用户的报表设置此项。

>[!TIP]
>
>您应将 **使用以下访问权限运行此报告：** 字段，其中包含活动的用户，但前提是您希望报表以该用户的访问权限显示。 例如，工作许可证用户可能没有权限查看由计划许可证用户或系统管理员构建的报告中的所有项目，除非该报告显示时具有规划者或系统管理员的访问权限。\
如果与具有类似权限的用户共享报告，则该用户在 **使用以下访问权限运行此报告：** 字段，可将此字段留空。

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表的权限（查看传送的报表）</p> <p>管理对报告的权限（运行报告）</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 显示具有其他用户访问权限的报告

填充 **使用以下访问权限运行此报告：** 字段可确保报表包含相同的数据，无论哪个用户正在访问报表。 报表将按指定用户的显示方式显示。

访问报告的用户必须至少具有报告的查看权限，才能看到报告。 如果用户列在 **使用以下访问权限运行此报告：** 字段已停用，则报告不再显示给共享该报告的任何其他用户。

要运行具有其他用户访问权限的报告，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **报表**.

1. 选择要显示的其他用户访问权限的报告。
1. 单击 **报表操作**，然后单击 **编辑**.

1. 单击 **报表设置**.

1. 在 **使用以下访问权限运行此报告：** 字段中，开始键入您希望报表显示的用户的名称，然后在列表中看到该名称时将其选定。\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   >
   对于允许构建报告的访问级别较低的用户，不能为其选择除自己之外的用户 **使用以下访问权限运行此报告：** 字段。

1. 单击 **完成**.
1. 单击 **保存+关闭**.\
   现在，与共享报告的所有用户均可看到该报告，就好像该报告已由中指定的用户查看一样。 **使用以下访问权限运行此报告：** 字段。

>[!IMPORTANT]
>
输入非登录用户的用户 **使用以下访问权限运行此报告：** 如果报表包含使用通配符引用登录用户的筛选器，则字段会影响报表中显示的信息。 报告会根据 **使用以下访问权限运行此报告：** 字段，而不是通配符筛选器中定义的内容。
>
有关用户字段通配符的更多信息，请参阅中的“基于用户的变量”部分 [通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 提交具有其他用户访问权限的报告

您可以设置要作为电子邮件附件传送的报表。 您可以将这些已传送报表设置为在为具有较高访问级别的用户显示时显示，以便所有用户都可以在已传送报表中看到相同信息。 将看到电子邮件中传送的报告的用户必须添加到报告传送中的收件人列表中。 有关设置报表以进行提交的更多信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

要交付具有其他用户访问权限的报告，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **报表**.

1. 选择要通过其他用户的访问权限提交的报告。
1. 单击报表名称将其选定。
1. 单击 **报表操作**.
1. 单击 **发送报告**.

1. 在 **提供这份报告的访问权限：** 字段中，开始键入您希望报表在电子邮件中传送时显示的用户名称，然后在列表中看到该报表时将其选定。 默认名称是正在构建报告的用户的名称。\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   >
   对于允许构建报告的访问级别较低的用户，不能为其选择除自己之外的用户 **提供这份报告的访问权限：** 字段。

1. 选择 **格式** 您希望报表显示在电子邮件中：

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. 单击 **立即发送** 立即发送。\
   或\
   单击 **重复传送** 计划报表的定期投放。\
   有关报告交付的更多信息，请参阅文章 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 具有源列的报表的限制

以下报表显示一个“源”列，您可以在其中查看有关父对象的信息：

* 问题报告
* 小时报告
* 文档报表

如果用户无权访问问题、小时或文档的父对象，则报告的“源”列显示为空，即使报告配置为显示或使用其他用户的访问权限传递。

为了在报告中显示有关父对象的信息，我们建议为父对象添加一列，您可以在其中显示父对象的名称。

例如，您可以将以下任意一项添加到具有“源”列的报表中：

* “项目名称”、“任务名称”或“问题名称”列到文档或小时报告。
* 问题报告的“项目名称”或“任务名称”列。
* 使用文本模式表达式的列，该列引用所有三个对象。 以下是小时报告的示例：

  `displayname=Custom Source`

  `linkedname=opTask`

  `namekey=view.relatedcolumn`

  `namekeyargkey.0=opTask`

  `namekeyargkey.1=name`

  `textmode=true`

  `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

  `valueformat=HTML`

  有关文本模式视图的信息，请参见 [使用文本模式编辑视图](../text-mode/edit-text-mode-in-view.md).