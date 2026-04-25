---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 链接来自外部应用程序的文档
description: 您可以从外部源将文档和文件夹链接到Adobe Workfront。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '2592'
ht-degree: 1%

---

# 链接来自外部应用程序的文档

<!-- Audited: 01/2024 -->

您可以从以下来源将文档和文件夹链接到Adobe Workfront：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">现有的第三方云文档提供商</td> 
   <td>这些功能包括： 
    <ul> 
     <li>盒子</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 校样 </td> 
   <td>您可以使最初在Workfront Proof中创建的验证在Workfront中可用。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以从Experience Manager Assets Essentials将文档链接到Workfront。 有关详细信息，请参阅<a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref">适用于Experience Manager Assets Essentials的Adobe Workfront</a>。</td> 
  </tr>

<tr> 
   <td role="rowheader">其他文档提供程序（通过自定义文档集成）</td> 
   <td> <p class="workfront_plans">这些集成可以在“设置”区域中配置。</p> </td>
  </tr> 
 </tbody> 
</table>

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如[配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

您可以验证和批准链接到外部云提供商的文档，就像验证直接上传到Workfront的文档一样。

>[!NOTE]
>
>新文档区域不提供此功能。<br>
>如果您的组织使用企业存储，则当您访问Workfront中的文档时，将会看到“新建文档”区域。 有关企业存储的更多信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td>
   <td> <p>“任一”</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td>
   <td><p>参与者或更高版本</p>
    <p>请求或更高版本</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 文档存储

从外部应用程序链接到Workfront的文档会与外部云提供商存储，而不是存储在Workfront中。

The following exceptions apply:

* When provided by the document service, thumbnails and preview images might be stored on Workfront servers.
* When you use proofing in Workfront, the document is copied and added to the proofing servers.

## File size limits

Third-party cloud providers:

* Single file: 5 GB or less
* Multiple file: 1 GB or less (total of all files)

## Link a document from an external application to Workfront

You can link existing documents with an external cloud provider. This includes any shared documents.

### 先决条件 {#prerequisites}

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如[配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

### Link an external document to Workfront {#link-an-external-document-to-workfront}

You can link documents to Workfront from an external application such as Google and Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox stores documents based on the file path. Because of this, if a file linked from Dropbox is moved, renamed, or deleted, it becomes inaccessible in Workfront.

1. Go to the **Documents** area in Workfront where you want the document.
1. Click **Add New**, then click the external document provider where you want to link documents to Workfront.

   For example, to link documents from Dropbox, click **From Dropbox**.

   External providers that you have already authorized appear at the top of the list.

1. (Conditional) If you are prompted to log into the external service, type your login credentials for the service in the box that appears, then click **Sign in**.
1. (Conditional) If you are prompted to authorize the external application, click the **Authorize** button.

   You need to do this only once.

1. In the search box of the **Link External Files and Folders** box that appears, type the name of the item you want to search for, then press **Enter** to see all results from the external application, regardless of which folder they are storied in.

   或

   Browse to and select the documents you want to link.

   Though you can select multiple documents, only documents that are selected in the current view are linked. 例如，如果您选择文档，然后进入文件夹，则最初选择的文档不会链接。

1. （视情况而定）如果您是Workfront DAM客户，请单击&#x200B;**缩略图**&#x200B;图标以将文件显示为缩略图。

   >[!NOTE]
   >
   >从Workfront DAM链接文档时，Workfront DAM客户可以查看缩略图。 可能还会为Workfront DAM客户显示其他服务（如Dropbox和Box）的缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在从SharePoint或Google Drive链接文档时从不显示缩略图。

1. 单击&#x200B;**链接**。

   在Workfront中，云提供商的图标显示在文档旁边。

   >[!NOTE]
   >
   >* 如果用于链接文档的下载URL超过2,048个字符，则文件无法链接。
   >* 对于链接到Box的文档，在刷新页面之前，不会显示Box中文档的链接。

### 添加链接文档的新版本 {#add-a-new-version-of-a-linked-document}

您可以添加从外部应用程序链接到Workfront的文档的新版本。

1. 转到链接文档的&#x200B;**文档**&#x200B;区域，然后选择链接的文档。

   >[!IMPORTANT]
   >
   >文档必须在链接的文件夹之外，才能创建新版本。

1. 单击&#x200B;**新增** > **版本**，然后单击外部文档提供程序。

   例如，要从Dropbox链接文档的新版本，请单击&#x200B;**从Dropbox**。

   您已经授权的外部提供程序将显示在列表顶部。

1. （视情况而定）如果系统提示您登录外部服务，请在显示的框中键入该服务的登录凭据，然后单击&#x200B;**登录**。
1. （视情况而定）如果系统提示您授权外部应用程序，请单击&#x200B;**授权**。

   您只需执行此操作一次。

1. 在出现的&#x200B;**链接外部文件和文件夹**&#x200B;框的搜索框中，键入要搜索的项目名称，然后按&#x200B;**Enter**&#x200B;查看来自外部应用程序的所有结果，无论这些结果存储在哪个文件夹中。

   或

   浏览并选择要链接的文档。

   您可以选择多个文档；但是，只链接在当前视图中选择的文档。 例如，如果您选择文档，然后进入文件夹，则最初选择的文档不会链接。

1. （视情况而定）如果您是Workfront DAM客户，请单击&#x200B;**缩略图**&#x200B;图标以将文件显示为缩略图。

   >[!NOTE]
   >
   >从Workfront DAM链接文档时，Workfront DAM客户可以查看缩略图。 可能还会为Workfront DAM客户显示其他服务（如Dropbox和Box）的缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在从SharePoint或Google Drive链接文档时从不显示缩略图。

1. 单击&#x200B;**链接**。

   In Workfront, the cloud provider&#39;s icon appears next to the documents, indicating that they are linked to the external cloud provider.

   >[!NOTE]
   >
   >对于链接到Box的文档，在刷新页面之前，不会显示Box中文档的链接。

For information about adding new version of a document you have uploaded to Workfront from your file system, see [Add documents to Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) in [Add documents to Adobe Workfront from your file system](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Link Workfront Proof documents {#link-workfront-proof-documents}

You can link proofs to Workfront that originally existed in Workfront Proof. When you link a proof from Workfront Proof, all comments and other metadata associated with the proof are available in Workfront.

You can link only those proofs for which you have View access in Workfront Proof.

1. Go to the **Documents** area in Workfront where you want the document.
1. Click **Add New**, then click **From Workfront Proof**.

   >[!NOTE]
   >
   >The options in this menu may vary depending on what third party providers are configured in your environment.

1. In the **Link proofs from Workfront Proof** box that appears, begin typing the name of the proof you want to make available in Workfront.

   The list is filtered as you type.

1. Select up to 10 proofs to link.

   Any proof name that is dimmed is not available to link, because the proof is already associated with a document in Workfront.

1. 单击&#x200B;**链接**。

   The most current version of the proof is linked to Workfront. When you open the proof, all versions are available in the proofing viewer.

### Create a Google document from within Workfront {#create-a-google-document-from-within-workfront}

You can create a new Google document from within Workfront. You cannot create new documents from within Workfront for other cloud providers.

1. Go to the **Documents** area in Workfront where you want the document.
1. Click **Add New** > **Google File**, then select the type of Google document you want to create.
1. 如果出现&#x200B;**添加Google驱动器帐户**&#x200B;框，请单击&#x200B;**授权Google驱动器**。

   Google文档已添加到&#x200B;**文档**&#x200B;选项卡。

   >[!NOTE]
   >
   > “我的驱动器”和“与我共享”显示两个不同的结果。 如果您在“我的驱动器”中找不到文件，请签入“与我共享”文件夹。

## 将文档从Workfront上传并链接到外部云提供商

您可以上传文档，并将其从Workfront链接到外部云提供商。 这会将文档的存储空间从Workfront移动到外部云提供商。 当文档在外部应用程序中更改时，会自动在Workfront中更新。

>[!NOTE]
>
>将资产发送到外部文档提供商会创建资产的新版本。

没有Workfront访问权限的用户可以在外部应用程序中查看文档（如果他们有权访问应用程序）。

1. 选择在Workfront中上传的文档。
1. 单击&#x200B;**更多** >**发送至**，然后选择要存储链接文档的云提供商。

   您还可以使用“文档详细信息”页面上的“更多”菜单![“更多”菜单](assets/more-icon.png)来执行此操作。

1. 在提供程序的应用程序中选择要存储文档的文件夹。

   这可以是提供商应用程序中的任何文件夹，包括共享文件夹。

1. 单击&#x200B;**保存**。

   外部提供商的徽标显示在文档名称旁边，表示该文档现在链接到Workfront并由外部云提供商存储。

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## 链接文件夹

在Workfront和外部云提供商之间链接文件夹时，将链接该文件夹及其所有内容。 如果没有Workfront访问权限的用户从外部文档应用程序添加、删除和修改文件，则其更改将同步到Workfront。

### 文件夹访问权限 {#folder-access-rights}

从外部文档应用程序同步文件夹内容时，Workfront使用最初链接该文件夹的用户的凭据。 这会产生以下用户体验：

* 如果用户无权查看外部应用程序中的文件和文件夹，但有权通过Workfront查看链接的文件夹，则他们只能查看Workfront中的文件和文件夹的名称，而非其内容。
* 当有人访问Workfront中由其他用户链接到Workfront的链接文件夹（例如链接文件夹中的子文件夹）中的内容时，内容使用最初链接该文件夹的用户的Workfront登录凭据同步到Workfront，而不是使用访问内容的用户的凭据同步到。

>[!IMPORTANT]
>
>* 如果从Workfront系统中删除了最初链接文件夹的用户，则用户将无法再通过Workfront访问链接文件夹上的内容。 在这种情况下，文件夹必须由对外部应用程序中的文件夹具有权限的活动Workfront用户重新链接。
>* 如果链接文件夹的用户不再具有访问外部应用程序的权限，Workfront则无法再访问文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。 为确保继续访问，对该文件夹具有访问权限的用户必须重新链接该文件夹。

### 链接一个或多个外部文件夹 {#link-one-or-more-external-folders}

1. 转到Workfront中您希望文件夹所在的区域，然后单击左侧面板中的&#x200B;**文档** ![文档图标](assets/document-icon.png)。

1. 单击“新建”****，然后单击要将文件夹链接到Workfront的外部文档提供商。
1. （视情况而定）如果尚未授权外部服务，请为外部提供程序指定登录凭据，然后单击&#x200B;**登录**。

   您已经授权的外部提供程序将显示在列表顶部。

1. 在出现的&#x200B;**链接外部文件和文件夹**&#x200B;框中，浏览并选择要链接的文件夹。

   或

   键入要搜索的文件夹的名称，然后按&#x200B;**Enter**。

   您可以选择多个文件夹；但是，只链接在当前视图中选择的文件夹。 例如，如果您选择文件夹，然后进入文件夹，则不会链接您最初选择的文件夹。

   >[!NOTE]
   >
   >从Google驱动器链接文件夹时，只能链接位于个人驱动器（我的驱动器）和团队驱动器中的文件夹。 您无法从“与我共享”区域链接文件夹。

1. 单击&#x200B;**链接**。

   在Workfront中，云提供商的徽标显示在文件夹旁边，表示该文件夹已链接到外部云提供商。

1. （可选）要重命名文件夹，以使Workfront中的文件夹名称不同于外部文档应用程序中的文件夹名称，请在&#x200B;**文件夹**&#x200B;分区中选择文件夹，单击文件夹名称旁边显示的“更多”菜单![更多菜单](assets/more-icon.png)，然后单击&#x200B;**重命名**。

   ![重命名文件夹](assets/documents-folderlink-rename-nwe-350x154.png)

这不会重命名外部应用程序中的文件夹。

### 将子文件夹添加到链接的文件夹  {#add-subfolders-to-a-linked-folder}

您可以在现有的链接文件夹中创建新文件夹。 您还可以将另一个文件夹拖到现有的链接文件夹中。

1. 要在现有的链接文件夹中创建新文件夹，请转到现有文件夹，然后按照[创建文档文件夹](../../documents/organizing-documents/create-documents-folder.md)中的说明创建新文件夹。

   或

   要将现有文件夹拖到现有的链接文件夹中，请转到要放置子文件夹的“文档”区域，然后将其拖到链接文件夹中。

   ![拖到链接的文件夹中](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >将现有Workfront文件夹拖到链接文件夹中时，适用以下限制：
   >
   >* 您正在拖动的文件夹不能已链接，也不能包含任何已链接的内容。
   >* 要拖动的文件夹（包括其内容）不能超过50 MB。

## 将文档添加到链接的文件夹

通过Workfront将文档添加到链接文件夹时，会自动添加为链接文档。

1. 选择要在其中插入文档的链接文件夹，单击&#x200B;**新增>文档**，然后浏览到文档并将其添加到文件夹中。

   或

   在您想要该文档的&#x200B;**文档**&#x200B;区域中，将该文档拖到链接的文件夹中。

   文档的新版本会自动在外部应用程序中创建，并链接到Workfront。

>[!NOTE]
>
> * 文档正在移动时，文档选项不可用。
>
> * 将文档移至Experience Manager Assets后，在Workfront的文档列表中不再可见。
>
> * 您在文档移动时对文档所做的任何操作或编辑都不会显示在Experience Manager Assets的文档中，因此将丢失。

## 删除链接的文档或文件夹

从外部应用程序中删除链接的文档或文件夹时，该文档或文件夹将保留在Workfront系统中，直到您也从Workfront中删除它为止。

1. 选择链接的文档或文件夹，然后单击&#x200B;**删除**。
1. 在出现的确认框中，单击&#x200B;**是，取消链接**。

   该文档将从Workfront网站取消链接。 它在外部应用程序中不受影响。

## 关于重命名链接的文档和文件夹

重命名链接的文档或文件夹时，更改仅在创建它的应用程序中可见。 例如，如果在Workfront中重命名链接文档，则新名称仅在Workfront中可见。

如果您希望名称在Workfront和外部应用程序中匹配，则必须在两个位置都重命名它。

>[!IMPORTANT]
>
>请勿在Workfront中重命名链接到Dropbox的文档；这样做会导致Workfront中的文件无法访问。 请改为在Dropbox中重命名文件，然后重新同步该文件。
