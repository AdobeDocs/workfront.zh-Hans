---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：SAML 2.0身份验证失败：未找到用户标识符'
description: 当您使用SAML 2.0时，错误“未找到SAML 2.0身份验证失败用户标识符”表示未从ADFS声明规则传递UID或名称ID。 在ADFS中，信赖方信任需要具有可传递UID或NAME ID值的声明规则。 当您运行 [!DNL Workfront] 测试连接时，如果成功，应显示此内容。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# 错误消息：SAML 2.0身份验证失败：未找到用户标识符

## 问题

使用SAML 2.0时，我收到此错误：&quot;SAML 2.0身份验证失败：未找到用户标识符。”

## 原因

当 **UID** 或 **名称ID** 未从 **ADFS索赔规则**.

在ADFS中， **信赖方信任** 需要 **索赔规则** 通过 **UID** 或 **名称ID** 值。 当您运行 **[!DNL Workfront]测试连接**，如果成功，则应显示此内容。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

1. 编辑 **[!UICONTROL ADFS信息]**，在 **[!UICONTROL 信赖方信托]** >选择对象>**[!UICONTROL 编辑声明规则]**.

1. 的 **[!UICONTROL LDAP属性]** （左列）应具有 **[!UICONTROL 电子邮件地址]** （或任何唯一标识符）。

1. 的 **[!UICONTROL 传出声明类型]** （右列）应为 **[!UICONTROL 名称ID]**.

   >[!NOTE]
   >
   >它不必具有LDAP属性电子邮件地址。 可以使用任何标识用户的唯一标识符，但必须将其传递到 [!DNL Adobe Workfront] 作为 **名称ID**.
