---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用方案计划员所需的访问权限
description: 方案规划器需要与Adobe Workfront单独的许可证和附加访问权限。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# 使用所需的访问权限 [!DNL Scenario Planner]

的 [!DNL Scenario Planner] 需要额外的许可证。 有关 [!DNL Workfront Scenario Planner]，请参阅 [的 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

如果没有正确的访问权限或权限，您可能无法查看 [!UICONTROL 方案] 面积[!DNL  Adobe Workfront] 也无法管理贵组织的计划或计划。 管理计划和计划包括创建、编辑和删除计划和计划。

>[!IMPORTANT]
>
>访问 [!UICONTROL 方案]，则您只能查看和管理已创建的计划。 如果要允许其他用户查看或管理您创建的计划，则必须执行以下操作：
>
>* 将指向计划的链接发送给其他用户
>* 与其他用户共享计划
>
>  有关共享计划的信息，请参阅 [在中共享计划 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>停用用户后，其计划没有所有者，除非之前与链接共享，否则无法访问。

## 查看和使用 [!DNL Adobe Workfront Scenario Planner]

在访问 [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* 贵组织必须购买 [!DNL Workfront] [!UICONTROL 商业] 或更高 [!DNL Workfront] 计划。 有关 [!DNL Workfront] 计划，请参阅 [Workfront计划](http://workfront.com/plans).
* 贵组织必须购买 [!DNL Workfront Scenario Planner] 除 [!DNL Workfront] 许可证。 联系您的 [!DNL Workfront] 客户代表了解 [!DNL Workfront Scenario Planner] 许可证。

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* 您的 [!DNL Workfront] 管理员必须为您分配以下任何一项的许可证 [!DNL Workfront] 类型：

   * [!UICONTROL 计划]
   * [!UICONTROL 工作]
   * [!UICONTROL 复查]

   >[!NOTE]
   >
   >具有 [!UICONTROL 请求] 或 [!UICONTROL 外部] 许可证类型无法访问 [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* 您的 [!DNL Workfront] 管理员必须 [!UICONTROL 查看] 或 [!UICONTROL 编辑] 访问 [!DNL Scenario Planner] 访问级别。

   有关授予对 [!DNL Workfront Scenario Planner]，请参阅 [授予访问 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* （可选和推荐）要查看或更新您的计划和计划的财务信息，请 [!DNL Workfront] 管理员还必须授予您访问权限 [!UICONTROL 财务数据] 访问级别。 有关在访问级别授予财务数据的信息，请参阅 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* 如果您需要访问您未创建的计划，计划创建者必须授予您其计划的正确访问权限，才能访问该计划。 有关访问您未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 章节。

## 查看计划和计划所需的访问权限

除了贵公司为 [!DNL Workfront Scenario Planner]，您的 [!DNL Workfront] 管理员还必须为您分配以下访问权限和设置，以便您能够查看 [!DNL Workfront Scenario Planner] 以及这方面的信息：

* 至少具有 [!UICONTROL 查看] 访问 [!DNL Scenario Planner].

   有关访问级别的信息 [!DNL Scenario Planner]，请参阅 [授予访问 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 至少具有 [!UICONTROL 查看] 访问 [!UICONTROL 财务数据] 如果您还需要查看有关计划和计划的财务信息，请参阅。 财务信息的一些示例包括预算、成本或职务职责费率。

   有关 [!UICONTROL 财务数据] 访问级别，请参阅 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL 请求者] 和 [!UICONTROL 外部] 用户无权查看 [!DNL Scenario Planner].

* 查看计划的权限。 有关访问您未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 章节。

## 管理计划和计划所需的访问权限

您的 [!DNL Workfront] 管理员必须为您分配以下访问权限，以便您可以在 [!DNL Scenario Planner]:

* A [!UICONTROL 计划] 或 [!UICONTROL 工作] 具有编辑访问权限的许可证类型 [!DNL Scenario Planner] 访问级别。

   所有其他许可证类型都无权管理计划。

   有关授予 [!DNL Scenario Planner] 从访问级别，请参阅 [授予访问 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL 计划] 许可证类型 [!UICONTROL 编辑] 访问 [!UICONTROL 财务数据] 在访问级别中，如果您还需要更新有关计划的财务信息。

   您可以编辑的一些财务信息示例包括 [!UICONTROL 预算], [!UICONTROL 计划福利]和 [!UICONTROL 固定成本].

   >[!TIP]
   >
   >仅 [!UICONTROL 计划] 许可证持有者 [!UICONTROL 编辑] 访问 [!UICONTROL 财务数据].

   有关 [!UICONTROL 财务数据] 访问级别，请参阅 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 管理您未创建的计划的权限。 有关访问您未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 章节。

## 访问计划和计划所需的权限

访问级别与 [!DNL Workfront] 让您能够查看您未创建的计划和计划。 除了具有正确的访问级别以访问 [!DNL Scenario Planner]，则您还必须拥有要查看或管理的计划的正确权限（如果您不是这些计划的创建者）。

默认情况下，您只能访问您创建的计划。 要查看其他用户创建的计划，他们必须与您共享其计划。 有关共享计划的信息，请参阅 [在中共享计划 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

如果用户共享指向计划的链接，而又不共享计划，则您可以请求对该计划的权限。 有关请求计划权限的信息，请参阅 [请求对 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

