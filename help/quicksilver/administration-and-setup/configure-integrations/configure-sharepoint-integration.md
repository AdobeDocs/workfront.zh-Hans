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
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
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

有关通过新链接文档的说明 [!DNL SharePoint] 集成，请参阅 [将外部文档链接到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 集成可以连接到单个 [!DNL SharePoint] 实例。 因此，用户可以为 [!DNL SharePoint]，但无法将集成设置为秒 [!DNL SharePoint]，即使他们有权访问和 [!DNL SharePoint].
>
>* 用户可以通过 [!DNL Workfront] [!DNL SharePoint] 集成 [!DNL SharePoint] 帐户。


## 配置旧版SharePoint集成，以便继续访问文档

要确保您的用户能够继续访问通过旧版SharePoint集成链接到Workfront的文档，您必须重新配置对旧版SharePoint集成的访问权限，并保持SharePoint客户端密钥为最新。

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



## 有关设置旧版SharePoint集成的说明

>[!IMPORTANT]
>
>此集成已弃用。 此处的说明仅供参考，将在不久的将来删除。


Workfront连接到 [!DNL SharePoint] 联机使用OAuth 2.0，这是大多数基于Web的集成用于用户身份验证和授权的标准。

要配置OAuth，您需要创建 [!DNL SharePoint] 网站和 [!DNL SharePoint]. 以下各节介绍了此过程。

有关OAuth的更多信息，请参阅 [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>以便于在 [!DNL Workfront] 和 [!DNL SharePoint] 在这些步骤中，我们建议保持这两个应用程序在单独的选项卡中打开。

* [创建和配置 [!DNL SharePoint] 网站](#create-and-configure-a-sharepoint-site)
* [向网站应用程序授予写入权限](#grant-write-permissions-to-the-site-app)
* [创建 [!DNL Workfront] [!DNL SharePoint] 集成实例](#create-a-workfront-sharepoint-integration-instance)
* [完成集成](#complete-your-integration)
* [添加文档](#add-documents)

### 创建和配置 [!DNL SharePoint] 网站  {#create-and-configure-a-sharepoint-site}

为 [!DNL Workfront] 验证 [!DNL SharePoint], [!DNL Workfront] 可以使用主控网站，其中用户 [!UICONTROL 完全控制] 权限级别或特定的“管理”权限。 此主控网站用作 [!DNL Workfront].

创建和配置 [!DNL SharePoint] 网站：

1. （可选）如果您不想使用组织的根站点，可以在 [!DNL SharePoint].

   有关说明，请访问 [创建网站](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) 在 [!DNL Microsoft] 文档。

   * 选择 **[!UICONTROL 团队网站]** 选项。

1. （视情况而定）如果您在步骤1中创建了网站，请转到刚刚创建的网站。

   或

   如果您未在步骤1中创建站点，请转到贵组织的根站点。

1. 添加 `/_layouts/15/appregnew.aspx` 到浏览器窗口顶部搜索栏中URL的结尾。
1. 配置以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客户端ID]</p> </td> 
      <td> <p>单击 <strong>[!UICONTROL Generate]</strong> 生成客户端ID。 将此ID复制到安全位置。 稍后当您设置 [!DNL SharePoint] 集成 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客户端密钥]</p> </td> 
      <td> <p>单击 <strong>[!UICONTROL Generate]</strong> 生成客户端密钥。 将此密钥复制到安全位置。 稍后当您设置 [!DNL SharePoint] 集成 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>标题</p> </td> 
      <td> <p>输入标题，例如 [!DNL Workfront] 网站应用程序。 用户在添加文档时会看到此标题。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL应用程序域]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL重定向URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建]**
1. 继续 [向网站应用程序授予写入权限](#grant-write-permissions-to-the-site-app).

### 向网站应用程序授予写入权限  {#grant-write-permissions-to-the-site-app}

此时，您已成功创建网站应用程序，并在中注册了该应用程序 [!DNL Workfront]. 此网站应用程序在 [!DNL SharePoint]. 它位于您的租户内。 新网站应用程序不会自动在租户中拥有对网站集的访问权限。 必须明确授予每个网站集的权限。 以下步骤将向您展示如何向新网站应用程序授予网站集的“写入”权限。 对您在 [!UICONTROL 可见网站集] 中，单击。

此网站应用程序必须 [!UICONTROL 写入] 用户需要通过访问的任何网站集的权限 [!DNL Workfront].

1. 将“/_layouts/15/appinv.aspx”添加到 [!DNL Sharepoint].

   **示例:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. 配置以下字段

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL应用程序ID]</td> 
      <td> <p>添加您在中创建的客户端ID <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">创建和配置 [!DNL SharePoint] 网站 </a>单击 <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL客户端] / [!UICONTROL应用程序域] / [!UICONTROL重定向URL]</p> </td> 
      <td> <p>当您单击[!UICONTROL Lookup]时，这些参数会自动填充。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL权限请求XML]</td> 
      <td> <p>将以下XML复制到[!UICONTROL Permission Request XML]字段。 确保按照所示完全添加该变量，而不会添加其他空格等。 以避免错误。</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. 单击&#x200B;**[!UICONTROL 创建]**。
1. 在出现的对话框中，单击 **[!UICONTROL 相信它]**.
1. 通过单击 **[!UICONTROL 网站集应用程序权限]** 链接 [!UICONTROL 网站设置].
1. 对其余网站集重复上述步骤，然后继续 [创建 [!DNL Workfront] [!DNL SharePoint] 集成实例](#create-a-workfront-sharepoint-integration-instance).

### 创建 [!DNL Workfront] [!DNL SharePoint] 集成实例 {#create-a-workfront-sharepoint-integration-instance}

在中创建网站应用程序后 [!DNL SharePoint]，您现在可以将信息从网站应用程序复制到 [!DNL Workfront]. 网站应用程序是应用程序主体，充当OAuth请求访问网站集内文档的渠道。

1. 登录 [!DNL Workfront] 作为管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL [!DNL SharePoint]集成]**.
1. 单击 **[!UICONTROL 添加[!DNL SharePoint]]**.
1. 配置以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL名称]</p> </td> 
      <td> <p>输入 [!DNL SharePoint] 集成。 用户在单击[!UICONTROL Add] &gt; [!UICONTROL From] '集成名称'时会看到此名称。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] 主机实例]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] 访问域]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>这是指用户将用于通过进行身份验证的主控网站。 它可能与[!UICONTROL的域相同 [!DNL SharePoint] 主机实例]。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>重要信息</b> 网站集仅在旧版中使用 [!DNL SharePoint] 集成。
       <ul> 
        <li> <p><b>如果您使用的是贵组织的根站点</b><b>:</b> </p> <p>输入 <code>/</code></p> </li> 
        <li> <p><b>如果您使用的是主控网站和子网站：</b> </p> <p><b>重要信息</b>: [!DNL Microsoft SharePoint] 不再建议使用子网站。</p> <p>在以上部分中输入您创建的网站集的URL主干。</p> <p>这是.com之后的URL的部分。</p> <p>示例：对于URL <code>https://mycompany.sharepoint.com/sites/mysite</code>，茎部 <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 客户端ID]</td> 
      <td>输入您在 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">创建和配置 [!DNL SharePoint] 网站 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] 客户端密钥]</td> 
      <td>输入您在 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">创建和配置 [!DNL SharePoint] 网站 </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL可见网站集]</td> 
      <td> <b>重要信息</b> 网站集仅在旧版中使用 [!DNL SharePoint] 集成。
       <ul> 
        <li> <p><b> 如果您使用的是贵组织的根站点</b><b>:</b> </p> <p>输入 <code>/</code></p> </li> 
        <li> <p><b>如果您使用的是主控网站和子网站：</b> </p> <p><b>重要信息</b>: [!DNL Microsoft SharePoint] 不再建议使用子网站。</p> <p>对于要添加到的每个子网站 [!DNL SharePoint] 集成，输入子站点的主体。</p> <p>示例：对于URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>，茎部 <code>/sites/mysite/mysubsite</code>.</p> <p><b>注释</b>:   <p>如果只想测试配置（无子网站），请输入主控网站的主体。 </p> <p>示例：对于URL <code> https://mycompany.sharepoint.com/sites/mysite</code>，茎部 <code>/sites/mysite</code>.</p> <p>当您已按照 <a href="#complete-your-integration" class="MCXref xref">完成集成</a>，则必须删除主控网站并输入子网站。</p> 
          <ol> 
           <li value="1">单击 <strong>[!UICONTROL主菜单]</strong> 图标 <img src="assets/main-menu-icon.png"> 的右上角 [!DNL Adobe Workfront]，然后单击 <strong>[!UICONTROL设置]</strong> <img src="assets/gear-icon-settings.png">.<li><p>在左侧面板中，单击 <strong>[!UICONTROL文档]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] 集成]</strong>.</p></li><li><p>单击 [!DNL SharePoint] 要设置的集成，然后单击编辑。</p></li><li><p>从[!UICONTROL Visible Site Collections]字段中删除主控站点的主体。</p></li><li><p>对于要添加到的每个子网站 [!DNL SharePoint] 集成，输入子站点的主体。</p></li><p>示例：对于URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>，茎部 <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 保存]**
1. 继续 [完成集成](#complete-your-integration).

### 完成集成 {#complete-your-integration}

基本配置即将完成。

1. 在Workfront中，单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 文档]** ![](assets/document-icon.png).
1. 单击 **[!UICONTROL 新增]**.
1. 单击 **[!UICONTROL 从]`<title of your [!DNL SharePoint] site>`** 中。

   此时会显示一个邀请您信任此网站的对话框。

   >[!NOTE]
   >
   >如果未显示此对话框，则 [!DNL SharePoint] 集成配置不正确。

1. 单击 **[!UICONTROL 相信它]**.

### 添加文档 {#add-documents}

您现在可以从 [!DNL SharePoint] 网站。

有关说明，请参阅 [将外部文档链接到 [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>如果链接文件夹的用户不再具有访问外部应用程序的权限， [!DNL Workfront] 无法再访问文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。 要确保继续访问，有权访问文件夹的用户必须重新链接该文件夹。

## 疑难解答

* [问题：使用 [!DNL SharePoint] 集成。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [问题：As a [!DNL Workfront] 用户，我无法配置新 [!DNL SharePoint] 实例。 当我尝试做时，我看到错误。](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [问题：尝试浏览时 [!DNL SharePoint] 文件 [!DNL Workfront]，则看不到任何或所有网站收藏集。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [问题：我无法访问 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 问题：使用 [!DNL SharePoint] 集成。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解决方案：

用户必须是具有相应权限的组的成员 [!DNL SharePoint] 网站。

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

### 问题：As a [!DNL Workfront] 用户，我无法配置新 [!DNL SharePoint] 实例。 当我尝试做时，我看到错误。 {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

解决方案：

这可能是由以下任一原因导致的 [!DNL Workfront] 或 [!DNL SharePoint]的配置。 确认：

* 在 [!DNL Workfront] [!DNL SharePoint] 集成实例和 [!DNL SharePoint] 网站应用程序。
* 用户具有 [!UICONTROL 完全控制] 访问用于身份验证的网站集的权限。
* 网站应用程序列在 [!UICONTROL 网站应用程序权限] 对于 [!UICONTROL 网站集] 用于身份验证。

### 问题：尝试浏览时 [!DNL SharePoint] 文件 [!DNL Workfront]，则看不到任何或所有网站收藏集。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解决方案：

要在 [!DNL Workfront]，则必须满足以下条件：

* 必须在 [!DNL Workfront] [!DNL SharePoint] 集成实例。

   要在 [!DNL Workfront]:

   1. 转到 [!UICONTROL 设置] > [!UICONTROL 文档] > [!UICONTROL [!DNL SharePoint] 集成].
   1. 编辑 [!DNL SharePoint] 集成实例信息。
   1. 验证网站集是否列在 [!UICONTROL 可见网站集].

* 用户必须有权查看 [!DNL SharePoint].
* 要在 [!DNL SharePoint]，转到 [!DNL SharePoint]，然后打开网站集> [!UICONTROL 设置] > [!UICONTROL 网站权限].
* 的 [!DNL SharePoint] 网站应用程序必须拥有网站集的访问权限。

   要在 [!DNL SharePoint]:

   1. 转到网站集> [!UICONTROL 设置] > [!UICONTROL 网站应用程序权限].
   1. 确保 [!UICONTROL 网站应用程序] 使用者 [!DNL Workfront] 列于此处。
   1. （视情况而定）如果网站应用程序未列出，请使用_layouts/15/appinv.aspx添加到网站集。

      有关添加网站集的信息，请参阅向网站应用程序授予写入权限。

### 问题：我无法访问 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解决方案：

如果链接了 [!DNL SharePoint] 文件夹无法再进行身份验证， [!DNL Workfront] 无法再访问文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。

要确保继续访问，有权访问文件夹的用户必须重新链接该文件夹。

有关从外部提供程序关联文件夹的信息，请参阅 [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 问题：尝试从添加文档时，我看到“404未找到”错误 [!DNL Sharepoint]

#### 解决方案：

如果在 [!UICONTROL 可见网站集] 列表已在Sharepoint中删除。 检查 [!UICONTROL 可见网站集] 列出，并删除已在Sharepoint中删除的所有站点。
