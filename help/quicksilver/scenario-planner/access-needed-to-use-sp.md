---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 使用Scenario Planner所需的访问权限
description: Scenario Planner需要独立于Adobe Workfront的许可证和附加访问权限。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# 使用所需的访问权限 [!DNL Scenario Planner]

此 [!DNL Scenario Planner] 需要额外的许可证。 欲知关于 [!DNL Workfront Scenario Planner]，请参见 [此 [!DNL Scenario Planner] 概述](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

如果没有正确的访问权限或权限，您可能无法查看 [!UICONTROL 方案] 面积[!DNL  Adobe Workfront] 也不管理组织的计划或计划。 管理计划和计划包括创建、编辑和删除它们。

>[!IMPORTANT]
>
>访问时 [!UICONTROL 方案]，则只能查看和管理您创建的计划。 如果要允许其他用户查看或管理您创建的计划，必须执行以下操作：
>
>* 向其他用户发送指向您的计划的链接
>* 与其他用户共享计划
>
>  有关共享计划的信息，请参阅 [在中共享计划 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>停用用户时，其计划没有所有者，除非之前与链接共享，否则无法访问。

## 查看和使用所需的访问权限 [!DNL Adobe Workfront Scenario Planner]

您必须确保满足所有以下条件，然后才能访问 [!DNL Workfront Scenario Planner]：

1. 您的组织必须具有如下所述的Workfront计划之一。

   根据您使用的是新计划还是当前Workfront计划，您的组织必须具有以下任一项：

   * 对于当前计划，您的组织必须具有以下任一项：

      * 此 [!UICONTROL Ultimate] [!DNL Workfront] 计划。 Scenario Planner包含在最终计划中。

        或

      * 此 [!UICONTROL 选择] 或 [!UICONTROL Prime] [!DNL Workfront] 计划，另外购买单独的 [!DNL Scenario Planner] 许可证。

   * 对于当前的Workfront计划，您的组织必须同时具备以下两个条件：

      * 您的组织必须购买 [!DNL Workfront] [!UICONTROL 商业] 或更高 [!DNL Workfront] 计划。 欲知关于 [!DNL Workfront] 计划，请参阅 [Workfront计划](https://workfront.com/plans).

      * 您的组织必须购买 [!DNL Workfront Scenario Planner] 除了许可证之外， [!DNL Workfront] 许可证。 联系 [!DNL Workfront] 要了解的客户代表 [!DNL Workfront Scenario Planner] 许可证。

1. 您必须拥有如下所述的Workfront许可证之一。

   根据您使用的是新许可证还是当前许可证， [!DNL Workfront] 管理员必须为您分配以下任意类型的许可证：

   * 对于新许可证：
      * [!UICONTROL 标准]
      * [!UICONTROL 浅色]

   * 对于当前许可证：

      * [!UICONTROL 计划]
      * [!UICONTROL 工作]
      * [!UICONTROL 审核]

   >[!NOTE]
   > 
   >* 使用新许可证时，具有 [!UICONTROL 投稿人] 或 [!UICONTROL 外部] 许可证类型无法访问 [!DNL Scenario Planner].
   >
   >* 使用当前许可证时，具有“请求”或“外部”许可证类型的用户无法访问Scenario Planner。

1. 您的 [!DNL Workfront] 管理员必须提供您 [!UICONTROL 视图] 或 [!UICONTROL 编辑] 访问 [!DNL Scenario Planner] 在访问级别中。

   有关授予对 [!DNL Workfront Scenario Planner]，请参见 [授予访问权限 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. （可选，推荐）要查看或更新计划和计划的财务信息，请 [!DNL Workfront] 管理员还必须授予您访问 [!UICONTROL 财务数据] 在访问级别中。 有关在访问级别授予财务数据的信息，请参见 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. （可选）如果您需要访问未创建的计划，则计划创建者必须向您授予其计划的正确权限才能访问它。 有关访问未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 部分。

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## 查看计划和计划所需的访问权限

除了您的公司为获取正确的许可证之外， [!DNL Workfront Scenario Planner]，您的 [!DNL Workfront] 管理员还必须为您分配以下访问和设置，以便您能够查看 [!DNL Workfront Scenario Planner] 以及此区域中的信息：

* 访问级别至少为 [!UICONTROL 视图] 访问 [!DNL Scenario Planner].

  有关对的访问级别的信息 [!DNL Scenario Planner]，请参见 [授予访问权限 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 访问级别至少为 [!UICONTROL 视图] 访问 [!UICONTROL 财务数据] 如果您还需要查看有关计划和计划的财务信息。 财务信息的一些示例包括预算、成本或工作角色费率。

  欲知关于 [!UICONTROL 财务数据] 访问级别，请参见 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL 请求者] 和 [!UICONTROL 外部] 用户无权查看 [!DNL Scenario Planner].

* 查看计划的权限。 有关访问未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 部分。

## 管理计划和计划所需的访问权限

您的 [!DNL Workfront] 管理员必须为您分配以下访问权限，以便您能够在以下位置管理计划及其信息： [!DNL Scenario Planner]：

* A [!UICONTROL 计划] 或 [!UICONTROL 工作] 许可证类型，具有对的编辑访问权限 [!DNL Scenario Planner] 在访问级别中。

  所有其他许可证类型无权管理计划。

  有关授予访问权限的信息 [!DNL Scenario Planner] 在访问级别中，请参阅 [授予访问权限 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL 计划] 使用的许可证类型 [!UICONTROL 编辑] 访问 [!UICONTROL 财务数据] 在访问级别上，如果您还需要更新有关计划的财务信息。

  您可以编辑的一些财务信息示例包括 [!UICONTROL 预算]， [!UICONTROL 计划收益]、和 [!UICONTROL 固定成本].

  >[!TIP]
  >
  >仅 [!UICONTROL 计划] 许可证持有者拥有 [!UICONTROL 编辑] 访问 [!UICONTROL 财务数据].

  欲知关于 [!UICONTROL 财务数据] 访问级别，请参见 [授予对财务数据的访问权限](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 管理您未创建计划的权限。 有关访问未创建的计划和计划所需的权限的信息，请参阅 [访问计划和计划所需的权限](#permissions-needed-to-access-plans-and-initiatives) 部分。

## 访问计划和计划所需的权限

访问级别与中的权限配合使用 [!DNL Workfront] 以便您能够查看未创建的计划和计划。 除了具有正确的访问级别之外， [!DNL Scenario Planner]，您还必须对要查看或管理的计划具有正确的权限（如果您不是这些计划的创建者）。

默认情况下，您只能访问您创建的计划。 要查看其他用户创建的计划，他们必须与您共享他们的计划。 有关共享计划的信息，请参阅 [在中共享计划 [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

如果用户共享指向计划的链接而没有共享该计划，则您可以请求对该计划的权限。 有关向计划请求权限的信息，请参阅 [在中请求对计划的访问权限 [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

