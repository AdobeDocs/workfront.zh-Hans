---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 添加用户
description: 作为Workfront管理员或具有完全管理访问权限的用户，您可以在Workfront中添加用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: 9bcd792139f8f2f0198da943e5c63a2add32e856
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 1%

---

# 添加用户

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中添加用户的说明：
>
>* 请参阅 [在Workfront中使用Adobe Admin Console创建用户](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
>* 请参阅文章中的“添加用户”部分 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* 联系您的Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以在Adobe Workfront中通过从头开始创建个人用户或复制现有用户来添加用户。

有关如何同时导入多个用户的信息，请参阅 [导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 在配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 先决条件

在添加用户之前，请收集以下所列用户的相关信息并确定要与该用户关联的信息：

* 用户的个人信息是什么？ 您至少需要满足以下条件：

   * 全名
   * 用户名
   * 默认密码
   * 电子邮件地址

   >[!NOTE]
   >
   >您可以通过在指定Workfront对象的访问级别时微调“用户视图”设置来确定用户是否可以查看其他用户的联系信息。 有关更多信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 新用户在公司中的位置是什么？ 此人是否有直接报告？ 此人向谁报告？
* 该人担任什么职务？ 此作业角色在Workfront中存在吗？ 能够担任此职务的人数是否存在限制？ 有关创建作业角色的信息，请参阅 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
* 用户应该具有什么访问级别？ 它是否已存在，或您是否需要创建一个新的？ 有关更多信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
* 此用户应属于哪个主页组？ 该人应该属于多个组吗？ 有关群组的信息，请参阅 [群组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).
* 此用户应属于哪个主团队？ 此人应该在多个团队中吗？ 有关团队的信息，请参阅 [团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).
* 您需要将哪些自定义信息与此用户关联？

   如果在您创建的自定义字段中捕获了有关用户的信息，则在创建用户时必须准备好自定义表单。 有关自定义表单的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 从头开始创建用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 单击 **新用户>新用户** 添加尚未添加到Workfront的用户。

   或

   单击 **新用户>导入用户** 通过上传电子表格导入文件来添加用户。

   如果要导入用户，则无需继续执行这些步骤。 有关更多信息，请参阅 [导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md).

1. 在 **新用户** 框，单击 **显示高级选项**，然后配置可用选项以输入人员信息。

   有关这些选项的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 执行下列操作之一：

   * 离开 **向此人发送邀请电子邮件** 已启用。 如果您这样做，用户会收到一封电子邮件，用户可通过该邮件链接创建自己的Workfront密码。 不接受电子邮件邀请并创建Workfront密码的用户在Workfront中列为“未注册”。
   * 禁用 **向此人发送邀请电子邮件**，然后键入 **密码** 并在 **确认密码** 框中。 您需要与Workfront外的用户共享此密码。

   >[!NOTE]
   >
   >如果您的Workfront管理员启用了与Workfront的SSO集成，则 &lt;sso configuration=&quot;&quot;> 如果禁用电子邮件邀请，则会隐藏身份验证字段。 联合ID或 &lt;sso configuration=&quot;&quot;> 用户名字段仍然可见。

   >[!NOTE]
   如果贵组织已载入Admin Console，并且您通过Workfront添加了用户，则无法选择发送电子邮件邀请。
   新的Adobe用户会添加到Admin Console,Admin Console会发送一封电子邮件邀请他们完成注册流程。 所有用户必须完成注册过程才能访问任何Adobe系统。
   对于现有Adobe用户，用户可能会（也可能不会）收到有关Workfront可用的电子邮件。 这是由Adobe管理员控制的产品首选项。

1. 单击 **添加此用户**.

   或

   单击 **添加人员用户并启动其他用户** 以保存新用户并添加另一个用户。

## 复制用户以创建新用户

您可以通过复制现有用户来创建用户。

>[!NOTE]
以这种方式创建用户时，除以下信息外，所有信息都会从原始用户复制到新创建的用户：
* 个人信息部分中的信息。
* 登录时，显示：此框中选择了访问级别的默认登陆选项卡。
* 直接下属
>


要通过复制现有用户来创建新用户，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).
1. 选择要复制的用户，然后单击复制图标 ![](assets/copy-icon.png).
1. 在 **新用户** 框中，编辑新用户可用的字段。

   有关与用户关联的所有字段的信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 单击 **添加此用户**.

   或

   单击 **添加人员用户并启动其他用户** 以保存新用户并添加另一个用户。

这会在Workfront中为用户创建一个新帐户。

如果您选择了向用户发送邀请的选项，则用户应会收到一封电子邮件，用户可以在其中跟踪创建Workfront密码的链接。

>[!NOTE]
如果贵组织已载入Admin Console，并且您通过Workfront添加了用户，则无法选择发送电子邮件邀请。
新的Adobe用户会添加到Admin Console,Admin Console会发送一封电子邮件邀请他们完成注册流程。 所有用户必须完成注册过程才能访问任何Adobe系统。
对于现有Adobe用户，用户可能会（也可能不会）收到有关Workfront可用的电子邮件。 这是由Adobe管理员控制的产品首选项。
