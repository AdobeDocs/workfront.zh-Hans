---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 管理API密钥
description: 为了最大程度地降低API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 2%

---

# 管理 API 密钥

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

为了最大程度地降低API安全漏洞，Adobe Workfront管理员可以管理用于使应用程序能够代表用户访问Workfront的API密钥。

您可以重置或删除当前管理员API密钥，将API密钥配置为过期，以及删除所有用户的API密钥。

以下是利用Workfront API的应用程序示例：

* 记录集成，例如Dropbox、Google Drive和Workfront DAM
* Workfront移动应用程序

>[!IMPORTANT]
>
>重置或删除API密钥时，必须重新配置任何利用Workfront API并通过此API密钥向Workfront进行身份验证的应用程序，才能重新获得对Workfront的访问权限。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Workfront API密钥

Workfront中的每个用户都有一个唯一的API密钥。 当用户访问利用Workfront API的集成(例如Workfront移动应用程序或文档集成)时，将生成此密钥。

>[!NOTE]
>
> 在每周刷新期间，您在生产环境中生成的API密钥将会复制到预览环境中。 在每周刷新期间，您在“预览”环境中生成的任何API密钥都将由生产API密钥覆盖。

Workfront管理员还有唯一的API密钥。 当应用程序使用管理员API密钥访问Workfront时，该应用程序具有Workfront的管理员访问权限。

## 管理管理员API密钥

您可以为管理员用户帐户生成、重置或删除API密钥。

>[!NOTE]
>
>您还可以通过API生成API密钥。 有关详细信息，请参阅[事件订阅API](../../../wf-api/general/event-subs-api.md)中的[事件订阅API](../../../wf-api/general/event-subs-api.md)部分。

{{step-1-to-setup}}

1. 单击&#x200B;**系统>** **客户信息。**
1. （视情况而定）执行以下操作之一：

   要生成API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**生成API密钥**。

   或\
   要重置API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**重置**，然后单击&#x200B;**重置。**

   或

   要删除API密钥：在&#x200B;**API密钥设置**&#x200B;部分中，单击&#x200B;**删除**，然后单击&#x200B;**删除**。

## 为非管理员用户生成API密钥

您可以为非Workfront管理员角色的用户生成和管理API密钥。

>[!NOTE]
>
>如果您组织的Workfront实例已启用Adobe IMS，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

1. （视情况而定）如果您的组织使用单点登录(SSO)访问管理，请暂时禁用需要SSO身份验证的选项。

   {{step-1-to-setup}}

   1. 展开&#x200B;**系统**，然后单击&#x200B;**单点登录(SSO)**。
   1. 在&#x200B;**类型**&#x200B;字段中，选择贵组织使用的SSO类型。
   1. 选定类型后，向下滚动并清除&#x200B;**启用**&#x200B;复选框。
      ![启用SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. 单击&#x200B;**保存**。


1. 在浏览器的地址栏中，输入以下API调用：

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**用户名**&amp;password=**密码**&amp;method=PUT

   将`<domain>`替换为您的Workfront域名，并将用户名和密码替换为用户的Workfront凭据。

1. （视情况而定）如果在步骤1中禁用了SSO身份验证，请启用该选项。

   {{step-1-to-setup}}

   1. 展开&#x200B;**系统**，然后单击&#x200B;**单点登录(SSO)**。

   1. 在&#x200B;**类型**&#x200B;下拉菜单中选择您的SSO方法。
   1. 选中要求SSO身份验证的复选框。

## 配置API密钥过期时间

您可以将API密钥配置为对系统中的所有用户过期。 当用户的API密钥过期时，用户必须向使用Workfront API访问Workfront的任何应用程序重新进行身份验证。 您可以更改API密钥的过期频率。 您还可以配置API密钥在用户密码过期时是否过期。

{{step-1-to-setup}}

1. 单击&#x200B;**系统** > **客户信息**。
1. 在&#x200B;**API密钥设置**&#x200B;区域的&#x200B;**创建**&#x200B;后&#x200B;**API密钥在**&#x200B;下拉列表中过期，请选择希望API密钥过期的时间范围。

   更改此选项时，新时间范围从您进行更改时开始。 例如，如果您将此选项从&#x200B;*1个月*&#x200B;更改为&#x200B;*6个月*，则API密钥将在您进行更改后6个月过期。

   默认情况下，API密钥每月过期。

1. 若要将API密钥配置为在用户密码过期时过期，请启用&#x200B;**在用户密码过期时删除API密钥**。

   默认情况下，不启用此选项。

   有关如何配置用户密码过期的信息，请参阅[配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

1. 单击&#x200B;**保存**。

## 删除所有用户的API密钥

如果您担心您的Workfront系统存在特定的安全漏洞，则可以同时为所有用户删除API密钥。

>[!IMPORTANT]
>
>删除所有用户的API密钥将导致系统中所有用户的所有API密钥失效。 此操作将导致Workfront中的所有集成失败，直到您在Workfront中生成新的API密钥并更新所有集成为止。

{{step-1-to-setup}}

1. 展开&#x200B;**系统**，然后单击&#x200B;**客户信息**。

1. 在&#x200B;**API密钥设置**&#x200B;区域中，单击&#x200B;**删除所有API密钥**，然后单击&#x200B;**删除**&#x200B;**全部**。

## 使用X.509证书限制API登录

>[!IMPORTANT]
>
>本节中介绍的过程仅适用于尚未载入Adobe Business Platform的组织。 如果您的组织已载入到Workfront Business Platform，则无法通过Workfront API登录Adobe。
>
>有关因贵组织是否已登记到Adobe业务平台而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

>[!NOTE]
>
>如果您组织的Workfront实例已启用Adobe IMS，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

第三方应用程序可以通过API与Workfront通信。 要提高Workfront站点的安全性，您可以通过将X.509证书上传到Workfront来将Workfront配置为限制API登录请求。 启用后，所有通过API的登录请求除了用户名和密码外，还必须包含客户端证书。

* [获取X.509证书](#obtain-the-x-509-certificate)
* [将证书上传到Workfront](#upload-the-certificate-to-workfront)
* [验证API登录调用是否受到限制](#verify-api-login-calls-are-restricted)

### 获取X.509证书 {#obtain-the-x-509-certificate}

从受信任的证书颁发机构（如Verisign）获取有效的X.509证书，并将其保存到工作站上的临时位置。

### 将证书上传到Workfront {#upload-the-certificate-to-workfront}

从证书颁发机构获得X.509证书后，需要将其上传到Workfront。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**设置**![齿轮设置图标](assets/gear-icon-settings.png)。

1. 展开&#x200B;**系统**，然后单击&#x200B;**客户信息**。

1. 在&#x200B;**API密钥设置**&#x200B;区域，选择&#x200B;**需要API登录的X.509证书**。
1. 单击&#x200B;**更改证书**。
1. 在工作站上，浏览并选择您之前下载的X.509证书。
1. （可选）单击证书名称旁边的&#x200B;**查看详细信息**&#x200B;以查看有关证书的以下详细信息：

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

### 验证API登录调用是否受到限制 {#verify-api-login-calls-are-restricted}

在将Workfront实例配置为需要X.509证书之前，请使用有效的用户名和密码参数对`/login`端点执行API请求。 您将收到一个包含sessionID的200响应。

在通过Workfront实例中的客户信息页面要求登录X.509证书后，再次尝试登录。 此时，您将收到500错误响应，并显示以下消息：“不受信任的请求。 请联系您的系统管理员并附加证书。”

确认需要X.509证书后，执行相同的登录请求，并将apiCertificate的附加参数设置为证书的值。 如果正确执行了此操作，您将收到包含有效sessionID的200响应。
