---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 运行并交付具有其他用户访问权限的报告
description: 默认情况下，用户只能查看他们有权查看的报表中的对象。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 0%

---

# 运行并交付具有其他用户访问权限的报告

<!-- Audited: 11/2024 -->

默认情况下，用户只能查看他们有权查看的报表中的对象。

您可以允许所有用户以其他用户身份在报表中查看相同的结果，无论他们对报表中对象的访问级别或权限级别如何。

如果您使用具有更高访问权限的其他用户的访问权限(例如，Adobe Workfront管理员的访问权限)来运行报表，则所有有权查看报表的用户都可以以Report Builder中指定的用户的身份查看报表中的信息。 您可以为用户在Workfront界面中找到的报表设置此项，也可以为作为电子邮件附件发送给用户的报表设置此项。

>[!TIP]
>
>只有当您希望报表显示时显示该用户的访问权限，才应将&#x200B;**Run this report with Access Rights of：** field with an active user替换为active。 例如，工作许可证用户可能没有权限查看由计划许可证用户或系统管理员构建的报告中的所有项目，除非该报告显示时具有规划者或系统管理员的访问权限。\
>如果与具有与&#x200B;**在**&#x200B;字段的访问权限下运行此报告中指定的用户类似访问权限的用户共享报告，您可以将此字段留空。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
     <td> <p>查看权限报表可以查看传送的报表</p>
     <p>管理运行报告的报告权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 显示具有其他用户访问权限的报告

使用&#x200B;**的访问权限填充**&#x200B;运行此报告字段可确保报告包含相同的数据，无论哪个用户正在访问报告。 报表将按指定用户的显示方式显示。

访问报告的用户必须至少具有报告的查看权限，才能看到报告。 如果&#x200B;**运行此报告中列出的具有**&#x200B;访问权限的用户被停用，则报告不再显示给共享该报告的任何其他用户。

要运行具有其他用户访问权限的报告，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 报表]**。

1. 选择要显示的其他用户访问权限的报告。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**编辑**。

1. 单击&#x200B;**报表设置**。

1. 在&#x200B;**使用**&#x200B;的访问权限运行此报告字段中，开始键入您希望报告显示的用户名称，然后在列表中看到时将其选定。\
   ![运行访问权限为](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >具有允许生成报告的较低访问级别的用户无法为&#x200B;**运行具有**&#x200B;访问权限的此报告字段选择除自己之外的用户。

1. 单击&#x200B;**完成**。
1. 单击&#x200B;**保存+关闭**。\
   现在，与共享报告的所有用户均可看到该报告，就好像该报告已被&#x200B;**以**&#x200B;字段的访问权限运行此报告中指定的用户查看过。

>[!IMPORTANT]
>
>如果为&#x200B;**运行具有**&#x200B;访问权限的此报告字段输入非登录用户，并且该报告包含使用引用登录用户的通配符的筛选器，则会影响报告中显示的信息。 该报告将根据&#x200B;**使用**&#x200B;字段的访问权限运行此报告中指定的值显示，而不是根据通配符筛选器中定义的值显示。
>
>有关用户字段通配符的更多信息，请参阅[通配符筛选器变量概述](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)中的“基于用户的变量”部分。

## 提交具有其他用户访问权限的报告

您可以设置要作为电子邮件附件传送的报表。 您可以将这些已传送报表设置为在为具有较高访问级别的用户显示时显示，以便所有用户都可以在已传送报表中看到相同信息。 将看到电子邮件中传送的报告的用户必须添加到报告传送中的收件人列表中。 有关设置报表以进行传送的更多信息，请参阅文章[报表传送概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

要交付具有其他用户访问权限的报告，请执行以下操作：

1. 单击Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。

1. 选择要通过其他用户的访问权限提交的报告。
1. 单击报表名称将其选定。
1. 单击&#x200B;**报告操作**。
1. 单击&#x200B;**发送报告**。

1. 在&#x200B;**提交此报告（访问权限为：**）字段中，开始键入您希望报告在电子邮件中发送时显示的用户名称，然后在列表中看到报告时将其选定。 默认名称是正在构建报告的用户的名称。\
   ![已发送访问权限为](assets/unshimmed-send-report-access-rights-of.png)的报告

   >[!NOTE]
   >
   >具有允许生成报告的较低访问级别的用户无法为&#x200B;**提交具有**&#x200B;访问权限的此报告字段选择除自己之外的用户。

1. 选择您希望报告在电子邮件中显示的&#x200B;**格式**：

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. 单击&#x200B;**立即发送**&#x200B;立即发送。\
   或\
   单击&#x200B;**重复传送**&#x200B;以计划报告的重复传送。\
   有关报告交付的详细信息，请参阅文章[报告交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 带有Source列的报表的限制

以下报表显示Source列，您可以在其中查看有关父对象的信息：

* 问题报告
* 小时报告
* 文档报表

如果用户无权访问问题、小时或文档的父对象，则报告的Source列显示为空，即使报告配置为显示或使用其他用户的访问权限传递。

为了在报告中显示有关父对象的信息，我们建议为父对象添加一列，您可以在其中显示父对象的名称。

例如，您可以向包含Source列的报表中添加以下任意内容：

* “项目名称”、“任务名称”或“问题名称”列到文档或小时报告。
* 问题报告的“项目名称”或“任务名称”列。
* 使用文本模式表达式的列，该列引用所有三个对象。 以下是小时报告的示例：

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  有关文本模式视图的信息，请参阅[使用文本模式编辑视图](../text-mode/edit-text-mode-in-view.md)。
