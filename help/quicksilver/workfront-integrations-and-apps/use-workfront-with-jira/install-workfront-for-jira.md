---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 安装 [!DNL Adobe Workfront] 表示 [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront] 表示 [!DNL Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# 安装 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。

安装加载项后，您可以定义创建 [!DNL Jira] 在 [!DNL Workfront] 将创建工作项。 两个应用程序中的项目都会链接起来，并且这两个系统中的某些项目信息会自动更新。

中的所有用户 [!DNL Workfront] 和 [!DNL Jira] 可以从此集成中受益。 他们只需要获得最常工作的系统的许可证，而不需要两个系统的许可证。

此加载项适用于 [!UICONTROL 服务器] 和 [!UICONTROL 按需] (或 [!UICONTROL 云])版本 [!DNL Jira] 软件。 此加载项不适用于 [!DNL Data Center] 版本 [!DNL Jira] 软件。

要获取 [!DNL Jira] 版本 [!DNL Workfront for Jira] 当前支持，请参阅 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在Atlassian Marketplace上。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 计划</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 许可证概述</a>*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在 [!DNL Jira] 和 [!DNL Workfront] 专门用于此集成，而不是使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 安装 [!DNL Workfront] 表示 [!DNL Jira]

安装 [!DNL Workfront] 表示 [!DNL Jira] OnDemand与在 [!DNL Jira] 服务器实例。

你必须是 [!DNL Jira] 管理员安装 [!DNL Workfront] 附加组件。

如果您不是 [!DNL Jira] 管理员，您可以浏览 [!DNL Workfront] 附加组件，并请求安装它。 您的请求将发送到 [!DNL Jira] 管理员进行审批和安装。

有关请求在 [!DNL Jira] 应用程序，请参阅 [管理加载项的用户请求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

安装 [!DNL Workfront for Jira]:

1. 登录到 [!DNL Jira] as a [!DNL Jira] 管理员。
1. 查找 **[!DNL Workfront for Jira]** 中的附加组件 [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. 单击 **[!UICONTROL 立即获取]** 来安装它。

   安装完成后，您可以登录到 [!DNL Workfront] 从 [!DNL Jira] 和配置集成。
   [!DNL ]
有关更多信息，请参阅 [为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 有关 [!DNL Jira Server] 安装

>[!NOTE]
>
>这些要求不适用于 [!UICONTROL 按需] ([!UICONTROL 云])版本 [!DNL Jira] 软件。

尽管安装了 [!DNL Workfront] 两个 [!DNL Jira] 环境类似，在使用 [!DNL Jira Server] 安装：

* 在 [!DNL Jira]，在 **[!DNL JIRA Base URL]** 字段可能与您用来访问的URL不同 [!DNL Jira] 在您的专用服务器上。 的 **[!DNL JIRA Base URL]** 必须是使用NAT或反向代理协议连接到您的专用服务器的可公开访问的地址，因此 [!DNL Workfront] 可以访问它以向服务器发出请求。

* 您必须使用SSL加密来保护之间的通信 [!DNL Jira] 和 [!DNL Workfront]. 启用SSL时，您必须拥有证书颁发机构的完整SSL证书堆栈。 我们不支持自签名证书。
* 您必须确保 [!DNL jira.workfront.com] 域可以从公司服务器访问。 它用作 [!DNL Workfront] 和 [!DNL Jira] 和是加载项运行所必需的。

   对于出站和入站连接，还必须将以下静态IP允许列表地址添加到防火墙上的。

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   有关配置防火墙以通过 [!DNL Workfront]，请参阅 [配置防火墙](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
