---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 配置身份验证的密码策略
description: 作为Adobe Workfront管理员，您可以配置密码策略选项，以自定义对Workfront系统的身份验证体验。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 4%

---

# 配置身份验证的密码策略

{{important-admin-console-onboard}}

作为Adobe Workfront管理员，您可以配置密码策略选项，以自定义对Workfront系统的身份验证体验。

我们建议您在Workfront实施期间配置身份验证首选项，之后仅偶尔会重新访问它们。

改进的密码管理功能即将推出或可能已经提供给您的组织。 使用下列任一部分，具体取决于您的组织是否有权访问新的身份验证体验。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置身份验证（适用于所有客户） {#configure-authentication-available-for-all-customers}

将为所有客户显示身份验证选项。 改进的密码管理功能即将推出，或可能已经提供给您的组织，如本文中的[配置增强身份验证)](#configure-enhanced-authentication-coming-soon)部分所述。

要配置身份验证首选项：

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **身份验证**。

1. 选择以下任意字段为您的组织建立身份验证设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">强制用户每<em>&lt;value&gt;</em>天重置一次密码</td> 
      <td>这将为用户重置其Workfront密码建立期限。 默认情况下，此选项处于禁用状态。 启用后，您可以选择30、60、90、120、180天。 默认值为30天。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允许用户将密码与其以前的<em>&lt;value&gt;</em>密码设置相同</td> 
      <td> <p>此字段禁止用户为一组重置重复使用密码。 默认情况下，此字段处于禁用状态。 启用后，您可以将此值设置为5、10或15重置，然后才能重用密码。</p> <p>选择此选项时，用户无法在指定日期内多次重置密码</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果连续输入密码不正确，请锁定帐户<em>&lt;值&gt;</em>分钟： </td> 
      <td> <p>选择连续5次输入错误密码后用户将被锁定Workfront多久。 默认启用此选项，等待时间为10分钟。 您可以锁定帐户10分钟、30分钟、1小时、8小时或24小时。 </p> <p>手动重置用户的密码将覆盖此默认等待值。 <br>用户可以通过登录屏幕锁定自己的密码。 有关他们如何重置密码的详细信息（如果忘记密码），请参阅<a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">重置密码</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密码必须包含至少<em>&lt;值&gt;</em>个不同类型的字符：</td> 
      <td> <p>通过允许您选择密码中所需的不同类型字符数，确定需要多强的用户密码。</p> <p>可识别的词典单词不能用作密码。<br>默认情况下，Workfront要求密码中至少存在下列字符中的两项（对于有效密码，也可以要求存在这些字符中的三项）： </p> 
       <ul> 
        <li>大写字符</li> 
        <li>小写字符</li> 
        <li>数字</li> 
        <li>符号</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

## 配置增强型身份验证{#configure-enhanced-authentication-coming-soon}

此部分介绍增强的身份验证体验，您的组织可能尚未提供该体验。 如果您的组织尚未迁移到新的身份验证体验，则必须配置身份验证设置，如[配置身份验证（适用于所有客户）](#configure-authentication-available-for-all-customers)中所述。

要配置增强的身份验证首选项，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **增强型身份验证**。
1. 在&#x200B;**密码长度**&#x200B;框中，输入有效密码所需的最小字符数。

   Workfront至少需要6个字符。

1. （可选）在&#x200B;**密码要求**&#x200B;部分中，选择用户密码所需的字符类型。

   通过要求“密码要求”部分中的任何或所有类型的字符，可以增加用户密码的强度。 可以使用以下选项：

   | 小写字母 | 至少需要一个小写字母 |
   |---|---|
   | 大写字母 | 至少需要一个大写字母 |
   | 数字 | 至少需要一个数字 |
   | 特殊字符 | 至少需要一个特殊字符 |

   {style="table-layout:auto"}

1. 单击&#x200B;**保存**。
