---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 在Microsoft Exchange中配置POP
description: ' [!DNL Microsoft Exchange] 中的POP电子邮件帐户已禁用。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---

# 在[!DNL Microsoft Exchange]中配置POP

## 问题

[!DNL Microsoft Exchange]中的POP电子邮件帐户已禁用。

## 解决方案

在花费时间解决问题之前，请确保已正确配置用户的POP帐户。 如果在确认POP帐户配置正确后继续遇到问题，请联系[!DNL Microsoft]支持部门或其合作伙伴之一以获取其他帮助。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是[!DNL Workfront]管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在[!DNL Microsoft Exchange]中配置POP

>[!NOTE]
>
>以下步骤可用作在生产[!DNL Workfront]系统的[!DNL Microsoft Exchange]中配置POP的常规指南。 根据Exchange的版本或Microsoft所做的代码更改，这些步骤可能会有显着差异。

1. 在Exchange 2010服务器上启动并启用POP3服务。

   >[!NOTE]
   >
   >默认情况下，POP3服务不启动。

   1. 启动[!DNL Microsoft]的服务器管理器。
   1. 导航： **[!UICONTROL 服务器管理器]** > **[!UICONTROL 配置]** >**[!UICONTROL 高级安全Windows防火墙]** > **[!UICONTROL 服务]**。

   1. 右键单击&#x200B;**[!DNL Microsoft Exchange]POP3**，然后单击&#x200B;**[!UICONTROL 属性]**。

   1. （视情况而定）要确保POP服务自动启动，请在&#x200B;**[!UICONTROL 常规]**&#x200B;选项卡上将&#x200B;**[!UICONTROL 启动]**&#x200B;类型设置为[!UICONTROL 自动]。

1. 为服务器配置POP3。

   1. 启动[!DNL Microsoft Exchange]管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL Exchange内部部署]** > **[!UICONTROL 服务器配置]** > **[!UICONTROL 客户端访问]**。

   1. 选择&#x200B;**[!UICONTROL POP3]**。

      POP3位于[!UICONTROL POP3]和[!UICONTROL IMAP4]选项卡下的列表中。

   1. 在右侧&#x200B;**[!UICONTROL 操作]**&#x200B;下，选择&#x200B;**[!UICONTROL POP3]**，然后选择&#x200B;**[!UICONTROL 属性]**。

   1. 单击&#x200B;**[!UICONTROL POP3属性]**，然后打开&#x200B;**[!UICONTROL 绑定]**&#x200B;选项卡。

      为POP3服务器配置的所有可用IP地址和端口号都会显示。 顶框显示未加密，底框显示SSL/TLS连接的IP和端口。

   1. 单击&#x200B;**[!UICONTROL POP3属性]**，然后打开&#x200B;**[!UICONTROL 身份验证]**&#x200B;选项卡。

   1. **[!UICONTROL 选择Secure]**&#x200B;登录。

      客户端向服务器进行身份验证需要TLS连接。

1. 启用或允许用户连接到POP。

   1. 启动[!DNL Microsoft Exchange]管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL Exchange内部部署]** > **[!UICONTROL 收件人配置]** > **[!UICONTROL 邮箱]**。

      此时将显示邮箱或用户列表。

   1. 突出显示[!DNL Workfront]中正在使用的电子邮件。
   1. 在右侧&#x200B;**[!UICONTROL 操作]**&#x200B;下，选择&#x200B;**[!UICONTROL 属性]**，然后打开&#x200B;**[!UICONTROL 邮箱功能]**&#x200B;选项卡。

   1. （视情况而定）如果POP3已禁用，请单击&#x200B;**[!UICONTROL POP3]**，然后单击&#x200B;**[!UICONTROL 启用]**。

      此时将显示邮箱或用户列表。

1. 配置接收连接器。

   1. 启动[!DNL Microsoft Exchange]管理控制台。
   1. 导航： [!DNL Microsoft] **[!UICONTROL Exchange内部部署]** > **[!UICONTROL 服务器配置]** > **[!UICONTROL 集线器传输]**。

      此时将显示接收连接器的列表。

   1. 确认接收连接器&#x200B;*客户端* *EX01*&#x200B;已启用。

      其中&#x200B;*Client* *EX01*&#x200B;是Exchange服务器的名称。

   1. 选择&#x200B;*客户端EX01*，然后在右侧&#x200B;**[!UICONTROL 操作]**&#x200B;下，选择&#x200B;**[!UICONTROL 属性]**。

   1. 打开&#x200B;**[!UICONTROL 身份验证]**&#x200B;选项卡，然后确保选中&#x200B;**[!UICONTROL 传输层安全性(TLS)]**。

      >[!NOTE]
      >
      >若要使用基本身份验证，您可能需要启动TLS和集成的Windows身份验证。
