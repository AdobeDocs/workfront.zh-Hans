---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置密码策略以进行身份验证
description: 作为Adobe Workfront管理员，您可以配置密码策略选项以自定义Workfront系统的身份验证体验。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 1%

---

# 配置密码策略以进行身份验证

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以配置密码策略选项以自定义Workfront系统的身份验证体验。

我们建议您在Workfront实施期间配置身份验证首选项，并且只是在以后偶尔重新访问它们。

改进的密码管理功能即将推出，或者可能已经可供您的组织使用。 根据贵组织是否有权访问新的身份验证体验，请使用以下任一部分。

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 配置身份验证（适用于所有客户） {#configure-authentication-available-for-all-customers}

将显示所有客户的身份验证选项。 改进的密码管理功能即将推出，或者可能已经可供您的组织使用，如部分所述 [配置增强的身份验证（即将推出）](#configure-enhanced-authentication-coming-soon) 在本文中。

要配置身份验证首选项，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **身份验证**.

1. 选择以下任意字段，为贵组织建立身份验证设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">强制用户重置其密码 <em>&lt;value&gt;</em> 天数</td> 
      <td>这为用户重置其Workfront密码确定了时间范围。 默认情况下，此选项处于禁用状态。 启用此选项后，您可以选择30天、60天、90天、120天、180天。 默认为30天。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允许用户设置与以前任何用户相同的密码 <em>&lt;value&gt;</em> 密码</td> 
      <td> <p>此字段禁止用户为一组重置重复使用密码。 默认情况下，此字段处于禁用状态。 启用此值后，您可以将此值设置为5、10或15，然后密码才能重复使用。</p> <p>选择此选项后，用户在指定日期内无法多次重置其密码</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果连续5次输入错误密码，请锁定帐户 <em>&lt;value&gt;</em> 分钟： </td> 
      <td> <p>选择在连续五次输入错误密码后，用户将被锁定在Workfront外的时长。 默认情况下，此选项处于启用状态，等待时间为10分钟。 您可以将帐户锁定10分钟、30分钟、1小时、8小时或24小时。 </p> <p>手动重置用户的密码将覆盖此默认等待值。 <br>当用户通过登录屏幕被锁定时，用户可以重置自己的密码。 有关如何重置密码（如果忘记）的详细信息，请参阅 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">重置密码</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密码必须至少包含 <em>&lt;value&gt;</em> 不同字符类型：</td> 
      <td> <p>通过允许您选择密码中所需的不同类型字符的数量，确定需要多强的用户密码。</p> <p>可识别的词典词不能用作密码。<br>默认情况下，Workfront要求密码中至少存在以下2个字符（对于有效密码，您还可以要求其中3个字符存在）： </p> 
       <ul> 
        <li>大写字母</li> 
        <li>小写字符</li> 
        <li>数字</li> 
        <li>符号</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

## 配置增强的身份验证（即将推出） {#configure-enhanced-authentication-coming-soon}

此部分介绍增强的身份验证体验，该体验可能尚未对贵组织可用。 如果贵组织尚未迁移到新的身份验证体验，则必须配置身份验证设置，如 [配置身份验证（适用于所有客户）](#configure-authentication-available-for-all-customers).

要配置增强的身份验证首选项，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **增强的身份验证**.
1. 在 **密码长度** 框中，输入有效密码所需的最小字符数。

   Workfront至少需要6个字符。

1. （可选）在 **密码要求** 部分，选择用户密码中所需的字符类型。

   您可以通过要求“密码要求”部分中的任意或所有类型的字符来增加用户密码的强度。 以下选项可供使用：

   | 小写字母 | 至少需要一个小写字母 |
   |---|---|
   | 大写字母 | 至少需要一个大写字母 |
   | 数字 | 至少需要一个数字 |
   | 特殊字符 | 至少需要一个特殊字符 |

   {style=&quot;table-layout:auto&quot;}

1. 单击&#x200B;**保存**。
