---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: 使用Workfront目标的要求
description: 您的Adobe Workfront管理员必须确保满足某些条件，然后才能访问Adobe Workfront目标。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 4298659c6eaf7c0370d8d88454e54aeba70f48cf
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 使用Workfront目标的要求

在您访问Adobe Workfront目标之前，您的Adobe Workfront管理员必须确保满足以下所有条件：

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 贵组织必须为Workfront Target购买正确的许可证。 有关信息，请参阅 [获取Workfront Target组织访问权限](#obtain-workfront-goals-organization-access)在本文中。

* 为您分配正确类型的Workfront许可证。 有关分配许可证类型和访问级别的信息，请参阅部分 [更新许可证类型和访问级别设置](#update-license-types-and-access-level-settings) 在本文中。

>[!NOTE]
>
>具有外部许可证类型的用户无法访问Workfront目标。

* 在访问级别授予您对目标的访问权限。 有关信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* 为您分配在主菜单中包含“目标”区域的布局模板。

   有关信息，请参阅部分 [将Workfront目标添加到布局模板](#add-workfront-goals-to-a-layout-template) 在本文中。

* 如果您必须修改您未自行创建的目标，则目标创建者必须与您共享这些目标，并为您授予这些目标的“管理”权限。

   有关信息，请参阅 [与其他用户共享单个目标](#share-individual-goals-with-other-users) 在本文中。

## 获取Workfront Target组织访问权限 {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

除了Workfront许可证之外，贵组织还必须购买其他许可证，才能让用户访问Workfront目标。 在贵组织购买其他许可证后，Workfront会为您的帐户启用Workfront目标。 有关为Workfront Target购买许可证的信息，请联系您的Workfront客户经理。

## 更新许可证类型和访问级别设置  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

您的Workfront管理员必须授予您以下Workfront许可类型之一才能访问Workfront目标：

* 计划
* 工作
* 复查
* 请求

在Workfront管理员授予您其中一种许可证类型后，他们还必须授予您访问级别中的“目标”的权限。 有关访问目标的信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

作为Workfront管理员，您可以查看系统中的Workfront Target许可证数量，并了解当前已启用的许可证数量。 有关更多信息，请参阅 [管理系统中的可用许可证](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront允许您分配已购买的更多Workfront Target许可证。 但是，如果您分配的许可证数量超过Workfront目标合同允许的数量，Workfront客户经理将联系您，以告知您您的合同编号已超出。

## 将Workfront目标添加到布局模板 {#add-workfront-goals-to-a-layout-template}

您的Workfront或组管理员必须为您分配一个布局模板，该模板在主菜单中包含目标区域，以便您能够访问Workfront目标。

![](assets/layout-template-align-highlighted-350x220.png)

您的Workfront管理员或组管理员还可以将以下内容添加到布局模板中，以便轻松访问Workfront目标：

* 固定的选项卡
* 将“目标”区域设为登陆页面

有关更新布局模板的信息，请参阅以下文章：

* [创建和管理布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [使用布局模板自定义主菜单](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [使用布局模板自定义固定的页面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [使用布局模板自定义登陆页面](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [将用户分配到布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 与其他用户共享单个目标 {#share-individual-goals-with-other-users}

默认情况下，所有在其访问级别至少具有查看目标访问权限的用户，都可以在Workfront中查看所有目标。

具有“编辑”目标访问权限的任何用户都可以创建目标，并且他们会自动获得对所创建目标的“管理”访问权限。 如果用户必须编辑其他用户的目标，则具有这些目标的“管理”权限的用户必须与他们共享他们未创建的目标。

有关与用户共享目标并为其授予“管理”权限的信息，请参阅 [在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
