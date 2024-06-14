---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 安装 [!DNL Adobe Workfront] 对象 [!DNL Jira]
description: 您可以使用 [!DNL Adobe Workfront] 对象 [!DNL Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# 安装 [!DNL Adobe Workfront for Jira]

您可以使用 [!DNL Adobe Workfront for Jira] 集成 [!DNL Jira] 和 [!DNL Workfront] 系统。

安装加载项后，您可以定义用于创建 [!DNL Jira] 出现以下情况时自动问题 [!DNL Workfront] 将创建工作项。 两个应用程序中的项目会相互链接，并且其中的一些信息可以在两个系统中自动更新。

中的所有用户 [!DNL Workfront] 和 [!DNL Jira] 将受益于此集成。 他们只需要许可证就可以使用他们最常使用的系统，而不需要许可证就可以同时使用两个系统。

此加载项可用于 [!UICONTROL 服务器] 和 [!UICONTROL 按需] (或 [!UICONTROL 云])个版本 [!DNL Jira] 软件。 此加载项不可用于 [!DNL Data Center] 版本 [!DNL Jira] 软件。

对于 [!DNL Jira] 版本 [!DNL Workfront for Jira] 当前支持，请参阅 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) 在Atlassian集市。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> 
   <p>新建：任何</p>
   <p>当前： [！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] 许可证概述</td> 
   <td> 
   <p>新增：标准</p>
   <p>当前： [！UICONTROL计划]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在中创建单独的系统管理员帐户 [!DNL Jira] 和 [!DNL Workfront] 以专门用于此集成，而不使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td><p>您必须是 [!DNL Workfront] 管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 安装 [!DNL Workfront] 对象 [!DNL Jira]

安装 [!DNL Workfront] 对象 [!DNL Jira] OnDemand与将其安装在 [!DNL Jira] 服务器实例。

您必须是 [!DNL Jira] 管理员安装 [!DNL Workfront] 加载项。

如果您不是 [!DNL Jira] 管理员，您可以浏览 [!DNL Workfront] 加载项并请求安装它。 您的请求将发送至 [!DNL Jira] 管理员审批和安装。

有关请求在您的计算机上安装加载项的更多信息， [!DNL Jira] 应用程序，请参阅 [管理加载项的用户请求。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

安装 [!DNL Workfront for Jira]：

1. 登录 [!DNL Jira] as a [!DNL Jira] 管理员。
1. 查找 **[!DNL Workfront for Jira]** 中的加载项 [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. 单击 **[!UICONTROL 立即获取]** 安装它。

   安装完成后，您可以登录到 [!DNL Workfront] 从 [!DNL Jira] 并配置您的集成。

   有关更多信息，请参阅 [为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 有关的注意事项 [!DNL Jira Server] 安装

>[!NOTE]
>
>这些要求不适用于 [!UICONTROL 按需] ([!UICONTROL 云])版本 [!DNL Jira] 软件。

尽管安装了 [!DNL Workfront] 这两者中的附加功能 [!DNL Jira] 环境是相似的，使用时必须考虑以下事项 [!DNL Jira Server] 安装：

* 在中配置加载项时 [!DNL Jira]，中指定的地址 **[!DNL JIRA Base URL]** 字段可能与您用于访问的URL不同 [!DNL Jira] 您的专用服务器上。 此 **[!DNL JIRA Base URL]** 必须是可公开访问的地址，并使用NAT或反向代理协议连接到您的专用服务器，因此 [!DNL Workfront] 可以访问它以向服务器发出请求。

* 您必须使用SSL加密来保护以下两种协议之间的通信 [!DNL Jira] 和 [!DNL Workfront]. 启用SSL时，必须从证书颁发机构获得完整的SSL证书栈栈。 我们不支持自签名证书。
* 您必须确保 [!DNL jira.workfront.com] 可以从您的公司服务器访问域。 它充当中间件环境，介于 [!DNL Workfront] 和 [!DNL Jira] 并且是加载项运行所必需的。

  您还必须将以下静态IP地址添加到防火墙上的允许列表中，以便进行出站和入站连接。

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  有关配置防火墙以使其具有最佳功能的详细信息 [!DNL Workfront]，请参见 [配置防火墙](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
