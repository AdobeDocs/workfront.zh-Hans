---
title: 停用或重新激活用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Workfront管理员，您可以停用或重新激活用户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: a907cd9d07a2912d42ae26d69815a05a1006a633
workflow-type: tm+mt
source-wordcount: '1261'
ht-degree: 0%

---

# 停用或重新激活用户

<!--Audited 2/2024-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

如果用户离开组织，您可能需要从Adobe Workfront中删除他们。 他们不应在系统中保持活动状态，因为这会给其他用户在将他们添加到更新或分配工作时，造成混淆。 当您停用某个用户时，其他用户在其搜索系统中的人员时不再看到其名称。

管理员可以在“设置”区域看到非活动用户。

您可以随时重新激活用户。

>[!IMPORTANT]
>
>我们建议您取消激活已离开组织的用户，而不是删除他们。 如果删除某个用户，则与该用户相关联的Workfront中的所有历史记录都将丢失。 这包括他们的工作分配、他们与注释、小时、文档以及他们曾经创建的所有其他对象的关联。
>
>在Workfront中停用用户会移除用户对Workfront和数字校对的许可证。 此外，不能再为用户分配工作。 当用户被停用时，该用户的Workfront许可证和验证许可证将可供其他用户使用。 已停用用户配置文件中的所有其他信息保持不变。
>
>有关删除和停用用户所产生的影响的更多信息，请参阅 [删除用户](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td>  <p>新增：标准 </p> <p>或 </p><p>当前：计划 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>. </p> </li> 
     <li> <p><b>用户</b> 将访问级别中的设置配置为 <b>编辑</b> 访问，使用 <b>创建</b> 而且至少两者 <b>用户管理员</b> 下启用的选项 <b>微调您的设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>这两个选项中的一个，如果用户 <b>管理员（组用户）</b> 启用，您必须是用户所属的组的组管理员。</p> <p>欲知关于 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

在停用Workfront管理员或Standard或Plan许可证用户之前，必须将其对象和活动与其他用户关联。

有关更多信息，请参阅 [关于停用Workfront管理员和计划许可证用户](#about-deactivating-workfront-administrators-and-plan-license-users) 本文章中。

## 取消激活用户

停用用户时，请注意以下事项：

* 用户将无法访问系统。
* 将从Frame.io查看链接、资产、项目和帐户中删除用户。
   * 重新激活用户不会自动将其添加回Frame.io项目。 您必须手动将用户重新分配给需要Frame.io协作的Workfront项目、任务和资源。
* 将保留与用户关联的所有数据。
* 您可以将已停用用户的许可证分配给另一个用户。

要停用用户，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择一个用户，单击 **更多** 图标 ![](assets/more-icon.png)，然后单击 **取消激活**.

1. 单击 **取消激活** 在出现的框中。

## 安排用户停用

作为经理，您可能希望在用户实际离开您的组织之前将其标记为停用。 例如，如果您正在与合同绑定的用户合作，则他们会在您的系统中停留一段有限的时间，并且您知道他们的终止日期。 您可以安排在当天将其停用。

Workfront管理员和计划许可证用户可在用户配置文件中查看停用日期。

要计划用户停用，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择用户的名称。

   或

   （可选）选择多个用户以安排他们批量停用。

1. 单击编辑图标 ![](assets/edit-icon.png).
1. 在显示的编辑用户框中，单击 **资源规划** 去那个地方。
1. 启用 **计划停用** 选项。

1. 在显示的日历中，指定日期和时间 **计划的停用日期**.

   >[!NOTE]
   >
   >* 在时间框中，您只能选择整小时增量，不能选择分钟。
   >* 如果您选择已经过去的当天时间，Workfront会将停用时间安排在接下来的中午12:00。 所选时间与计划取消激活的用户的计算机时区匹配。

1. 单击 **保存更改**.

   在选定日期的选定时间后的某个时间取消激活用户。 如果您选择了多个用户批量停用，则在选定日期的选定时间之后的某个时间停用所有选定用户。

我们建议您为已计划取消激活的用户生成报告，以随时了解哪些用户即将被取消激活。 不确认在停用用户后是否发生了停用。

## 重新激活用户

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 选择一个用户，单击更多图标 ![](assets/more-icon.png)，然后单击 **激活**.

1. 分配新 **访问级别**&#x200B;在下拉菜单中，然后单击 **重新激活**.

### 重新激活用户时产生的资产审查和批准影响

已停用用户将无法访问其分配的Frame.io帐户以及分配的项目、资源和审阅链接。 如果选择重新激活用户，则必须手动将其重新分配给需要Frame.io协作的项目、任务和资源。

### 重新激活用户时的验证影响

已停用用户将失去为其分配的默认验证角色和验证许可证(如果您使用Workfront Premium旧版计划)。 如果选择重新激活用户，您必须：

* 重新分配许可证(如果您使用Workfront Premium旧版计划)。 有关Workfront校对计划的详细信息，请参阅 [访问Workfront中的验证功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* 验证他们是否具有正确的验证角色。 重新激活的验证用户将分配给指定为新用户的默认验证角色的任何角色。 请参阅 [配置默认验证角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) 以了解更多信息。

## 关于停用Workfront管理员以及Standard或Plan许可用户

在停用Workfront管理员或拥有计划许可证的用户之前，请务必检查涉及该人员的Workfront对象和活动，然后根据需要将它们与其他Workfront管理员或计划许可证用户相关联。

这些对象和活动可能包括以下内容：

* 分配给用户的任务或问题
* 用户拥有的项目
* 设置为使用用户的访问权限运行的报告
* 用户拥有的模板
* 用户被设置为资源管理器的项目和模板
* Workfront管理员或计划许可证用户是默认受分配人的请求队列路由规则
* 具有包含用户的阶段的审批流程（尤其是当他们是阶段中的唯一审批者时）
* 将用户列为批准者的时间表
* 将用户列为批准者的时间表配置文件
* 验证包括用户的自动化工作流

## 在您计划用户停用时会影响资源计划

当您计划停用用户时，它们不再出现在资源规划者中作为可用于预算小时数。 如果它们仍然是资源池的一部分，则它们会显示在资源规划者中，但它们的可用性将从计划取消激活的日期开始设置为零小时。

资源规划者考虑用户的所有工作角色和任务的计划完成日期，并相应地计算资源。

有关资源规划者的详细信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
