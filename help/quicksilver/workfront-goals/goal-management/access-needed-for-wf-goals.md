---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: 使用Workfront Goals的要求
description: 在访问Adobe Workfront目标之前，您的Adobe Workfront管理员必须确保满足某些条件。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 0%

---

# 使用Workfront Goals的要求

在访问Adobe Workfront目标之前，您的Adobe Workfront管理员必须确保满足所有以下条件：

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 您的组织必须购买Workfront Goals的正确许可证。 有关信息，请参阅部分 [获取Workfront目标组织访问权限](#obtain-workfront-goals-organization-access) 本文章中。

* 为您分配正确类型的Workfront许可证。 有关分配许可证类型和访问级别的信息，请参阅部分 [更新许可证类型和访问级别设置](#update-license-types-and-access-level-settings) 本文章中。

>[!NOTE]
>
>具有外部许可证类型的用户无法访问Workfront目标。

* 授予您访问访问级别中目标的权限。 有关信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* 为您分配包含主菜单中的目标区域的布局模板。

  >[!NOTE]
  >
  >必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。

  有关信息，请参阅部分 [将Workfront目标添加到布局模板](#add-workfront-goals-to-a-layout-template) 本文章中。

* 如果必须修改未自行创建的目标，则目标创建者必须与您共享目标并授予您管理权限。

  有关信息，请参阅部分 [与其他用户共享个人目标](#share-individual-goals-with-other-users) 本文章中。

## 获取Workfront目标组织访问权限 {#obtain-workfront-goals-organization-access}


根据贵公司当前使用的Workfront计划，存在以下情况：

* 如果贵公司有新的Workfront计划，您必须具备以下任一项：

   * 终极的Workfront计划。 Workfront目标包含在此计划中。
   * 选择或更高版本Workfront计划和单独的Workfront Goals许可证。

* 如果贵公司当前采用Workfront计划，则除了Workfront许可证外，贵组织还必须购买其他许可证，以便您的用户能够访问Workfront目标。

  在您的组织购买附加许可证后，Workfront将为您的帐户启用Workfront目标。 有关为Workfront Goals购买许可证的信息，请联系您的Workfront客户经理。

有关Workfront访问要求的信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 更新许可证类型和访问级别设置  {#update-license-types-and-access-level-settings}

根据贵公司当前使用的Workfront计划，存在以下情况：

* 如果贵公司具有新的访问级别模型，则Workfront管理员必须向您授予以下Workfront许可证类型之一才能访问Workfront目标：

   * 投稿人
   * 轻量
   * 标准

* 如果贵公司具有当前的访问级别模型，则Workfront管理员必须向您授予以下Workfront许可证类型之一才能访问Workfront目标：

   * 计划
   * 工作
   * 评论
   * 请求

在您的Workfront管理员向您授予这些许可证类型之一后，他们还必须授予您访问级别中目标的访问权限。 有关访问“目标”的信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

作为Workfront管理员，您可以查看系统中Workfront目标许可证的数量，并了解当前启用的数量。 有关更多信息，请参阅 [管理系统中的可用许可证](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Workfront允许您分配更多已购买的Workfront Goals许可证。 但是，当您分配的许可证数超过Workfront目标合同允许的许可证数时，Workfront客户经理将会联系您，告知您超出合同数量限制。

## 将Workfront目标添加到布局模板 {#add-workfront-goals-to-a-layout-template}

您的Workfront或组管理员必须为您分配一个布局模板，该模板包括主菜单中的目标区域，以便您能够访问Workfront目标。

![](assets/layout-template-align-highlighted-350x220.png)

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

有关与用户共享目标并授予他们管理权限的信息，请参阅 [在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
