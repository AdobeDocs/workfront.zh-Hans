---
title: 授予对问题的访问权限
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中问题的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 授予对问题的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对问题的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

有关使用自定义访问级别管理用户对Workfront中其他对象类型的访问的信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

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

## 使用自定义访问级别授予用户对问题的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击问题右侧&#x200B;**查看**&#x200B;或&#x200B;**编辑**&#x200B;按钮上的齿轮图标![](assets/gear-icon-settings.png)，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

1. （可选）要限制从更高层对象继承的问题权限，请单击&#x200B;**设置其他限制**，然后选择&#x200B;**从项目、任务、问题等中永不继承文档访问权限**。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 按许可证类型访问问题

有关每个访问级别中的用户可以如何处理问题的信息，请参阅[适用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一文中的[问题](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues)部分。

## 访问共享的问题

作为问题的所有者或创建者，您可以通过授予其他用户权限来与其共享，如[共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)中所述。

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置

此外，如果访问级别允许，用户可以通过对象层次结构获得对问题的访问权限：如果用户已经拥有问题的父级项目或任务的权限，则他们也将拥有该问题的权限（请参阅上面的步骤3）。 当您共享问题时，您可以看到继承了问题权限的用户列表。

![](assets/inherited-permissions.png)
