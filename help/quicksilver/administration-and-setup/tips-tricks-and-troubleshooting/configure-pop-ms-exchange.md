---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 在Microsoft Exchange中配置POP
description: 中的POP电子邮件帐户 [!DNL Microsoft Exchange] 已禁用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 在中配置POP [!DNL Microsoft Exchange]

## 问题

中的POP电子邮件帐户 [!DNL Microsoft Exchange] 已禁用。

## 解决方案

在花时间解决问题之前，请确保正确配置用户的POP帐户。 如果在确认POP帐户配置正确后继续遇到问题，请联系 [!DNL Microsoft] 支持或其某个合作伙伴以获取其他帮助。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## 在中配置POP [!DNL Microsoft Exchange]

>[!NOTE]
>
>以下步骤可用作配置POP的常规指南 [!DNL Microsoft Exchange] 用于生产 [!DNL Workfront] 系统。 根据Exchange版本或Microsoft所做的代码更改，这些步骤可能会有显着差异。

1. 在Exchange 2010服务器上启动并启用POP3服务。

   >[!NOTE]
   >
   >默认情况下，POP3服务未启动。

   1. 开始 [!DNL Microsoft]服务器管理器。
   1. 导航： **[!UICONTROL 服务器管理器]** > **[!UICONTROL 配置]** >**[!UICONTROL 具有高级安全性的Windows防火墙]** > **[!UICONTROL 服务]**.

   1. 右键单击 **[!DNL Microsoft Exchange]POP3**，然后单击 **[!UICONTROL 属性]**.

   1. （视情况而定）为确保POP服务在 **[!UICONTROL 常规]** 选项卡，设置 **[!UICONTROL 启动]** 键入 [!UICONTROL 自动].

1. 为服务器配置POP3。

   1. 启动 [!DNL Microsoft Exchange] 管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL 内部部署Exchange]** > **[!UICONTROL 服务器配置]** > **[!UICONTROL 客户端访问]**.

   1. 选择 **[!UICONTROL POP3]**.

      POP3在 [!UICONTROL POP3] 和 [!UICONTROL IMAP4] 选项卡。

   1. 在右侧，位于 **[!UICONTROL 操作]**，选择 **[!UICONTROL POP3]**，然后选择 **[!UICONTROL 属性]**.

   1. 单击 **[!UICONTROL POP3属性]**，然后打开 **[!UICONTROL 绑定]** 选项卡。

      为POP3服务器显示配置的所有可用IP地址和端口号。 顶部框显示未加密，底部框显示SSL/TLS连接的IP和端口。

   1. 单击 **[!UICONTROL POP3属性]**，然后打开 **[!UICONTROL 身份验证]** 选项卡。

   1. **[!UICONTROL 选择安全]** 登录。

      客户端需要TLS连接才能对服务器进行身份验证。

1. 启用或允许用户连接到POP。

   1. 启动 [!DNL Microsoft Exchange] 管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL 内部部署Exchange]** > **[!UICONTROL 收件人配置]** > **[!UICONTROL 邮箱]**.

      将显示邮箱或用户列表。

   1. 突出显示中使用的电子邮件 [!DNL Workfront].
   1. 在右侧，位于 **[!UICONTROL 操作]**，选择 **[!UICONTROL 属性]**，然后打开 **[!UICONTROL 邮箱功能]** 选项卡。

   1. （视情况而定）如果禁用了POP3，请单击 **[!UICONTROL POP3]**，然后单击 **[!UICONTROL 启用]**.

      将显示邮箱或用户列表。

1. 配置接收连接器。

   1. 开始 [!DNL Microsoft Exchange] 管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL 内部部署Exchange]** > **[!UICONTROL 服务器配置]** > **[!UICONTROL 集线器传输]**.

      此时将显示接收连接器列表。

   1. 确认接收连接器 *客户端* *EX01* 启用。

      其中 *客户端* *EX01* 是您的Exchange服务器的名称。

   1. 选择 *客户EX01*，然后在右下方 **[!UICONTROL 操作]**，选择 **[!UICONTROL 属性]**.

   1. 打开 **[!UICONTROL 身份验证]** 选项卡，然后确保 **[!UICONTROL 传输层安全性(TLS)]** 复选框。

      >[!NOTE]
      >
      >要进行基本身份验证，您可能需要启动TLS和集成的Windows身份验证。
