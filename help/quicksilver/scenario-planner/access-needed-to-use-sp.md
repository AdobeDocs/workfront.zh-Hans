---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用Scenario Planner所需的访问权限
description: Scenario Planner需要独立于Adobe Workfront的许可证和附加访问权限。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 使用[!DNL Scenario Planner]所需的访问权限

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

如果没有正确的访问权限或权限，您可能无法查看[!UICONTROL 的]方案[!DNL &#x200B; Adobe Workfront]区域，也无法管理组织的计划或计划。 管理计划和计划包括创建、编辑和删除它们。

## 查看和使用[!DNL Adobe Workfront Scenario Planner]所需的访问权限

在访问[!DNL Workfront Scenario Planner]之前，必须确保满足以下所有条件：

1. 您的组织必须具有Workfront Ultimate包。

   Scenario Planner不适用于Workfront Workflow包。

   如果您当前正在续订Workfront，并且想要保留Scenario Planner，请与您的Workfront客户代表联系。

   如果您是新客户，则无法再购买Scenario Planner。

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. 您必须拥有以下Workfront许可证之一：

   * [!UICONTROL 轻]或更高
   * [!UICONTROL 审阅者]或更高版本

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. 您的[!DNL Workfront]管理员必须为您授予访问级别为[!UICONTROL 的]查看[!UICONTROL 或]编辑[!DNL Scenario Planner]访问权限。

   有关授予[!DNL Workfront Scenario Planner]访问权限的信息，请参阅[授予 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)访问权限。

1. （可选且推荐）要查看或更新计划和计划的财务信息，您的[!DNL Workfront]管理员还必须授予您访问级别为[!UICONTROL 财务数据]的访问权限。 有关在访问级别授予财务数据的信息，请参阅[授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

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


