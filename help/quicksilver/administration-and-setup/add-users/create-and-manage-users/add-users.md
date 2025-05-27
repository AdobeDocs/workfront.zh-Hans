---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 添加用户
description: 作为Workfront管理员或具有完全管理访问权限的用户，您可以在Workfront中添加用户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e95dbc32-915b-4ea7-a5ad-e1da99edfbe3
source-git-commit: a8faf4aa1a0a1b60f61c0c981c3be1b0d9d033a4
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 1%

---

# 添加用户

<!--Audited 2/2024-->

>[!IMPORTANT]
>
>* **如果贵组织已登记到Adobe Admin Console，则必须通过Adobe Admin Console创建系统管理员。**
>
>   有关在Adobe Admin Console中创建系统管理员的说明，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。
>
>   已载入Adobe Admin Console的组织中的组管理员可以使用此过程创建用户并提交用户以供管理员审批。
>
>   有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
>
>* **如果您的组织使用单点登录(SSO)**，我们建议您在Adobe Admin Console中创建用户并将他们分配到Workfront。 可以在Workfront中创建这些用户，但根据贵组织的Admin Console的配置方式，将该信息传输到Adobe Admin Console时可能会出现问题。
>   在Adobe Admin Console中创建用户后，您可以在Workfront中配置用户信息，例如分配角色、组、团队和访问级别。
>* **如果您的组织不使用单点登录(SSO)**，则可以直接在Workfront中添加非系统管理员用户。 您可以在Adobe Admin Console中添加用户，但通过在Workfront中添加用户，您可以在创建用户时设置其访问级别，这可以节省您的时间。



您可以通过从头开始创建单个用户或复制现有用户，在Adobe Workfront中添加用户。

有关如何同时导入多个用户的信息，请参阅[导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)。

<!--
Replace this intro with something like the following when we switch to Admin Console:
As an Adobe administrator, you can add users in Adobe Workfront by adding them to your Workfront product profile in the Adobe Admin Console. For instructions, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md" class="MCXref xref">Manage users in the Adobe Admin Console</a>.
-->

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
   <td><p>新增：标准</p><p>或</p><p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <img src="assets/gear-icon-in-access-levels.png">下至少启用<b>用户管理员</b>选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在添加用户之前，请收集下面列出的用户的相关信息，并确定要与该用户关联的信息：

* 用户的个人信息是什么？ 您至少需要满足以下条件：

   * 全名
   * 用户名
   * 默认密码
   * 电子邮件地址

  >[!NOTE]
  >
  >在指定Workfront对象的访问级别时，您可以通过微调“用户视图”设置来确定用户是否可以查看其他用户的联系信息。 有关详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 新用户在公司中的位置是什么？ 此人有任何直接下属吗？ 此人向谁报告？
* 人员应担任什么工作角色？ Workfront中是否存在此工作角色？ 可以担任此工作角色的人数是否有限制？ 有关创建工作角色的信息，请参阅[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。
* 用户应该具有何种访问级别？ 是否已存在或需要创建一个新帐户？ 有关详细信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。
* 此用户应该位于哪个主组中？ 此人是否应属于多个组？ 有关组的信息，请参阅[组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)。
* 此用户应该属于哪个主团队？ 此人是否应该属于多个团队？ 有关团队的信息，请参阅[团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)。
* 您需要将哪些自定义信息与此用户关联？

  如果在您创建的自定义字段中捕获到有关用户的信息，则在创建用户时必须准备好自定义表单。 有关自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 从头开始创建用户

{{step-1-to-users}}

1. 单击&#x200B;**新用户>新用户**&#x200B;以添加尚未添加到Workfront的用户。

   或

   单击&#x200B;**新用户>导入用户**&#x200B;以通过上传电子表格导入文件来添加用户。

   如果您正在导入用户，则无需继续这些步骤。 有关详细信息，请参阅[导入用户](../../../administration-and-setup/add-users/create-and-manage-users/import-users.md)。

1. 在出现的&#x200B;**新用户**&#x200B;框中，单击&#x200B;**显示高级选项**，然后配置可用选项以输入人员信息。

   有关这些选项的信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. 执行下列操作之一：

   * 保留&#x200B;**向此人发送邀请电子邮件**&#x200B;已启用。 这样一来，用户会收到一封电子邮件，可以在其中单击链接以自行创建Workfront密码。 不接受电子邮件邀请并创建Workfront密码的用户在Workfront中将被列为“未注册”。
   * 禁用&#x200B;**向此人发送邀请电子邮件**，然后键入此人的&#x200B;**密码**，并在&#x200B;**确认密码**&#x200B;框中确认。 您需要与Workfront外部的用户共享此密码。

   >[!NOTE]
   >
   >* 如果您的Workfront管理员启用了与Workfront的SSO集成，那么如果您禁用电子邮件邀请，则仅允许&lt;SSO配置>身份验证字段会隐藏。 Federation ID或&lt;SSO配置>用户名字段仍然可见。
   >
   >* 如果贵组织已登记到Admin Console，并通过Workfront添加用户，则无法发送电子邮件邀请。
   >
   >对于现有Adobe用户，用户可能会收到也可能不会收到有关Workfront可用性的电子邮件。 这是由Adobe管理员控制的产品首选项。

1. 单击&#x200B;**添加此人**。

   或

   单击&#x200B;**添加人员并开始另一个**&#x200B;以保存新用户并添加另一个用户。

   >[!NOTE]
   >
   >* 如果您是组管理员，正在将用户添加到已载入Adobe Admin Console的组织，则此步骤的选项为&#x200B;**提交用户以供管理员审批**&#x200B;和&#x200B;**提交以供审批并启动另一个**。 用户创建时处于停用和待审批状态。
   > 
   >* 如果用户未在几分钟内从“已停用”和“未决批准”状态中移出，并且屏幕刷新未删除“未决批准”标记，则可以手动批准用户。
   >
   >1. 转到设置>用户。
   >1. 在“用户”列表中选择一个或多个用户。
   >1. 单击列表标题中的三个圆点菜单。
   >1. 选择&#x200B;**批准**。
   >1. 几分钟后，刷新页面。


## 复制用户以创建新用户

您可以通过复制现有用户来创建用户。

>[!NOTE]
>
>以这种方式创建用户时，除以下内容外，所有信息都将从原始用户复制到新创建的用户：
>
>* “个人信息”部分中的信息。
>* 登录时，显示：在此框中选择了访问级别的默认登录选项卡。
>* 直接下属
>

要通过复制现有用户来创建新用户，请执行以下操作：

{{step-1-to-users}}

1. 选择要复制的用户，然后单击“复制”图标![复制图标](assets/copy-icon.png)。
1. 在显示的&#x200B;**复制用户**&#x200B;框中，编辑可用于新用户的字段。

   有关与用户关联的所有字段的信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. 单击&#x200B;**添加此人**。

   或

   单击&#x200B;**添加人员并开始另一个**&#x200B;以保存新用户并添加另一个用户。

这会在Workfront中为用户创建一个新帐户。

如果您选择了向用户发送邀请的选项，这些用户应会收到一封电子邮件，以便他们可以通过链接创建其Workfront密码。

>[!NOTE]
>
>如果贵组织已登记到Admin Console，并通过Workfront添加用户，则无法发送电子邮件邀请。
>
>对于现有Adobe用户，用户可能会收到也可能不会收到有关Workfront可用性的电子邮件。 这是由Adobe管理员控制的产品首选项。
