---
title: 授予对报告、功能板和日历的访问权限
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中的报告、功能板和日历的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 授予对报告、功能板和日历的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对报告、功能板和日历的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

此访问权限还包括对外部页面的访问权限。 有关外部页面的信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

>[!NOTE]
>
>* 如果要授予用户访问报告、功能板和日历的权限，则还必须授予这些用户访问筛选器、视图和分组的权限。 有关说明，请参阅[授予对筛选器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)。
>* 当有人与其他用户共享报告、功能板或日历时，收件人在该报告上的权限由两件事的组合决定：收件人针对报告、功能板和日历的访问级别设置&#x200B;_以及_&#x200B;共享者授予该报告、功能板或日历的任何权限
>
>有关用户在共享报表、功能板或日历时可授予的权限的信息，请参阅[共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 使用自定义访问级别配置用户对报告、功能板和日历的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击报告右侧&#x200B;**查看**&#x200B;或&#x200B;**编辑**&#x200B;按钮上的齿轮图标![](assets/gear-icon-settings.png)，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![reports_access.png](assets/reports-access.png)

   默认启用以下选项：

   * **创建**
   * **删除**
   * **查看内置报告**：需要选择此项才能查看Workfront生成的报告。
   * **共享**
   * **公开共享报告**：通过与没有Workfront帐户的任何人共享指向报告的公共链接，可以公开共享报告。 必须选择此选项，才允许这种级别的共享。
   * **共享系统范围**：报告可与系统中拥有Workfront许可证的每个人共享。 必须选择此选项，才允许这种级别的共享。

     有关共享报告、仪表板和日历的信息，请参阅[共享报告、仪表板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 按许可证类型访问报告、功能板和日历

有关每个访问级别中的用户可以如何处理问题的信息，请参阅[适用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一文中的[报告](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports)部分。

## 访问共享的报告、功能板和日历

作为报告、功能板或日历的所有者或创建者，您可以通过授予其他用户对其的权限来共享它，如[共享报告、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)中所述。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置
