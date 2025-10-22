---
title: 配置 [!DNL SharePoint] 集成
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 您可以将 [!DNL Workfront] 与 [!DNL SharePoint] 联机集成，使用户能够在Workfront中导航、链接和添加 [!DNL SharePoint] 文档。 提供的功能与其他 [!DNL Workfront] 文档集成的功能相似。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1711'
ht-degree: 0%

---

# 配置[!DNL SharePoint]集成

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新的[!DNL SharePoint]集成已在22.3版本（2022年7月）中发布到生产环境。
>
>* 虽然您的用户仍然可以访问通过旧版[!DNL SharePoint]集成链接的文档，但他们无法通过该集成链接文档。 他们必须使用新的[!DNL SharePoint]集成来链接来自SharePoint的文档。
>
>* 如果您未配置旧版SharePoint集成，则无法添加该集成。 您必须使用新的SharePoint集成将文档链接到SharePoint。
>
>* 新的SharePoint集成可能不需要管理员进行配置，并且可以由个人用户进行设置。 但是，要确保顺利过渡到新的SharePoint集成，Workfront管理员必须在Workfront设置区域中进行一些细微的设置更改。
>
>    有关信息和说明，请参阅本文中的[配置旧版SharePoint集成以继续访问文档](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents)。
>    
>* 我们建议用户链接当前通过新集成通过旧版[!DNL SharePoint]集成链接的文档。
>    
>    有关链接文档的说明，请参阅[链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

您可以将[!DNL Workfront]与[!DNL SharePoint Online]集成，使用户能够在Workfront中导航到、链接和添加[!DNL SharePoint]文档。 提供的功能与其他[!DNL Workfront]集成（如[!DNL Google Drive]、[!DNL Box]和[!DNL Dropbox]）的功能类似。

此集成仅与[!DNL SharePoint Online]兼容。 不支持[!DNL SharePoint]的内部部署实例。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

您必须在[!DNL SharePoint]中拥有任何必要的访问权限才能修改或配置您的[!DNL SharePoint]集成。

## 通过新的SharePoint集成链接文档

个人用户可以通过新的[!DNL SharePoint]集成链接文档。 集成不需要管理员配置。 而是在链接文档时，用户登录到其[!DNL Microsoft]帐户，这样集成即可访问用户[!DNL SharePoint]中可用的文档。

当用户第一次将[!DNL Workfront] [!DNL SharePoint]集成连接到其[!DNL SharePoint]帐户时，他们将看到并同意[!DNL Workfront]在与其[!UICONTROL SharePoint]帐户交互时使用的所有权限，或者能够向其Microsoft管理员请求权限。 读取权限允许[!DNL Workfront]查看和访问[!DNL SharePoint]上的文件，写入权限允许用户将文件上载到[!DNL SharePoint]。

![Sharepoint权限](assets/sharepoint-permissions.png)

有关通过新的[!DNL SharePoint]集成链接文档的说明，请参阅[将外部文档链接到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* 根据组织的Microsoft配置，用户可能会看到“需要批准”页面而不是“请求的权限”页面。 在这种情况下，用户可以使用此页面请求组织的Microsoft管理员授予Sharepoint集成的权限。
>
>* [!DNL SharePoint]集成可以连接到单个[!DNL SharePoint]实例。 因此，用户可以设置一个[!DNL SharePoint]的集成，但无法设置与另一个[!DNL SharePoint]的集成，即使他们有权访问第二个[!DNL SharePoint]上的和文档也是如此。
>
>* 用户通过[!DNL Workfront] [!DNL SharePoint]集成访问与其[!DNL SharePoint]帐户中相同的站点、收藏集、文件夹、子文件夹和文件。

### 从SharePoint链接文档

有关通过新的[!DNL SharePoint]集成从SharePoint链接文档的说明，请参阅[将外部文档链接到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)。

### 将文档发送到SharePoint

要将文档发送到SharePoint，请执行以下操作：

1. 单击&#x200B;**发送至**&#x200B;图标![发送至](assets/send-to-icon.png)，然后选择SharePoint (Graph API)。
1. （可选）在搜索栏中搜索要发送文档的站点或文件夹。
1. 从列表中选择站点或文件夹。

   * 站点标有![站点图标](assets/site-icon.png)。

   * 文件夹标有![文件夹图标](assets/folder-icon.png)。

   * 文件未使用图标进行标记。

1. 单击&#x200B;**保存**。


## [!DNL SharePoint]集成的安全性、访问和授权信息

### 身份验证和授权

[!DNL Workfront]使用OAuth2检索访问令牌和刷新令牌。 此访问令牌用于所有[!DNL SharePoint]区域的授权。

### 访问和权限

当用户首次从[!DNL Workfront]向[!DNL SharePoint]添加文档时，他们将被定向到所请求的权限页面，他们可以在其中向其SharePoint集成授予权限。

>[!NOTE]
>
>根据组织的Microsoft配置，用户可能会看到“需要批准”页面而不是“请求的权限”页面。 在这种情况下，用户可以使用此页面请求组织的Microsoft管理员授予Sharepoint集成的权限。

请求以下权限：

| 访问 | 原因 |
|---|---|
| 拥有对文件的完全访问权限 | 允许[!DNL Workfront]访问用户的文件以链接资产。 当文档从[!DNL Workfront]发送到[!DNL SharePoint]时，[!DNL Workfront]需要访问权限才能创建资产。 |
| 读取所有网站集中的项目 | 允许[!DNL Workfront]读取资产以启用用户导航。 |
| 编辑或删除所有网站集中的项目 | 允许[!DNL Workfront]在站点和站点集合中创建资产。 仅在链接尝试失败后进行清理时使用“删除”。 |
| 维护对您已授予其访问权限的数据的访问权限 | 允许[!DNL Workfront]生成刷新令牌。 |
| 登录并读取用户配置文件 | 允许[!DNL Workfront]通过OAuth2登录流使用访问令牌代表用户操作。 |

* 此访问权限在用户首次使用集成时授予，并可随时撤销。
* 为此集成请求的权限是&#x200B;**已委派**&#x200B;权限。
* [!DNL Workfront]请求在集成中执行操作所需的最低访问权限。
* 查看、编辑或删除链接到[!DNL Adobe Workfront]的[!DNL SharePoint]文档的访问权限基于用户在[!DNL Workfront]中的访问权限。 但是，任何导航、下载或编辑[!DNL SharePoint]文件或文件夹都需要访问[!DNL SharePoint]，并且这些操作的访问权限由[!DNL SharePoint]控制。
* 用户可以查看源自[!DNL SharePoint]的缩略图和预览图像，并且无需登录[!DNL SharePoint]即可在[!DNL SharePoint]中查看文件和文件夹名称。
* 仅当用户处于脱机状态且另一个用户查看链接到[!DNL Workfront]的文件夹的内容时，才会使用用户的访问令牌。 访问令牌用于发现文件夹中的任何文档是否已添加、删除或编辑。

### 安全性

[!DNL Workfront]和[!DNL SharePoint]之间的所有通信均通过HTTPS进行，这将加密信息。

[!DNL Workfront]不存储、复制或复制[!DNL SharePoint]中的数据。 唯一的例外是[!DNL Workfront]存储来自[!DNL SharePoint]的缩略图，以便在列表视图和预览中显示。

如果资产首先上传到[!DNL Workfront]，然后发送到[!DNL SharePoint]，则[!DNL Workfront]将保留第一个文件的数据，因为用户可以下载[!DNL Workfront]文档的早期版本。 如果文档是在[!DNL SharePoint]中创建的，则[!DNL Workfront]不会存储该文件数据。

## 配置旧版[!DNL SharePoint]集成以继续访问文档

要确保您的用户能够继续访问通过旧版[!DNL SharePoint]集成链接到Workfront的文档，您必须重新配置对旧版[!DNL SharePoint]集成的访问权限，并使SharePoint客户端密钥保持最新。

* [重新配置对旧版 [!DNL SharePoint] 集成的访问权限](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [配置客户端密钥以继续访问旧版 [!DNL SharePoint] 集成](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### 重新配置对旧版[!DNL SharePoint]集成的访问权限

通过重新配置旧版[!DNL SharePoint]集成，您的用户可访问通过旧版[!DNL SharePoint]集成链接的文档，同时确保您的用户无法通过该集成链接新文档。

>[!NOTE]
>
> * 旧版[!DNL SharePoint]集成标记为“[!DNL SharePoint]”。
> * 新的[!DNL SharePoint]集成标记为“[!UICONTROL [!DNL SharePoint] (Graph API)]”。

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧导航中选择&#x200B;**[!UICONTROL 文档]**，然后选择&#x200B;**[!UICONTROL 云提供商]**。
1. 确保同时启用了&#x200B;**[!DNL SharePoint]**&#x200B;选项和&#x200B;**[!UICONTROL [!DNL SharePoint](Graph API)]**&#x200B;选项。
1. 单击&#x200B;**[!UICONTROL 保存]**。
1. 在左侧导航中选择&#x200B;**[!UICONTROL 文档]**，然后选择&#x200B;**[!UICONTROL [!DNL SharePoint]集成]**。
1. 选择列表左侧的复选标记以查看所有现有集成，然后选择&#x200B;**[!UICONTROL 禁用]**。



### 配置客户端密钥以继续访问旧版[!DNL SharePoint]集成

您的[!DNL SharePoint]客户端密钥每年过期一次。 为确保继续访问旧版[!DNL SharePoint]集成中的文档，您必须更新其[!DNL SharePoint]客户端密钥。

>[!IMPORTANT]
>
> 由于[!DNL SharePoint]客户端密钥由[!DNL Microsoft]处理，因此客户端密钥功能和过程可能会根据[!DNL SharePoint]对[!DNL Microsoft]所做的更新而更改。 请始终查看[!DNL Microsoft]文档，以了解[!DNL SharePoint]中有关过程和功能的最新信息。

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 按照[中的说明生成新的客户端密钥。替换 [!DNL SharePoint] 外接程序](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)中的过期客户端密钥。
1. 将此客户端密钥复制到安全位置。
1. 以管理员身份登录[!DNL Workfront]。
1. 在Workfront中，单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]** ![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧面板中，单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL [!DNL SharePoint]集成]**。
1. 单击要更新的[!DNL SharePoint]集成，然后单击&#x200B;**[!UICONTROL 编辑]**。
1. 找到编辑窗口的&#x200B;**连接信息**&#x200B;部分，然后在&#x200B;**[!UICONTROL SharePoint客户端密钥]**&#x200B;字段中输入新的客户端密钥。
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
1. Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

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

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![Document icon](assets/document-icon.png).
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

* [问题：用户在使用 [!DNL SharePoint] 集成时遇到基于身份验证的错误。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [问题：尝试浏览 [!DNL SharePoint] 中的 [!DNL Workfront]文件时，我看不到任何或所有网站集。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [问题：我无法访问 [!DNL SharePoint]中以前链接的文件夹和文档。](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 问题：用户在使用[!DNL SharePoint]集成时遇到基于身份验证的错误。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解决方案：

用户必须具有对[!DNL SharePoint]网站的适当权限。

具有[!UICONTROL 完全控制]访问权限的用户拥有您的[!DNL SharePoint]集成的所有必要权限。 如果不希望向用户授予完全控制访问权限，则必须授予以下权限：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL设计]</p> </td> 
   <td> <p>可以查看、添加、更新、删除、批准和自定义</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL编辑]</p> </td> 
   <td> <p>可以添加、编辑和删除列表；可以查看、添加、更新和删除列表项和文档</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Contribute]</p> </td> 
   <td> <p>可以查看、添加、更新和删除列表项和文档</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL仅视图]</p> </td> 
   <td> <p>可以查看页面、列表项和文档（具有服务器端文件处理程序的文档类型可以在浏览器中查看，但不能下载）</p> </td> 
  </tr> 
 </tbody> 
</table>

有关创建和编辑权限级别的说明，请参阅Microsoft文档中的[如何创建和编辑权限级别](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels)。

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### 问题：当尝试浏览[!DNL SharePoint]中的[!DNL Workfront]文件时，我看不到任何或所有网站集。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解决方案：

要在[!DNL Workfront]中查看网站集，必须满足以下条件：

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* 用户必须具有对[!DNL SharePoint]中网站集的查看权限。

  若要在[!DNL SharePoint]中对此进行验证，请在SharePoint中检查网站集的权限。

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### 问题：我无法访问[!DNL SharePoint]中以前链接的文件夹和文档。 {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解决方案：

如果链接[!DNL SharePoint]文件夹的用户无法再进行身份验证，[!DNL Workfront]将无法再访问该文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。

为确保继续访问，对该文件夹具有访问权限的用户必须重新链接该文件夹。

有关链接来自外部提供商的文件夹的信息，请参阅[链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
