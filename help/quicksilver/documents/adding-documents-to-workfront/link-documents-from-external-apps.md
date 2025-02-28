---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 链接来自外部应用程序的文档
description: 您可以从外部源将文档和文件夹链接到Adobe Workfront。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '2620'
ht-degree: 0%

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
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox业务</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront 验证 </td> 
   <td>您可以使最初在Workfront Proof中创建的验证在Workfront中可用。 对于当前许可证，需要Pro Workfront计划或更高版本才能使用此功能。 对于新许可证，所有计划都包含此功能。 有关各种可用计划的详细信息，请参阅<a href="https://www.workfront.com/plans">Workfront计划</a>。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以从Experience Manager Assets Essentials将文档链接到Workfront。 有关详细信息，请参阅<a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref">适用于Experience Manager Assets Essentials的Adobe Workfront</a>。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>这需要进行额外购买。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他文档提供程序（通过自定义文档集成）</td> 
   <td> <p class="workfront_plans">对于当前许可证，需要Pro Workfront计划或更高版本才能使用此功能。 对于新许可证，所有计划都包含此功能。 有关各种可用计划的详细信息，请参阅<a href="https://www.workfront.com/plans">Workfront计划</a>。</p> </td>
  </tr> 
 </tbody> 
</table>

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如[配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

您可以验证和批准链接到外部云提供商的文档，就像验证直接上传到Workfront的文档一样。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td>
   <td> <p> 任何</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td>
   <td><p>新文档：参与者或更高版本</p>
    <p>或</p>
    <p>当前：请求或更高版本</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 文档存储

从外部应用程序链接到Workfront的文档会与外部云提供商存储，而不是存储在Workfront中。

以下情况例外：

* 如果由文档服务提供，则缩略图和预览图像可能会存储在Workfront服务器上。
* 在Workfront中使用验证时，文档将被复制并添加到验证服务器。

## 将文档从外部应用程序链接到Workfront

您可以将现有文档与外部云提供商链接。 这包括任何共享文档。

### 先决条件 {#prerequisites}

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如[配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md)中所述。

### 将外部文档链接到Workfront {#link-an-external-document-to-workfront}

您可以从外部应用程序(如Workfront和Google OneDrive)将文档链接到Microsoft。

>[!IMPORTANT]
>
>Dropbox根据文件路径存储文档。 因此，如果移动、重命名或删除了从Dropbox链接的文件，则该文件将在Workfront中变得不可访问。

1. 转到Workfront中您想要获取文档的&#x200B;**文档**&#x200B;区域。
1. 单击“新建”****，然后单击要将文档链接到Workfront的外部文档提供商。

   例如，要链接来自Dropbox的文档，请单击&#x200B;**来自Dropbox**。

   您已经授权的外部提供程序将显示在列表顶部。

1. （视情况而定）如果系统提示您登录外部服务，请在显示的框中键入该服务的登录凭据，然后单击&#x200B;**登录**。
1. （视情况而定）如果系统提示您授权外部应用程序，请单击&#x200B;**授权**&#x200B;按钮。

   您只需执行此操作一次。

1. 在出现的&#x200B;**链接外部文件和文件夹**&#x200B;框的搜索框中，键入要搜索的项目名称，然后按&#x200B;**Enter**&#x200B;查看来自外部应用程序的所有结果，而不管这些结果存储在哪个文件夹中。

   或

   浏览并选择要链接的文档。

   虽然您可以选择多个文档，但仅链接在当前视图中选择的文档。 例如，如果您选择文档，然后进入文件夹，则最初选择的文档不会链接。

1. （视情况而定）如果您是Workfront DAM客户，请单击&#x200B;**缩略图**&#x200B;图标以将文件显示为缩略图。

   >[!NOTE]
   >
   >从Workfront DAM链接文档时，Workfront DAM客户可以查看缩略图。 可能还会为Workfront DAM客户显示其他服务(如Dropbox和Box)的缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在从SharePoint或Google Drive链接文档时从不显示缩略图。

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
   >从Workfront DAM链接文档时，Workfront DAM客户可以查看缩略图。 可能还会为Workfront DAM客户显示其他服务(如Dropbox和Box)的缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在从SharePoint或Google Drive链接文档时从不显示缩略图。

1. 单击&#x200B;**链接**。

   在Workfront中，云提供商的图标显示在文档旁边，指示它们已链接到外部云提供商。

   >[!NOTE]
   >
   >对于链接到Box的文档，在刷新页面之前，不会显示Box中文档的链接。

有关将您从文件系统上传到Workfront的文档的新版本添加的信息，请参阅[将文档从文件系统添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)中的[将文档添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront)。

### 链接Workfront Proof文档 {#link-workfront-proof-documents}

您可以将验证链接到最初存在于Workfront Proof中的Workfront。 从Workfront Proof链接验证时，与验证关联的所有评论和其他元数据在Workfront中可用。

您只能链接那些您在Workfront Proof中拥有查看权限的校样。

1. 转到Workfront中您想要获取文档的&#x200B;**文档**&#x200B;区域。
1. 单击&#x200B;**新增**，然后单击Workfront Proof中的&#x200B;****。

   >[!NOTE]
   >
   >根据环境中配置的第三方提供商，此菜单中的选项可能有所不同。

1. 在出现的&#x200B;**从Workfront Proof链接校样**&#x200B;框中，开始键入要在Workfront中提供的校样名称。

   列表会在您键入内容时进行筛选。

1. 选择最多10个要链接的验证。

   任何灰显的验证名称均不可链接，因为验证已与Workfront中的文档相关联。

1. 单击&#x200B;**链接**。

   该验证的最新版本已链接到Workfront。 打开验证时，验证查看器中所有版本都可用。

### 在Workfront中创建Google文档 {#create-a-google-document-from-within-workfront}

您可以在Workfront中创建新的Google文档。 您不能在Workfront中为其他云提供商创建新文档。

1. 转到Workfront中您想要获取文档的&#x200B;**文档**&#x200B;区域。
1. 单击&#x200B;**新增** > **Google文件**，然后选择要创建的Google文档类型。
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
