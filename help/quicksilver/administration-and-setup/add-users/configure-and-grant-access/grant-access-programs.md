---
title: 授予对程序的访问权限
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中程序的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 169f6357-1fbb-43e0-83af-1c4be682ddbf
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# 授予对程序的访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对程序的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

有关使用自定义访问级别管理用户对Workfront中其他对象类型的访问权限的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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

## 使用自定义访问级别配置用户对程序的访问权限

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 或 **编辑** 按钮，然后选择要在下授予的功能 **优化设置**.

   有关每个访问级别的用户可以对程序执行的操作的信息，请参阅部分 [程序](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

   >[!NOTE]
   >
   >在为特定类型的对象配置访问级别设置时，该配置不会影响用户对级别较低的对象的访问。 例如，您可以限制用户删除其访问级别中的程序，但这并不限制用户删除排名低于程序的项目。有关对象层次结构的详细信息，请参阅部分 [对象的相互依赖和层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

   创建访问级别后，您可以将其分配给用户。 有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按许可证类型访问程序

有关每个访问级别的用户可以对程序执行的操作的信息，请参阅部分 [程序](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#programs) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 访问共享程序

作为程序的所有者或创建者，您可以通过授予其他用户对该程序的权限来与其共享，如 [共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md).

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
