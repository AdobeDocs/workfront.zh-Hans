---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion组织和团队
description: 通过Adobe Workfront Fusion的“组织”和“团队”功能，企业可以控制对Fusion中场景和其他功能的访问。
author: Becky
feature: Workfront Fusion
exl-id: 601e937f-0286-4557-9a87-59aa9c0c22f1
source-git-commit: 9828fe3602342520ef203ac174990f0ea03f0588
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 组织和团队

[!DNL Adobe Workfront Fusion]的“组织”和“团队”功能使企业能够控制对Fusion中场景和其他功能的访问。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> 
     <p>您必须是 [!DNL Workfront Fusion] 组织管理员。</p>
     <p>您必须是 [!DNL Workfront Fusion] 您的团队的管理员。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

<p>**有关以下内容的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 <a href="../../workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] 许可证</a></p>


## 组织

[!DNL Workfront Fusion] 用户属于一个组织。

* [组织角色](#organization-roles)
* [邀请用户加入组织](#inviting-users-to-an-organization)
* [在组织之间切换](#switch-between-organizations)

### 组织角色

用户在组织中具有以下角色之一：

* **[!UICONTROL 所有者]**：所有者拥有组织中可用的所有权限。
* **[!UICONTROL 管理员]**：管理员角色使用户能够为组织创建和管理团队和用户。
* **[!UICONTROL 会员]**：成员可以使用 [!DNL Workfront Fusion] 但无法进行组织更改。
* **[!UICONTROL 会计师]**：会计师角色仅允许用户在组织功能板上查看许可证信息。
* **[!UICONTROL 应用程序开发人员]**：此角色的功能当前不可用，并且将在不久的将来可用。 我们建议目前不要将用户分配给此角色。

### 邀请用户加入组织

默认情况下，组织所有者（或授权用户）可以邀请其他人加入其组织。

邀请用户加入组织：

1. 单击 **[!UICONTROL 更改详细信息]** 屏幕右上角的。
1. 选择 **[!UICONTROL 邀请新用户]**.

   ![](assets/fusion-organization-invite-user-350x199.png)

1. 填写用户的电子邮件地址和名称。
1. 为用户选择角色。 有关角色的详细信息，请参阅 [组织角色](#organization-roles) 在本文档中。
1. （可选）添加注释。 此注释会显示在用户收到的邀请电子邮件中。
1. 单击&#x200B;**[!UICONTROL 保存]**。

[!DNL Fusion] 向特定组织发送一封包含邀请的电子邮件，并且 [!UICONTROL 接受角色] 按钮。

收件人单击按钮后，会被重定向到邀请页面，以便接受邀请。

邀请将在天后过期。

>[!NOTE]
>
>如果用户是新用户 [!DNL Fusion]， [!DNL Fusion] 自动为他们创建一个帐户，并发送一封包含临时密码的电子邮件，指导新用户登录并更改其密码。

### 在组织之间切换

您可能属于Fusion中的多个组织。 资源不会在组织之间共享。

您可以通过单击右上角的组织名称并从下拉菜单中选择新组织，在AdobeUnified Experience中切换组织。 只有具有Fusion帐户的组织才会显示在下拉列表中，即使您是Adobe中其他组织的成员。

## 团队

团队是共享对特定资源的访问权限的用户组。 这些资源可能包括：

* 场景
* 连接
* Webhooks
* 键
* 数据存储
* 数据结构
* 电子邮件通知设置

>[!NOTE]
>
>由于团队控制对资源的访问，因此有时团队仅有一个成员会很有用。 例如，培训用户可创建与其个人的连接 [!DNL Google] 帐户。 任何团队成员也能够连接到个人 [!DNL Google] 帐户，因此在这种情况下，用户最好是培训团队的唯一成员。

组织可以拥有所需数量的团队，并且用户可能属于一个或多个团队。

用户可以从左侧导航面板的下拉列表中选择其团队。 用户只能看到其所属的团队。 选择团队将允许用户访问该团队的资源。

* [团队角色](#team-roles)
* [团队管理](#team-management)

### 团队角色

用户在其每个团队中具有以下角色之一：

* **[!UICONTROL 团队管理员]**：除了其他团队角色的功能外，管理员角色还允许用户添加、删除或更改团队成员的角色。
* **[!UICONTROL 团队成员]**：团队成员角色允许用户创建和执行方案。
* **[!UICONTROL 团队监控]**：和 [!UICONTROL 监测] 角色允许用户访问方案的执行信息，但他们无法设计方案或更改其“活动”状态。
* **[!UICONTROL 团队操作员]**：和 [!UICONTROL 运算符] 角色允许用户查看执行数据并更改方案的“活动”状态。
* **[!UICONTROL 团队受限成员]**：此角色的功能当前不可用，并且将在不久的将来可用。 我们建议目前不要将用户分配给此角色。

有关团队角色可用的特定任务的信息，请参阅[组织和团队角色](/help/quicksilver/workfront-fusion/organizations/organization-roles.md).

### 团队管理

* [创建团队](#create-a-team)
* [设置团队通知选项](#set-team-notification-options)

#### 创建团队

组织所有者和管理员能够创建团队。

要创建团队，请执行以下操作：

1. 在左侧导航面板中，单击 **[!UICONTROL 组织]**
1. 选择 **[!UICONTROL 团队]** 选项卡。
1. 单击 **[!UICONTROL 添加新团队]** 在团队列表中。
1. 输入新团队的名称，然后单击 **添加**.

#### 设置团队通知选项

在团队级别设置电子邮件通知选项。

1. 在左侧导航面板中，单击 **[!UICONTROL 团队]**
1. 选择 **[!UICONTROL 通知选项]** 选项卡。
1. 启用您希望团队接收的通知。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">'[！UICONTROL Warning in scenario run]'</td> 
      <td> <p>在场景运行中出现警告时收到电子邮件</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL场景运行错误]</td> 
      <td>在场景运行中发生错误时收到电子邮件。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[！UICONTROL方案停用]</p> </td> 
      <td><p>在场景停用时收到电子邮件。</p><p><b>注意：</b> 仅当场景由于错误而被自动停用时，才会通知您场景停用。 您不会收到有关手动停用的方案的通知。</p><p>在某些情况下，场景可能会被停用 [!DNL Workfront Fusion] 工程团队，因为场景会导致性能或其他问题。 在这些情况下，您不会在中收到通知 [!DNL Workfront Fusion]. </p></td>

</tr>
</tbody>
</table>

自动保存对通知选项所做的更改

#### 在团队之间切换

您可能属于Fusion中的多个团队。 由于团队不共享资源，因此您可能需要切换团队以访问特定方案或其他资源。

如果贵组织不在Unified ExperienceAdobe中，则可以通过单击左侧导航中的团队名称，然后从下拉菜单中选择一个团队来切换团队。

如果您的团队位于Unified ExperienceAdobe上，您可以通过单击标题中的团队名称，然后从下拉菜单中选择团队来选择一个新团队。 此选项适用于特定团队的所有页面，如场景页面或“连接”页面。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/organization-add-team-350x181.png" style="width: 350;height: 181;"> </p>
-->