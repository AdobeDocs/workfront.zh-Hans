---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: 使用Workfront Goals的要求
description: 在访问Adobe Workfront目标之前，您的Adobe Workfront管理员必须确保满足某些条件。 在本篇文章中，了解访问Workfront目标的访问权限、权限和布局要求。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 使用Workfront Goals的要求

<!--Audited P&P only: 04/2025-->

在访问Adobe Workfront目标之前，您的Adobe Workfront管理员必须确保满足所有以下条件：

* 您的组织以前购买过Adobe Workfront Goals包。 Adobe Workfront目标不再可供购买。

  有关更多信息，请参阅本文中的[获取Workfront目标组织访问权限](#obtain-workfront-goals-organization-access)部分。

* 为您分配正确类型的Workfront许可证。 有关分配许可证类型和访问级别的信息，请参阅本文中的[更新许可证类型和访问级别设置](#update-license-types-and-access-level-settings)部分。

  >[!NOTE]
  >
  >具有外部许可证类型的用户无法访问Workfront目标。

* 授予您访问访问级别中目标的权限。 有关信息，请参阅[授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

  >[!NOTE]
  >
  >默认情况下，用户无法访问其访问级别中的目标。


* 为您分配包含主菜单中的目标区域的布局模板。

  >[!NOTE]
  >
  >必须为包括系统管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。

  有关信息，请参阅本文中的[将Workfront目标添加到布局模板](#add-workfront-goals-to-a-layout-template)部分。

* 如果必须修改未自行创建的目标，则目标创建者必须与您共享目标并授予您管理权限。

  有关信息，请参阅本文中的[与其他用户共享各个目标](#share-individual-goals-with-other-users)部分。

## 获取Workfront目标组织访问权限 {#obtain-workfront-goals-organization-access}

最后一个包含Workfront目标的Adobe Workfront包是Adobe Workfront Ultimate。
Workfront目标不再可用于购买较新的包。
与您的客户代表联系以查询Workfront目标。

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## 更新许可证类型和访问级别设置  {#update-license-types-and-access-level-settings}

如果贵公司有权访问以前购买过的Workfront目标，则Workfront管理员必须授予您以下权限才能访问Workfront目标：

1. 以下许可证之一：

   * 参与者或更高版本
   * 请求或更高版本

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. 以下访问级别：

   * 在访问级别中查看或拥有对目标的更高访问权限。

   有关访问目标的信息，请参阅[授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)。

作为Workfront管理员，您可以查看系统中Workfront目标许可证的数量，并了解当前启用的数量。 有关详细信息，请参阅[管理系统中的可用许可证](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)。

>[!NOTE]
>
>Workfront允许您分配更多已购买的Workfront Goals许可证。 但是，当您分配的许可证数超过Workfront目标合同允许的许可证数时，Workfront客户经理将会联系您，告知您超出合同数量限制。

## 将Workfront目标添加到布局模板 {#add-workfront-goals-to-a-layout-template}

您的Workfront或组管理员必须为您分配一个布局模板，该模板包括主菜单中的目标区域，以便您能够访问Workfront目标。

![布局模板](assets/layout-template-align-highlighted-350x220.png)

您的Workfront管理员或组管理员还可以将以下内容添加到您的布局模板中，以便您能够轻松访问Workfront目标：

* 固定选项卡
* 将目标区域设置为您的登陆页面

有关更新布局模板的信息，请参阅以下文章：

* [创建和管理布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [使用布局模板自定义主菜单](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [使用布局模板自定义固定页面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [使用布局模板自定义登陆页面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [将用户分配给布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 与其他用户共享个人目标 {#share-individual-goals-with-other-users}

默认情况下，所有至少具有访问级别的“查看目标”访问权限的用户都可以在Workfront中查看所有目标。

任何对目标具有“编辑”访问权限的用户都可以创建目标，并且他们会自动获得对其创建的目标的“管理”访问权限。 如果他们必须编辑其他用户的目标，则拥有这些目标管理权限的用户必须与他们共享他们未创建的目标。

有关与用户共享目标以及授予用户管理权限的信息，请参阅[在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md)。
