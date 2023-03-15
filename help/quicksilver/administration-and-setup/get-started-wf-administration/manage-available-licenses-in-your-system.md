---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 管理系统中的可用许可证
description: 作为Adobe Workfront管理员，您可以访问有关Workfront帐户的信息，包括为贵组织购买的许可证数量以及当前使用的许可证数量。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# 管理系统中的可用许可证

作为Adobe Workfront管理员，您可以访问有关Workfront帐户的信息，包括为贵组织购买的许可证数量以及当前使用的许可证数量。

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
   <td> <p>您必须是Workfront管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 查看贵组织的许可证

当您为添加到Workfront的用户分配访问级别时，正在使用的许可证数量会自动更新。 有关更多信息，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

要查看系统中的许可证信息，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板的底部，单击 **系统** > **许可证**.

   有关此页面上列出的许可证的详细信息，请参阅 [Adobe Workfront许可证概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >除了Workfront许可证外，校样许可证仅适用于已购买付费Workfront Proof加载项的客户。 有关此加载项的信息，请参阅 [Workfront校样](../../workfront-proof/workfront-proof.md).

1. （视情况而定）如果您看到消息 **要设置最大值，必须添加“主页组”**，按照部分中的说明在系统中添加主组 [在“许可证”页面中添加或删除主组](#add-or-remove-a-home-group-to-the-licenses-page) 在本文中。

## 查看有关Workfront加载项的许可证的信息

在下面的屏幕快照中， **10个证明许可证中的5个** 表示此组织具有付费的Workfront Proof附加组件，且当前使用他们购买的10个Workfront Proof许可证中的5个。

![](assets/updated-licenses-page.png)

如果贵组织已购买Workfront目标，则此产品的许可证信息也会显示在此处。 在这种情况下，您可以查看以下信息：

* 您的公司已购买的Workfront Target许可证总数
* 与用户关联的Workfront Target许可证数量。 这是指在其访问级别上至少向其授予“查看目标”访问权限的用户数量。

有关Workfront目标的信息，请参阅 [Adobe Workfront目标概述](../../workfront-goals/goal-management/wf-goals-overview.md). 有关访问Workfront Target的信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>Workfront允许您分配已购买的更多Workfront Target许可证。 但是，如果您分配的许可证数量超过Workfront目标合同允许的数量，Workfront客户经理将联系您，以告知您您的合同编号已超出。

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>没有管理访问权限的用户可以使用群组报表查看许可证计数。 在“报表”选项卡中，创建新的群组报表并添加以下列：>
>* 许可证类型限制：工作程序限制
>* 许可证类型限制：计划员限制
>
>要了解有关创建报告的更多信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 在“许可证”页面中添加或删除主组 {#add-or-remove-a-home-group-to-the-licenses-page}

使用此功能需要企业或企业Workfront计划。 有关各种可用计划的更多信息，请参阅 [Workfront计划。](https://www.workfront.com/plans)

每个用户只能分配到一个主页组。 Workfront通过计算每个家庭组中分配和当前使用的许可证数量，提供面向群组的许可证计数。

如果您看到消息 **要设置最大值，必须添加“主页组”** 在“许可证”页面上，您需要向“许可证”页面至少添加一个主组。

>[!IMPORTANT]
>
>* 为了有效管理与主组的许可证，我们建议在更新最大许可证计数之前为业务单位设置特定的主组。 有关更多信息，请参阅 [主页组概述](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* 您只能将顶级组添加为“主页组”，而不能添加子组。 如果用户将某个子组指定为其主组，则其许可证会添加到该子组以上顶级组的许可证计数中。
>


要在“许可证”页面中添加或删除主组，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板的底部，单击 **系统** > **许可证**.

1. 单击 **管理组列表**.
1. 开始在 **家庭组** 框中。
1. 要添加群组，请在显示时单击其名称。

   或

   要删除该群组，请单击其名称右侧的X图标。

1. 单击&#x200B;**保存**。

作为Workfront管理员，您可以为家庭组设置最大许可证计数，以阻止业务部门使用为其他业务单位购买的Workfront许可证。 有关说明，请参阅 [设置家庭组的最大许可证计数](#set-the-maximum-license-count-for-a-home-group) 在本文中。

## 设置家庭组的最大许可证计数 {#set-the-maximum-license-count-for-a-home-group}

作为Workfront管理员，您可以为系统中顶级主组设置最大许可证计数。 这样，您就可以阻止业务部门使用为组织内其他业务部门购买的Workfront许可证。

默认情况下，最大许可证计数设置为N/A，这表示没有限制。

组管理员可以查看在他们管理的主组中分配和使用的许可证数量。 有关更多信息，请参阅 [在新的Adobe Workfront体验中查看群组中分配和使用的许可证数量](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

要设置主组的最大许可证计数，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板的底部，单击 **系统** > **许可证**.

1. 在列表中找到主组。
1. 在 **Max** 列中，单击要为其设置最大值的值。
1. 键入最大数，然后按Enter。

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >要将组的最大许可证值设置回默认值，请不要键入0。 而是删除框中的数字。 将最大许可证值设置为0表示没有分配给该组的许可证。
