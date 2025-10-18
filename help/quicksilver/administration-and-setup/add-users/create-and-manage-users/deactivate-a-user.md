---
title: 停用或重新激活用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Workfront管理员可以停用或重新激活用户。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 2%

---

# 停用或重新激活用户 {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="停用用户"
>abstract="停用用户会将其从 Workfront 和 Frame.io 中移除。已停用的用户稍后可以重新激活。"

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

如果用户离开组织，建议在系统中取消激活他们，以避免在将其添加到更新或分配工作时，给其他用户造成混淆。 当您停用某个用户时，其他用户在其搜索系统中的人员时不再看到其名称。

管理员可以在“设置”区域看到非活动用户。

您可以随时重新激活用户。

>[!IMPORTANT]
>
>* 我们建议您取消激活已离开组织的用户，而不是删除他们。 如果删除某个用户，则与该用户相关联的Workfront中的所有历史记录都将丢失。 这包括他们的工作分配、他们与注释、小时、文档以及他们曾经创建的所有其他对象的关联。
>
>* 在Workfront中停用用户会移除用户对Workfront和数字校对的许可证。 此外，不能再为用户分配工作。 当用户被停用时，该用户的Workfront许可证和验证许可证将可供其他用户使用。 已停用用户配置文件中的所有其他信息保持不变。
>
>* 在Workfront中停用用户不会从Adobe Admin Console的Workfront产品配置文件中删除该用户。 有关详细信息，请参阅[删除用户](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在停用Workfront管理员或Standard或Plan许可证用户之前，必须将其对象和活动与其他用户关联。

有关详细信息，请参阅本文中的[关于停用Workfront管理员以及Standard或Plan许可证用户](#about-deactivating-workfront-administrators-and-plan-license-users)。

## 停用用户

停用用户时，请注意以下事项：

* 用户将无法访问系统。
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* 将保留与用户关联的所有数据。
* 您可以将已停用用户的许可证分配给另一个用户。

要停用用户，请执行以下操作：

{{step-1-to-users}}

1. 在用户列表中选择用户。
1. 单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**停用**。

1. 在&#x200B;**停用用户**&#x200B;对话框中，单击&#x200B;**停用**。

## 安排用户停用

作为经理，您可能希望在用户实际离开您的组织之前将其标记为停用。 例如，如果您正在与合同绑定的用户合作，则他们会在您的系统中停留一段有限的时间，并且您知道他们的终止日期。 您可以安排在当天将其停用。

Workfront管理员和计划许可证用户可在用户配置文件中查看停用日期。

要计划用户停用，请执行以下操作：

{{step-1-to-users}}

1. 在用户列表中选择用户。

   或

   （可选）选择多个用户以安排他们批量停用。

1. 单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
1. 在&#x200B;**编辑用户**&#x200B;框的左侧面板中，单击&#x200B;**资源计划**。
1. 单击&#x200B;**设置停用日期**。

1. 选择&#x200B;**停用日期**&#x200B;的日期和时间。

   >[!NOTE]
   >
   >* 在时间框中，您只能选择整小时增量，不能选择分钟。
   >* 如果您选择已经过去当天的一个时间，Workfront将安排第二天凌晨12:00取消激活。
   >* 所选时间与计划取消激活的用户的计算机时区匹配。

1. 单击&#x200B;**保存**。

在选定日期的选定时间后的某个时间取消激活用户。 如果您选择了多个用户批量停用，则在选定日期的选定时间之后的某个时间停用所有选定用户。

我们建议您为已计划取消激活的用户构建一个报表，以随时了解哪些用户即将取消激活。 在停用用户后，不会确认是否已发生停用。

## 重新激活用户

{{step-1-to-users}}

1. 选择一个用户，单击&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**激活**。

1. 在&#x200B;**重新激活用户**&#x200B;对话框中，从下拉菜单中选择新的&#x200B;**访问级别**，然后单击&#x200B;**重新激活**。
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### 重新激活用户时的验证影响

已停用用户将失去为其分配的默认验证角色和验证许可证(如果您使用Workfront Premium旧版计划)。 如果选择重新激活用户，您必须：

* 重新分配许可证(如果您使用Workfront Premium旧版计划)。 有关Workfront验证计划的详细信息，请参阅[访问Workfront中的验证功能](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md)。
* 验证他们是否具有正确的验证角色。 重新激活的验证用户将分配给指定为新用户的默认验证角色的任何角色。 有关详细信息，请参阅[配置默认验证角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md)。

## 关于停用Workfront管理员以及Standard或Plan许可用户

在停用Workfront管理员或拥有计划许可证的用户之前，请务必检查涉及该人员的Workfront对象和活动，然后根据需要将它们与其他Workfront管理员或计划许可证用户相关联。

这些对象和活动可能包括以下内容：

* 分配给用户的任务或问题。
* 用户拥有的项目。
* 设置为使用用户的访问权限运行的报告。
* 用户拥有的模板。
* 用户被设置为资源管理器的项目和模板。
* 请求队列路由规则Workfront管理员或计划许可证用户是默认受分配人。
* 具有包含用户的阶段的审批流程（尤其是当他们是阶段中的唯一审批者时）。
* 将用户列为批准者的时间表。
* 将用户列为批准者的时间表配置文件。
* 验证包括用户的自动工作流。

## 在您计划用户停用时会影响资源计划

当您计划停用用户时，它们不再出现在资源规划者中作为可用于预算小时数。 如果它们仍然是资源池的一部分，则它们会显示在资源规划者中，但它们的可用性将从计划取消激活的日期开始设置为零小时。

资源规划者考虑用户的所有工作角色和任务的计划完成日期，并相应地计算资源。

有关资源规划者的详细信息，请参阅[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

