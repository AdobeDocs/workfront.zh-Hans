---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用Scenario Planner所需的访问权限
description: Scenario Planner需要独立于Adobe Workfront的许可证和附加访问权限。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 0%

---

# 使用[!DNL Scenario Planner]所需的访问权限

<!--Audited: 04/2024-->

[!DNL Scenario Planner]具有额外的许可证要求。 有关[!DNL Workfront Scenario Planner]的信息，请参阅[概述 [!DNL Scenario Planner] ](../scenario-planner/scenario-planner-overview.md)。

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

如果没有正确的访问权限或权限，您可能无法查看[!DNL  Adobe Workfront]的[!UICONTROL 方案]区域，也无法管理组织的计划或计划。 管理计划和计划包括创建、编辑和删除它们。

## 查看和使用[!DNL Adobe Workfront Scenario Planner]所需的访问权限

在访问[!DNL Workfront Scenario Planner]之前，必须确保满足以下所有条件：

1. 您的组织必须具有如下所述的Workfront计划之一。

   根据您使用的是新计划还是当前Workfront计划，您的组织必须具有以下任一项：

   * 对于新计划，您的组织必须具有[!UICONTROL Ultimate] [!DNL Workfront]计划。 Scenario Planner仅包含在[!UICONTROL Ultimate]计划中。

   * 对于当前的Workfront计划，您的组织必须同时具备以下两个条件：

      * 您的组织必须购买[!DNL Workfront] [!UICONTROL 业务]或更高版本[!DNL Workfront]计划。 有关[!DNL Workfront]计划的信息，请参阅[Workfront计划](https://www.workfront.com/plans)。

      * 除了购买[!DNL Workfront]许可证外，您的组织还必须购买[!DNL Workfront Scenario Planner]许可证。 请联系您的[!DNL Workfront]客户代表以了解[!DNL Workfront Scenario Planner]许可证。

1. 您必须拥有如下所述的Workfront许可证之一。

   根据您使用新许可证还是当前许可证，[!DNL Workfront]管理员必须为您分配以下任意类型的许可证：

   * 对于新许可证：
      * [!UICONTROL 标准]
      * [!UICONTROL 亮]

   * 对于当前许可证：

      * [!UICONTROL 计划]
      * [!UICONTROL 工作]
      * [!UICONTROL 审核]

   >[!NOTE]
   > 
   >* 使用新许可证时，具有[!UICONTROL 参与者]或[!UICONTROL 外部]许可证类型的用户无法访问[!DNL Scenario Planner]。
   >
   >* 使用当前许可证时，具有“请求”或“外部”许可证类型的用户无法访问Scenario Planner。

1. 您的[!DNL Workfront]管理员必须为您授予访问级别为[!DNL Scenario Planner]的[!UICONTROL 查看]或[!UICONTROL 编辑]访问权限。

   有关授予[!DNL Workfront Scenario Planner]访问权限的信息，请参阅[授予 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)访问权限。

1. （可选且推荐）要查看或更新计划和计划的财务信息，您的[!DNL Workfront]管理员还必须授予您访问级别为[!UICONTROL 财务数据]的访问权限。 有关在访问级别授予财务数据的信息，请参阅[授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

1. （可选）如果您需要访问未创建的计划，则计划创建者必须向您授予其计划的正确权限才能访问它。 有关访问未创建的计划和计划所需的权限的信息，请参阅本文中的[访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives)部分。

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## 查看计划和计划所需的访问权限

除了您的公司获得[!DNL Workfront Scenario Planner]的正确许可证外，[!DNL Workfront]管理员还必须为您分配以下访问和设置，以便您可以查看[!DNL Workfront Scenario Planner]和此区域中的信息：

* 对[!DNL Scenario Planner]具有至少[!UICONTROL 查看]访问权限的访问级别。

  有关[!DNL Scenario Planner]访问级别的信息，请参阅[授予对 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的访问权限。

* 访问级别至少具有[!UICONTROL 查看]访问[!UICONTROL 财务数据]的权限（如果您还需要查看有关计划和计划的财务信息）。 财务信息的一些示例包括预算、成本或工作角色费率。

  有关[!UICONTROL 财务数据]访问级别的信息，请参阅[授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

  >[!TIP]
  >
  >[!UICONTROL 请求者]和[!UICONTROL 外部]用户无权查看[!DNL Scenario Planner]。

* 查看计划的权限。 有关访问未创建的计划和计划所需的权限的信息，请参阅本文中的[访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives)部分。

## 管理计划和计划所需的访问权限

您的[!DNL Workfront]管理员必须为您分配以下访问权限，以便您可以在[!DNL Scenario Planner]中管理计划及其信息：

* [!UICONTROL 计划]或[!UICONTROL 工作]许可证类型，具有访问级别中[!DNL Scenario Planner]的“编辑”访问权限。

  所有其他许可证类型无权管理计划。

  有关从访问级别授予对[!DNL Scenario Planner]的访问权限的信息，请参阅[授予对 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)的访问权限。

* 如果还需要更新计划的财务信息，则在您的访问级别具有[!UICONTROL 编辑]访问[!UICONTROL 财务数据]权限的[!UICONTROL 计划]许可证类型。

  您可以编辑的财务信息示例包括[!UICONTROL 预算]、[!UICONTROL 计划收益]和[!UICONTROL 固定成本]。

  >[!TIP]
  >
  >只有[!UICONTROL 计划]许可证持有人具有[!UICONTROL 编辑]权限，可访问[!UICONTROL 财务数据]。

  有关[!UICONTROL 财务数据]访问级别的信息，请参阅[授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

* 管理您未创建计划的权限。 有关访问未创建的计划和计划所需的权限的信息，请参阅本文中的[访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives)部分。

## 访问计划和计划所需的权限

访问级别与[!DNL Workfront]中的权限配合使用，让您能够查看未创建的计划和计划。 除了具有访问[!DNL Scenario Planner]的正确访问级别之外，如果您不是计划的创建者，则还必须对要查看或管理的计划具有正确的权限。

所有用户（包括系统管理员）只能访问他们创建的计划。

要查看其他用户创建的计划，他们必须通过以下方式与您共享他们的计划：

* 与您共享计划

  有关共享计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md)中共享计划。

* 发送指向他们创建的计划的链接

  如果用户共享指向计划的链接而没有共享该计划，则您可以请求对该计划的权限。 有关请求对计划的权限的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)中请求对计划的访问权限。

>[!NOTE]
>
>停用用户时，其计划没有所有者，除非之前与链接共享，否则无法访问。


