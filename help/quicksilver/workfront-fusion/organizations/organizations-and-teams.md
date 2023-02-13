---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion组织和团队
description: Adobe Workfront Fusion的组织和团队功能使企业能够控制对Fusion中情景和其他功能的访问。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 组织和团队

[!DNL Adobe Workfront Fusion]的组织和团队功能使企业能够控制对Fusion中方案和其他功能的访问。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>Workfront Fusion实现工作自动化和集成，</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 
     <p>你必须是 [!DNL Workfront Fusion] 管理员。</p>
     <p>你必须是 [!DNL Workfront Fusion] 团队的管理员。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

<p>**有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 许可证</a></p>


## 组织

[!DNL Workfront Fusion] 用户属于某个组织。 您的 [!DNL Fusion] 许可证可确定贵组织中有多少活动方案和连接器可用。

[!DNL Fusion] 授权可确定组织可用的活动方案和活动应用程序的数量。 [!DNL Fusion] 在“组织”功能板上显示当前的“活动方案”和“活动应用程序”计数。

* [组织角色](#organization-roles)
* [邀请用户加入组织](#inviting-users-to-an-organization)

### 组织角色

用户在组织中具有以下角色之一：

* **[!UICONTROL 所有者]**:所有者具有组织中可用的所有权限。
* **[!UICONTROL 管理员]**:管理员角色允许用户为组织创建和管理团队和用户。
* **[!UICONTROL 会员]**:成员可以使用 [!DNL Workfront Fusion] 但无法进行组织更改。
* **[!UICONTROL 会计]**:会计角色仅允许用户在组织仪表板上查看许可证信息。
* **[!UICONTROL 应用程序开发人员]**:此角色的功能当前不可用，将在不久的将来提供。 我们目前不建议将用户分配给此角色。

### 邀请用户加入组织

默认情况下，组织所有者（或授权用户）可以邀请其他人加入其组织。

要邀请用户加入组织，请执行以下操作：

1. 单击 **[!UICONTROL 更改详细信息]** 中。
1. 选择 **[!UICONTROL 邀请新用户]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 填写用户的电子邮件地址和名称。
1. 为用户选择角色。 有关角色的更多信息，请参阅 [组织角色](#organization-roles) 在本文档中。
1. （可选）添加注释。 此注释显示在用户收到的邀请电子邮件中。
1. 单击&#x200B;**[!UICONTROL 保存]**。

[!DNL Fusion] 向特定组织发送一封包含邀请的电子邮件，并 [!UICONTROL 接受角色] 按钮。

![](assets/accept-the-role.png)

当收件人单击按钮时，他们将被重定向到邀请页面，他们可以在该页面接受邀请。

邀请将在一天后过期。

>[!NOTE]
>
>如果用户是新用户 [!DNL Fusion], [!DNL Fusion] 自动为其创建帐户，并发送一封包含临时密码的电子邮件，指示新用户登录并更改其密码。

## 团队

团队是共享特定资源访问权限的用户组。 这些资源可能包括：

* 场景
* 连接
* Webhooks
* 键
* 数据存储
* 数据结构
* 电子邮件通知设置

>[!NOTE]
>
>由于团队控制对资源的访问，因此团队有时只有一个成员很有用。 例如，培训中的用户可以创建与其个人的连接 [!DNL Google] 帐户。 任何团队成员也将能够连接到个人 [!DNL Google] 帐户，因此在这种情况下，最好让用户成为培训团队的唯一成员。

组织可以拥有所需数量的团队，并且用户可能属于一个或多个团队。

用户可以从左侧导航面板的下拉列表中选择其团队。 用户只会看到自己所属的团队。 选择团队将允许用户访问该团队的资源。

* [团队角色](#team-roles)
* [团队管理](#team-management)

### 团队角色

用户在其每个团队中都具有以下角色之一：

* **[!UICONTROL 团队管理员]**:除了其他团队角色的功能外，管理员角色还允许用户添加、删除或更改团队成员的角色。
* **[!UICONTROL 团队成员]**:团队成员角色允许用户创建和执行方案。
* **[!UICONTROL 团队监控]**:的 [!UICONTROL 监测] 角色允许用户访问方案的执行信息，但他们无法设计方案或更改其“活动”状态。
* **[!UICONTROL 团队操作员]**:的 [!UICONTROL 运算符] 角色允许用户查看执行数据并更改方案的“活动”状态。
* **[!UICONTROL 团队受限成员]**:此角色的功能当前不可用，将在不久的将来提供。 我们目前不建议将用户分配给此角色。

### 团队管理

* [创建团队](#create-a-team)
* [设置团队通知选项](#set-team-notification-options)

#### 创建团队

组织所有者和管理员能够创建团队。

要创建团队，请执行以下操作：

1. 在左侧导航面板中，单击 **[!UICONTROL 组织]**
1. 选择 **[!UICONTROL 团队]** 选项卡。
1. 单击 **[!UICONTROL 添加新团队]** 列表下。
1. 输入新团队的名称，然后单击 **添加**.

#### 设置团队通知选项

电子邮件通知选项在团队级别设置。

1. 在左侧导航面板中，单击 **[!UICONTROL 团队]**
1. 选择 **[!UICONTROL 通知选项]** 选项卡。
1. 启用您希望团队接收的通知。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">“[！方案运行中的UICONTROL警告]”</td> 
      <td> <p>在方案运行中出现警告时，会收到电子邮件</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！方案运行中的UICONTROL错误]</td> 
      <td>当运行方案时出错时，会收到电子邮件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL方案停用]</p> </td> 
      <td><p>在方案停用时接收电子邮件。</p><p><b>注意：</b> 仅当由于错误而自动停用方案时，才会通知您方案停用。 您不会收到有关手动停用方案的通知。</p><p>在某些情况下，可能会由 [!DNL Workfront Fusion] 工程团队，因为该方案会导致性能或其他问题。 在这些情况下，您不会在 [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

自动保存对通知选项所做的更改

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->