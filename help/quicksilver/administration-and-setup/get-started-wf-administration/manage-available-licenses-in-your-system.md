---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 管理系统中的可用许可证
description: 作为Adobe Workfront管理员，您可以访问有关您的Workfront帐户的信息，包括为您的组织购买的许可证数量，以及当前正在使用的许可证数量。
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# 管理系统中的可用许可证

<!-- Audited: 12/2023 -->

作为Adobe Workfront管理员，您可以访问有关您的Workfront帐户的信息，包括为您的组织购买的许可证数量，以及当前正在使用的许可证数量。

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
   <td>
    <p>新增：标准</p>
    <p>或</p>
    <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是系统管理员或组管理员。 组管理员只能查看有限的许可证信息。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

>[!NOTE]
>
>以下语句仅适用于新计划。
>
>对于Select计划：
>
>1. 系统管理员无法设置主组的限制。
>2. 系统管理员只能看到所有主组使用的许可证总数。
>3. 组管理员根本无法访问许可证页面。
>
>对于Prime和Ultimate计划：
>
>1. 系统管理员可以将主组添加到“许可证”页面以查看这些组中许可证的使用情况，还可以设置许可证限制。
>2. 组管理员可以访问“许可证”页面，并查看他们管理的组中系统管理员添加到“许可证”页面中的许可证的使用情况。
>3. 组管理员无法查看其他主组的信息或添加最大值。

+++

## 查看您组织的许可证

当您向添加到Workfront的用户分配访问级别时，会自动更新正在使用的许可证数量。 有关详细信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

要查看系统中的许可证信息，请执行以下操作：

{{step-1-to-setup}}

1. 在左面板底部，单击&#x200B;**系统** > **许可证**。

   有关此页面上列出的许可证的详细信息，请参阅[许可证概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。

   >[!NOTE]
   >
   >验证许可证仅适用于除购买Workfront许可证外还购买付费Workfront Proof加载项的客户。 有关此加载项的信息，请参阅[Workfront Proof：文章索引](../../workfront-proof/workfront-proof.md)。

1. （视情况而定）如果看到消息&#x200B;**要设置最大数，则必须添加主组**，按照本文中[在许可证页](#add-or-remove-a-home-group-to-the-licenses-page)中添加或删除主组部分中的说明在系统中添加主组。

   >[!NOTE]
   >
   >对于新计划，Select计划不允许管理员按主组查看许可证。 您只能看到已使用的许可证的总数。 Prime和Ultimate计划提供设置每个主组的最大许可证数的功能。

## 查看有关Workfront加载项许可证的信息

如果您的组织具有付费的Workfront Proof加载项，则会显示已使用的许可证数量和可用的许可证数量。 例如，10个验证许可证中的&#x200B;**5个许可证**&#x200B;指示组织当前正在使用他们购买的10个Workfront Proof许可证中的5个。

Workfront加载项的![许可证](assets/updated-licenses-page.png)

如果您的组织已购买Workfront Goals，则此产品的许可证信息也会显示在此处。 在这种情况下，您可以查看以下信息：

* 贵公司已购买的Workfront目标许可证总数
* 与用户关联的Workfront目标许可证数量。 这是在其访问级别至少授予了目标查看访问权限的用户数量。

有关Workfront目标的信息，请参阅[Adobe Workfront目标概述](../../workfront-goals/goal-management/wf-goals-overview.md)。 有关访问Workfront目标的信息，请参阅[授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)。

>[!NOTE]
>
>Workfront允许您分配更多已购买的Workfront Goals许可证。 但是，当您分配的许可证数超过Workfront目标合同允许的许可证数时，Workfront客户经理将会联系您，告知您超出合同数量限制。
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>没有管理权限的用户可以使用组报告查看许可证计数。 在报告选项卡中，创建新的组报告并添加以下列：
>
>* 许可证类型限制：工作人员限制
>* 许可证类型限制：规划者限制
>
>要了解有关创建报告的详细信息，请参阅[创建自定义报告](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 查看有关每月验证和文档决策拨款的信息

>[!IMPORTANT]
>
>验证和文档决策限制仅适用于新许可证的用户。 有关详细信息，请参阅[新许可证概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

所有非付费Workfront许可证的验证和文档决策都受到限制。 每月按用户重置限制。

每个许可证的决定限制因您采用的计划而异。 您可以在“设置”>“许可证”中查看每月分配。

有关验证和文档决策限制的更多信息，请参阅[非付费用户的有限文档和验证决策概述](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

![每月决策分配](assets/monthly-decision-allotment.png)

## 在“许可证”页面中添加或删除主组 {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

每个用户只能分配给一个主组。 Workfront通过计算每个主组中分配和当前使用的许可证数，提供了面向组的许可证计数。

如果看到消息&#x200B;**要设置最大数量，必须在“许可证”页面上添加主组**，则需要在“许可证”页面上至少添加一个主组。

>[!IMPORTANT]
>
>* 为了有效地管理主组的许可证，我们建议在更新最大许可证计数之前，为业务部门设置特定的主组。 有关详细信息，请参阅[主组概述](../../administration-and-setup/manage-groups/groups-overview/home-groups.md)。
>* 您只能将顶级组添加为主组，而不能添加子组。 如果用户将子组指定为主组，则其许可证将添加到该子组上方的顶级组的许可证计数中。
>

要在许可证页面中添加或删除主组，请执行以下操作：

{{step-1-to-setup}}

1. 在左面板底部，单击&#x200B;**系统** > **许可证**。

1. 单击&#x200B;**管理组列表**。
1. 在&#x200B;**主页组**&#x200B;框中开始键入顶级组的名称。
1. 要添加组，请在组出现时单击其名称。

   或

   要删除该组，请单击其名称右侧的X图标。

1. 单击&#x200B;**保存**。

作为Workfront管理员，您可以设置主组的最大许可证计数，以防止业务部门使用为其他业务部门购买的Workfront许可证。 有关说明，请参阅本文中的[设置主组](#set-the-maximum-license-count-for-a-home-group)的最大许可证计数。

## 设置主组的最大许可证计数 {#set-the-maximum-license-count-for-a-home-group}

作为Workfront管理员，您可以为系统中的顶级主组设置许可证最大计数。 这样，您就可以防止业务部门使用为您的组织内的其他业务部门购买的Workfront许可证。

默认情况下，许可证最大数量设置为N/A，这意味着没有限制。

组管理员可以查看他们管理的主组中分配和使用的许可证数量。 有关详细信息，请参阅[查看群组中已分配和使用许可证的数量](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)。

设置主组的最大许可证数：

{{step-1-to-setup}}

1. 在左面板底部，单击&#x200B;**系统** > **许可证**。

1. 在列表中找到主组。
1. 在组的&#x200B;**Max**&#x200B;列中，单击要为其设置最大值的值。
1. 键入最大数字，然后按Enter键。

   ![组](assets/updated-max.png)的最大许可证

   >[!NOTE]
   >
   >要将组的最大许可证值设置为默认值，请不要键入0。 请改为删除框中的数字。 将最大许可证值设置为0表示没有分配给该组的许可证。
