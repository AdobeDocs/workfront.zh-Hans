---
title: 配置 [!DNL SharePoint] 集成
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 您可以集成 [!DNL Workfront] with [!DNL SharePoint] 在线，为用户提供导航、链接和添加的功能 [!DNL SharePoint] 文档。Workfront 提供的功能与其他功能类似 [!DNL Workfront] 集成，如Google Drive、Box和Dropbox。
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 8799c4e3a1e14c286b0a19e80e483370aea64bb8
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 0%

---

# 配置旧版 [!DNL SharePoint] 集成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新 [!DNL SharePoint] 22.3版本（2022年7月）中的集成已发布到生产环境。 尽管您的用户仍可以访问通过旧版链接的文档 [!DNL SharePoint] 集成中，用户必须使用 [!DNL SharePoint] 集成以链接来自SharePoint的文档。
>
>* 新的SharePoint集成不需要管理员进行配置，并且可由个人用户进行设置。 但是，为确保顺利过渡到新的SharePoint集成，Workfront管理员必须在Workfront设置区域中进行一些小的设置更改。
   >
   >    有关信息和说明，请参阅 [配置旧版SharePoint集成，以便继续访问文档](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 在本文中。
>    
>* 我们建议用户链接当前通过旧版链接的文档 [!DNL SharePoint] 集成。
   >    
   >    有关链接文档的说明，请参阅 [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


您可以集成 [!DNL Workfront] with [!DNL SharePoint Online]，为用户提供导航、链接和添加的功能 [!DNL SharePoint] 文档。Workfront 提供的功能与其他功能类似 [!DNL Workfront] 集成，例如 [!DNL Google Drive], [!DNL Box]和 [!DNL Dropbox].

此集成仅与 [!DNL SharePoint Online]. 的内部部署实例 [!DNL SharePoint] 不受支持。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

您必须在 [!DNL SharePoint] 修改或配置贵组织的 [!DNL SharePoint].

## 通过新的SharePoint集成链接文档

单个用户可以通过新 [!DNL SharePoint] 集成。 集成不需要管理员配置。 用户而是会登录到 [!DNL Microsoft] 帐户，这允许集成访问用户 [!DNL SharePoint].

用户首次连接 [!DNL Workfront] [!DNL SharePoint] 集成 [!DNL SharePoint] 帐户，他们将看到并同意 [!DNL Workfront] 与他们进行交互时使用 [!UICONTROL SharePoint] 帐户。 读取权限允许 [!DNL Workfront] 在 [!DNL SharePoint]、和写入权限允许用户将文件上传到 [!DNL SharePoint].

![Sharepoint权限](assets/sharepoint-permissions.png)

有关通过新链接文档的说明 [!DNL SharePoint] 集成，请参阅 [将外部文档链接到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 集成可以连接到单个 [!DNL SharePoint] 实例。 因此，用户可以为 [!DNL SharePoint]，但无法将集成设置为秒 [!DNL SharePoint]，即使他们有权访问和 [!DNL SharePoint].
>
>* 用户可以通过 [!DNL Workfront] [!DNL SharePoint] 集成 [!DNL SharePoint] 帐户。


## 安全、访问和授权信息 [!DNL SharePoint] 集成

### 身份验证和授权

[!DNL Workfront] 使用OAuth2检索访问令牌和刷新令牌。 此访问令牌用于对所有 [!DNL SharePoint] 区域。

### 访问和权限

用户首次将文档添加到 [!DNL Workfront] 从 [!DNL SharePoint]，则会被定向到请求以下权限的屏幕：

| 访问权限 | 原因 |
|---|---|
| 拥有对文件的完全访问权限 | 允许 [!DNL Workfront] 访问用户文件以链接资产时，请执行以下操作： 从发送文档时 [!DNL Workfront] to [!DNL SharePoint], [!DNL Workfront] 需要访问权限才能创建资产。 |
| 读取所有网站集中的项目 | 允许 [!DNL Workfront] 读取资产以启用用户导航。 |
| 编辑或删除所有网站集中的项目 | 允许 [!DNL Workfront] 在站点和站点集中创建资产。 仅在链接尝试失败后进行清理时，才使用删除。 |
| 维护您授予其访问权限的数据的访问权限 | 允许 [!DNL Workfront] 以生成刷新令牌。 |
| 登录并读取用户配置文件 | 允许 [!DNL Workfront] 要通过OAuth2登录流程，使用访问令牌代表用户执行操作。 |

此访问权限由用户在首次使用集成时授予，并且可以随时撤消。

请考虑以下与访问 [!DNL SharePoint] 到 [!DNL Workfront] [!DNL SharePoint] 集成：

* 为此集成请求的权限为 **委托** 权限。
* [!DNL Workfront] 请求执行集成中的操作所需的最低访问权限。
* 查看、编辑或删除 [!DNL Adobe Workfront] 链接到的文档 [!DNL SharePoint] 基于用户在 [!DNL Workfront]. 但是，对于 [!DNL SharePoint] 文件或文件夹需要访问 [!DNL SharePoint]，并且这些操作的访问权限由 [!DNL SharePoint].
* 用户可以查看缩略图并预览源自 [!DNL SharePoint]，并且可以在 [!DNL SharePoint]，而不登录 [!DNL SharePoint].
* 用户的访问令牌仅在用户处于脱机状态且其他用户查看链接到的文件夹的内容时使用 [!DNL Workfront]. 访问令牌用于发现文件夹中是否有文档已添加、删除或编辑。

### 安全性

之间的所有通信 [!DNL Workfront] 和 [!DNL SharePoint] 通过HTTPS进行，以加密信息。

[!DNL Workfront] 不存储、复制或复制 [!DNL SharePoint]. 唯一的例外是 [!DNL Workfront] 存储缩略图 [!DNL SharePoint] 以在列表视图和预览中显示。

如果资产首次上传到 [!DNL Workfront]，然后发送到 [!DNL SharePoint], [!DNL Workfront] 保留第一个文件的数据，因为用户可以下载 [!DNL Workfront] 文档。 如果文档是在 [!DNL SharePoint], [!DNL Workfront] 不存储该文件数据。

## 配置旧版 [!DNL SharePoint] 集成以继续访问文档

确保用户能够继续访问通过旧版链接到Workfront的文档 [!DNL SharePoint] 集成中，您必须重新配置对旧版的访问权限 [!DNL SharePoint] 集成并保持SharePoint客户端密钥为最新。

* [重新配置对旧版的访问权限 [!DNL SharePoint] 集成](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [配置客户端密钥以继续访问旧版 [!DNL SharePoint] 集成](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### 重新配置对旧版的访问权限 [!DNL SharePoint] 集成

确保您可以访问通过旧版链接的文档 [!DNL SharePoint] 集成，同时确保用户无法通过该集成链接新文档，请完成以下过程。

>[!NOTE]
>
> * 旧版 [!DNL SharePoint] 集成标记为“[!DNL SharePoint].&quot;
> * 新 [!DNL SharePoint] 集成标记为“[!UICONTROL [!DNL SharePoint] （图形API）].&quot;


1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 设置]** ![设置](../get-started-wf-administration/assets/gear-icon-settings.png).
1. 选择 **[!UICONTROL 文档]** 在左侧导航中，选择 **[!UICONTROL 云提供商]**.
1. 确保 **[!DNL SharePoint]** 选项和 **[!UICONTROL [!DNL SharePoint]（图形API）]** 选项均已启用。
1. 单击&#x200B;**[!UICONTROL 保存]**。
1. 选择 **[!UICONTROL 文档]** 在左侧导航中，选择 **[!UICONTROL [!DNL SharePoint]集成]**.
1. 选择列表左侧的复选标记以用于所有现有集成，然后选择 **[!UICONTROL 禁用]**.


### 配置客户端密钥以继续访问旧版 [!DNL SharePoint] 集成

您的 [!DNL SharePoint] 客户端密钥每年过期一次。 确保继续访问旧版中的文档 [!DNL SharePoint] 集成时，必须保留 [!DNL SharePoint] 客户端密钥。

>[!IMPORTANT]
>
> 因为 [!DNL SharePoint] 客户端密钥由 [!DNL Microsoft]，客户端密钥功能和过程可能会根据 [!DNL SharePoint] 由 [!DNL Microsoft]. 始终检查 [!DNL Microsoft] 有关 [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 生成新的客户端密钥，如 [替换 [!DNL SharePoint] 插件](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. 将此客户端密钥复制到安全位置。
1. 登录 [!DNL Workfront] 作为管理员。
1. 在Workfront中，单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL [!DNL SharePoint]集成]**.
1. 单击 [!DNL SharePoint] 要更新的集成，然后单击 **[!UICONTROL 编辑]**.
1. 在 **[!UICONTROL 客户端密钥]** 字段。
1. 单击&#x200B;**[!UICONTROL 保存]**。

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## 故障排除

* [问题：使用 [!DNL SharePoint] 集成。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [问题：尝试浏览时 [!DNL SharePoint] 文件 [!DNL Workfront]，则看不到任何或所有网站收藏集。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [问题：我无法访问 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 问题：使用 [!DNL SharePoint] 集成。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解决方案：

用户必须拥有 [!DNL SharePoint] 网站。

具有 [!UICONTROL 完全控制] 拥有您的 [!DNL SharePoint] 集成。 如果您不想向用户授予完全控制访问权限，则必须授予以下权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>可以查看、添加、更新、删除、批准和自定义</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL编辑]</p> </td> 
   <td> <p>可以添加、编辑和删除列表；可以查看、添加、更新和删除列表项和文档</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>可以查看、添加、更新和删除列表项和文档</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！仅UICONTROL视图]</p> </td> 
   <td> <p>可以查看页面、列表项和文档（具有服务器端文件处理程序的文档类型可以在浏览器中查看，但不能下载）</p> </td> 
  </tr> 
 </tbody> 
</table>

有关创建和编辑权限级别的说明，请参阅 [如何创建和编辑权限级别](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) (在Microsoft文档中)。

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 问题：尝试浏览时 [!DNL SharePoint] 文件 [!DNL Workfront]，则看不到任何或所有网站收藏集。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解决方案：

要在 [!DNL Workfront]，则必须满足以下条件：

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 用户必须有权查看 [!DNL SharePoint].

   要在 [!DNL SharePoint]，转到 [!DNL SharePoint]，然后打开网站集> [!UICONTROL 设置] > [!UICONTROL 网站权限].
<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 问题：我无法访问 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解决方案：

如果链接了 [!DNL SharePoint] 文件夹无法再进行身份验证， [!DNL Workfront] 无法再访问文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。

要确保继续访问，有权访问文件夹的用户必须重新链接该文件夹。

有关从外部提供程序关联文件夹的信息，请参阅 [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->