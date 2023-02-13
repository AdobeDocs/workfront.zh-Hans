---
title: 授予对报表、功能板和日历的访问权限
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中报表、功能板和日历的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 授予对报表、功能板和日历的访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对报表、功能板和日历的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

此访问还包括对外部页面的访问。 有关外部页面的信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* 如果要授予用户对报表、功能板和日历的访问权限，则还必须授予这些用户对过滤器、视图和分组的访问权限。 有关说明，请参阅 [授予对过滤器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* 当某人与另一用户共享报表、功能板或日历时，收件人对报表、功能板或日历的权限由两项内容的组合决定：报表、功能板和日历的收件人访问级别设置 _和_ 共享者为报表、功能板或日历授予的任何权限
>
>有关用户在共享报表、功能板或日历时可以授予其权限的信息，请参阅 [共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定义访问级别配置用户对报表、功能板和日历的访问权限

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 或 **编辑** 按钮，然后选择要在 **优化设置**.

   ![reports_access.png](assets/reports-access.png)

   默认启用以下选项：

   * **创建**
   * **删除**
   * **查看内置报表**:需要选择此选项才能查看由Workfront构建的报表。
   * **共享**
   * **公开共享报表**:通过与没有Workfront帐户的任何人共享指向报表的公共链接，可以公开共享报表。 必须选择此选项才允许此级别的共享。
   * **在系统范围内共享**:可以与系统中拥有Workfront许可证的每个人共享报表。 必须选择此选项才允许此级别的共享。

      有关共享报表、功能板和日历的信息，请参阅 [共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

   创建访问级别后，您可以将其分配给用户。 有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按许可证类型访问报表、功能板和日历

有关每个访问级别中的用户可以处理问题的信息，请参阅部分 [报表](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 访问共享报表、功能板和日历

作为报表、功能板或日历的所有者或创建者，您可以通过授予其他用户对报表、功能板或日历的权限来与其共享，如 [共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

当您与其他用户共享任何对象时，收件人对该对象的权限取决于两件事的组合：

* 您为收件人授予的对象权限
* 对象类型的收件人访问级别设置
