---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 管理API密钥
description: 为了最大限度地减少API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# 管理API密钥

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

为了最大限度地减少API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。

您可以重置或删除当前管理员API密钥，配置API密钥以过期，以及删除所有用户的API密钥。

利用Workfront API的应用程序示例包括：

* 文档集成，如Dropbox、Google Drive和Workfront DAM
* Workfront移动应用程序

>[!IMPORTANT]
>
>重置或删除API密钥时，必须重新配置任何利用Workfront API并通过此API密钥验证到Workfront的应用程序，才能重新获得对Workfront的访问权限。

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

## Workfront API密钥

Workfront中的每个用户都有一个唯一的API密钥。 此密钥在用户访问利用Workfront API的集成(例如Workfront移动设备应用程序或文档集成)时按用户生成。

>[!NOTE]
>
> 您在生产环境中生成的API密钥将在每周刷新期间复制到预览环境。 在“预览”环境中生成的任何API密钥将在每周刷新期间被生产API密钥覆盖。

Workfront管理员还具有唯一的API密钥。 当应用程序使用管理员API密钥访问Workfront时，应用程序将具有Workfront的管理员访问权限。

## 管理管理员API密钥

您可以为管理员用户帐户生成、重置或删除API密钥。

>[!NOTE]
>
>您还可以通过API生成API密钥。 有关更多信息，请参阅 [事件订阅API](../../../wf-api/general/event-subs-api.md) 部分 [事件订阅API](../../../wf-api/general/event-subs-api.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统>** **客户信息。**
1. （视情况而定）执行以下操作之一：

   要生成API密钥，请执行以下操作：在 **API密钥设置** ，单击 **生成API密钥**.

   或\
   要重置API密钥，请执行以下操作：在 **API密钥设置** ，单击 **重置**，则&#x200B;**重置。**

   或

   要删除API密钥，请执行以下操作：在 **API密钥设置** ，单击 **删除**，则 **删除**.

## 为非管理员用户生成API密钥

您可以为除Workfront管理员以外的其他角色的用户生成和管理API密钥。

>[!NOTE]
>
>如果贵组织的Workfront实例通过Adobe IMS启用，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

1. （视情况而定）如果贵组织使用单点登录(SSO)访问管理，请临时禁用需要SSO身份验证的选项。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

   1. 展开 **系统**，然后单击 **单点登录(SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. 禁用需要SSO身份验证的复选框。

      例如，如果贵组织使用SAML 2.0，则禁用 **仅允许SAML 2.0身份验证**.

1. 在浏览器的地址栏中，输入以下API调用：

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**用户名**&amp;password=**密码**&amp;method=PUT

   替换 `<domain>` 以及用户的Workfront凭据的用户名和密码。

1. （视情况而定）如果您在步骤1中禁用了要求进行SSO身份验证的选项，请启用此选项。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

   1. 展开 **系统**，然后单击 **单点登录(SSO)**.

   1. 在 **类型** 下拉菜单。
   1. 选中需要SSO身份验证的复选框。

## 配置API密钥过期的时间

您可以配置API密钥，以使系统中的所有用户过期。 当用户的API密钥过期时，用户必须对使用Workfront API访问Workfront的任何应用程序进行重新身份验证。 您可以更改API密钥过期的频率。 您还可以配置API密钥在用户密码过期时是否过期。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **客户信息**.
1. 在 **API密钥设置** 区域，在 **创建后**, **API密钥过期时间** 下拉列表中，选择您希望API密钥过期的时间范围。

   当您更改此选项时，新的时间范围将从您进行更改时开始。 例如，如果您将 *1个月* to *6个月*，则API密钥将自您进行更改之日起6个月到期。

   默认情况下，API密钥每月过期。

1. 要将API密钥配置为在用户密码过期时过期，请选择 **在用户密码过期时删除API密钥**.

   默认情况下，未选择此选项。

   有关如何配置用户密码过期的信息，请参阅 [配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. 单击&#x200B;**保存**。

## 删除所有用户的API密钥

如果您担心与Workfront系统有关的特定安全漏洞，则可以同时为所有用户删除API密钥。

>[!IMPORTANT]
>
>删除所有用户的API密钥会使系统中所有用户的所有API密钥失效。 此操作将导致您在Workfront中的所有集成都失败，直到您在Workfront中生成新的API密钥并更新所有集成为止。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 展开 **系统**，然后单击 **客户信息。**

1. 在 **API密钥设置** 区域，单击 **删除所有API密钥**，然后单击 **删除** **全部**.

## 使用X.509证书限制API登录

>[!IMPORTANT]
>
>本节所述的程序仅适用于尚未载入Adobe业务平台的组织。 如果贵组织已载入Workfront业务平台，则通过Workfront API登录Adobe将不可用。
>
>有关根据贵组织是否已载入Adobe业务平台而不同的程序列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

第三方应用程序可以通过API与Workfront通信。 要提高Workfront网站的安全性，您可以将Workfront配置为通过将X.509证书上传到Workfront来限制API登录请求。 启用后，除用户名和密码外，所有通过API的登录请求都必须包含客户端证书。

>[!NOTE]
>
>如果贵组织的Workfront实例通过Adobe IMS启用，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

* [获取X.509证书](#obtain-the-x-509-certificate)
* [将证书上传到Workfront](#upload-the-certificate-to-workfront)
* [验证API登录调用是否受限](#verify-api-login-calls-are-restricted)

### 获取X.509证书 {#obtain-the-x-509-certificate}

从受信任的证书颁发机构（如Verisign）获取有效的X.509证书，并将其放置在您工作站上的临时位置。

### 将证书上传到Workfront {#upload-the-certificate-to-workfront}

从证书颁发机构获取X.509证书后，您需要将其上传到Workfront。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 展开 **系统**，然后单击 **客户信息**.

1. 在 **API密钥设置** 区域，选择 **启用X.509证书**.
1. 在您的工作站上，浏览并选择您之前下载的X.509证书。
1. （可选）单击 **查看详细信息** 在证书名称旁边，查看有关证书的以下详细信息：

   * 主题常用名
   * 主题组织
   * 主题组织单位
   * 审批者常用名
   * 审批者组织
   * 审批者组织单位
   * 序列号
   * 审批日期
   * 过期日期

1. 单击&#x200B;**保存**。

### 验证API登录调用是否受限 {#verify-api-login-calls-are-restricted}

在配置Workfront实例以要求使用X.509证书之前，请先向 `/login` 端点。 您将收到一个包含sessionID的200响应。

在通过Workfront实例中的客户信息页面要求X.509证书后，再次尝试登录。 此时，您将收到一个500错误响应，其中显示以下消息：“不受信任的请求。 请联系您的系统管理员并附加证书。”

确认需要X.509证书后，请使用额外的apiCertificate参数执行相同的登录请求，该参数设置为证书的值。 如果正确执行了此操作，您将收到包含有效sessionID的200响应。
