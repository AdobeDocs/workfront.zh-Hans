---
product-area: documents
navigation-topic: add-documents-to-workfront
title: 从外部应用程序链接文档
description: 您可以从以下源将文档和文件夹链接到Adobe Workfront — 编辑我。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: 0ecee45183f5bc77a1c4a489013e486d8c26094c
workflow-type: tm+mt
source-wordcount: '2586'
ht-degree: 0%

---

# 从外部应用程序链接文档

您可以从以下源将文档和文件夹链接到Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">现有第三方云文档提供程序</td> 
   <td>这些功能包括： 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox业务</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>MicrosoftSharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>您可以在Workfront中提供最初在Workfront校样中创建的校样。 使用此功能需要专业Workfront计划或更高版本。 有关各种可用计划的更多信息，请参阅 <a href="https://www.workfront.com/plans">Workfront计划</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>您可以从Experience Manager Assets Essentials将文档链接到Workfront。 有关更多信息，请参阅 <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>这需要额外购买。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他文档提供程序（通过自定义文档集成）</td> 
   <td> <p class="workfront_plans">使用此功能需要专业Workfront计划或更高版本。 有关各种可用计划的更多信息，请参阅 <a href="https://www.workfront.com/plans">Workfront计划</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如 [配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

您可以采用与直接上传到Workfront的文档相同的方式，校样和批准链接到外部云提供商的文档。 

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 文档存储

从外部应用程序链接到Workfront的文档将与外部云提供商一起存储，而不是在Workfront内存储。

以下例外适用：

* 当文档服务提供时，缩略图和预览图像可能会存储在Workfront服务器上。
* 在Workfront中使用校对时，文档会被复制并添加到校对服务器中。 

## 将文档从外部应用程序链接到Workfront

您可以将现有文档与外部云提供商进行链接。 这包括所有共享文档。

* [先决条件](#prerequisites)
* [将外部文档链接到Workfront](#link-an-external-document-to-workfront)
* [添加链接文档的新版本](#add-a-new-version-of-a-linked-document)
* [链接Workfront校样文档](#link-workfront-proof-documents)
* [在Workfront中创建Google文档](#create-a-google-document-from-within-workfront)

### 先决条件 {#prerequisites}

在链接文档或文件夹之前，Workfront管理员必须为每个文档提供商或自定义文档集成启用此功能，如 [配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### 将外部文档链接到Workfront {#link-an-external-document-to-workfront}

您可以从外部应用程序(如Google和Microsoft OneDrive)将文档链接到Workfront。

>[!IMPORTANT]
>
>Dropbox基于文件路径存储文档。 因此，如果移动、重命名或删除了从Dropbox链接的文件，则在Workfront中将无法访问该文件。

1. 转到 **文档** 区域(在Workfront中您需要文档的位置)。
1. 单击 **新增**，然后单击要将文档链接到的外部文档提供程序。Workfront

   例如，要链接Dropbox中的文档，请单击 **从Dropbox**.

   您已授权的外部提供程序将显示在列表顶部。

1. （视情况而定）如果系统提示您登录外部服务，请在显示的框中键入该服务的登录凭据，然后单击 **登录**.
1. （视情况而定）如果系统提示您授权外部应用程序，请单击 **授权** 按钮。

   您只需执行一次此操作。

1. 在 **链接外部文件和文件夹** 框中，键入要搜索的项目名称，然后按 **输入** 查看外部应用程序的所有结果，而不考虑它们存储在哪个文件夹中。

   或

   浏览并选择要链接的文档。

   虽然您可以选择多个文档，但只有在当前视图中选择的文档才会链接。 例如，如果您选择一个文档，然后进入文件夹，则最初选择的文档不会链接。

1. （视情况而定）如果您是Workfront DAM客户，请单击 **缩略图** 图标来将文件显示为缩略图。

   >[!NOTE]
   Workfront DAM客户在从Workfront DAM关联文档时可以查看缩略图。 对于其他服务(如Dropbox和框)，还可以为Workfront DAM客户显示缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在关联来自SharePoint或Google Drive的文档时，永远不会显示缩略图。

1. 单击 **链接**.

   在Workfront中，文档旁边会显示云提供商的图标。

   >[!NOTE]
   对于链接到Box的文档，在刷新页面之前，不会显示指向Box中文档的链接。

### 添加链接文档的新版本 {#add-a-new-version-of-a-linked-document}

您可以从外部应用程序添加链接到Workfront的文档的新版本。

1. 转到 **文档** 链接文档的区域，然后选择链接的文档。

   >[!IMPORTANT]
   文档必须位于链接文件夹之外才能创建新版本。

1. 单击 **新增** > **版本**，然后单击外部文档提供程序。

   例如，要从Dropbox链接新版本的文档，请单击 **从Dropbox**.

   您已授权的外部提供程序将显示在列表顶部。

1. （视情况而定）如果系统提示您登录外部服务，请在显示的框中键入该服务的登录凭据，然后单击 **登录**.
1. （视情况而定）如果系统提示您授权外部应用程序，请单击 **授权**.

   您只需执行一次此操作。

1. 在 **链接外部文件和文件夹** 框中，键入要搜索的项目名称，然后按 **输入** 查看外部应用程序的所有结果，而不考虑它们存储在哪个文件夹中。

   或

   浏览并选择要链接的文档。

   您可以选择多个文档；但是，只有在当前视图中选择的文档才会被链接。 例如，如果您选择一个文档，然后进入文件夹，则最初选择的文档不会链接。

1. （视情况而定）如果您是Workfront DAM客户，请单击 **缩略图** 图标来将文件显示为缩略图。

   >[!NOTE]
   Workfront DAM客户在从Workfront DAM关联文档时可以查看缩略图。 对于其他服务(如Dropbox和框)，还可以为Workfront DAM客户显示缩略图。 但是，不支持在Workfront中查看Workfront DAM以外的服务的缩略图，并且在关联来自SharePoint或Google Drive的文档时，永远不会显示缩略图。

1. 单击 **链接**.

   在Workfront中，文档旁边会显示云提供程序的图标，指示它们已链接到外部云提供程序。

   >[!NOTE]
   对于链接到Box的文档，在刷新页面之前，不会显示指向Box中文档的链接。

有关添加从文件系统上传到Workfront的文档新版本的信息，请参阅 [从文件系统将文档添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#adding-new-versions-of-documents) in [从文件系统将文档添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### 链接Workfront校样文档 {#link-workfront-proof-documents}

您可以将校样链接到Workfront Proof中最初存在的校样。 在链接Workfront校样中的校样时，与校样关联的所有注释和其他元数据都可在Workfront中使用。 

您只能链接那些在Workfront校样中具有“查看”访问权限的校样。

1. 转到 **文档** 区域(在Workfront中您需要文档的位置)。
1. 单击 **新增**，然后单击 **从Workfront校样**.

   >[!NOTE]
   此菜单中的选项可能会因您环境中配置的第三方提供商而异。

1. 在 **链接** 校样 **从** Workfront校样框，开始键入要在Workfront中提供的校样的名称。

   该列表会在您键入时进行过滤。

1. 选择最多10个要链接的校样。

   由于校样已与Workfront中的文档关联，因此无法链接任何灰显的校样名称。

1. 单击 **链接**.

   校样的最新版本已链接到Workfront。 打开校样时，校样查看器中提供了所有版本。

### 在Workfront中创建Google文档 {#create-a-google-document-from-within-workfront}

您可以在Workfront中创建新的Google文档。 您无法在Workfront内为其他云提供商创建新文档。

1. 转到 **文档** 区域(在Workfront中您需要文档的位置)。
1. 单击 **新增** > **Google文件**，然后选择要创建的Google文档类型。

1. 选择要创建的Google文档类型。
1. 如果 **添加Google驱动器帐户** 框，单击 **授权Google Drive**.

   将Google文档添加到 **文档** 选项卡。

   >[!NOTE]
    “My Drive and Shared with Me（我的驱动器和共享）”显示两个不同的结果。 如果无法在“My Drive（我的驱动器）”中找到文件，请检查“Shared with Me（与我共享）”文件夹。

## 将文档从Workfront更新并链接到外部云提供程序

您可以将文档从Workfront上传并链接到外部云提供商。 这会将文档的存储从Workfront移动到外部云提供程序。 在外部应用程序中更改文档时，该文档会在Workfront中自动更新。

没有Workfront访问权限的用户如果有权访问该应用程序，则可以在外部应用程序中查看该文档。

1. 选择在Workfront中上传的文档。
1. 单击 **更多** >**发送到**，然后选择要存储链接文档的云提供程序。

   您还可以使用“更多”菜单 ![](assets/more-icon.png) 在“文档详细信息”页面上执行此操作。

1. 在提供商的应用程序中选择要存储文档的文件夹。

   该文件夹可以是提供程序应用程序中的任意文件夹，包括共享文件夹。

1. 单击&#x200B;**保存**。

   外部提供商的徽标显示在文档名称旁边，以指示文档现已链接到Workfront并由外部云提供商存储。

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## 链接文件夹

在Workfront和外部云提供程序之间链接文件夹时，会关联该文件夹及其所有内容。 如果没有Workfront访问权限的用户从外部文档应用程序中添加、删除和修改文件，则其更改将同步到Workfront。 以下部分介绍了如何链接文件夹和子文件夹：

* [文件夹访问权限](#folder-access-rights)
* [链接一个或多个外部文件夹](#link-one-or-more-external-folders)
* [将子文件夹添加到链接的文件夹](#add-subfolders-to-a-linked-folder)

### 文件夹访问权限 {#folder-access-rights}

从外部文档应用程序同步文件夹内容时，Workfront会使用最初链接该文件夹的用户的凭据。 这会产生以下用户体验：

* 如果用户无权查看外部应用程序中的文件和文件夹，但有权通过Workfront查看链接的文件夹，则他们只能查看Workfront中的文件和文件夹的名称，而不能查看其内容。
* 当某人访问另一用户链接到Workfront的Workfront链接文件夹（例如链接文件夹中的子文件夹）中的内容时，该内容会使用最初链接该文件夹的用户的Workfront登录凭据（而不是访问内容的用户的凭据）同步到Workfront。

>[!IMPORTANT]
* 如果最初链接文件夹的用户从Workfront系统中删除，则用户将无法再通过Workfront访问链接文件夹上的内容。 在这种情况下，必须由对外部应用程序中的文件夹拥有权限的活动Workfront用户重新链接文件夹。
* 如果链接文件夹的用户不再具有访问外部应用程序的权限，则Workfront将无法再访问文件夹的内容。 例如，如果最初链接文件夹的用户离开公司，则可能会发生这种情况。 要确保继续访问，有权访问文件夹的用户必须重新链接该文件夹。


### 链接一个或多个外部文件夹 {#link-one-or-more-external-folders}

1. 转到Workfront中需要文件夹的区域，然后单击  **文档** ![](assets/document-icon.png) 中。

1. 单击 **新增**，然后单击要将文件夹关联到的外部文档提供程序。Workfront
1. （视情况而定）如果您尚未授权外部服务，请指定外部提供商的登录凭据，然后单击 **登录**.

   您已授权的外部提供程序将显示在列表顶部。

1. 在 **链接外部文件和文件夹** 框中，浏览到要链接的文件夹并将其选中。

   或

   键入要搜索的文件夹的名称，然后按 **输入**.

   您可以选择多个文件夹；但是，只有在当前视图中选择的文件夹才会被链接。 例如，如果您选择一个文件夹，然后转到文件夹，则最初选择的文件夹不会关联。

   >[!NOTE]
   从Google驱动器链接文件夹时，您只能链接位于您个人驱动器（我的驱动器）和Team Drive中的文件夹。 无法从“与我共享”区域链接文件夹。

1. 单击 **链接**.

   在Workfront中，云提供商的徽标显示在文件夹旁边，表示它已链接到外部云提供商。

1. （可选）要重命名文件夹，以便Workfront中的文件夹名称与外部文档应用程序中的文件夹名称不同，请在 **文件夹** ，单击“更多”菜单 ![](assets/more-icon.png)  显示在文件夹名称旁边，然后单击 **重命名**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

这不会重命名外部应用程序中的文件夹。

### 将子文件夹添加到链接的文件夹  {#add-subfolders-to-a-linked-folder}

您可以在现有链接文件夹内创建新文件夹。 您还可以将其他文件夹拖到现有的链接文件夹中。

1. 要在现有链接文件夹中创建新文件夹，请转到现有文件夹，然后按照 [创建文档文件夹](../../documents/organizing-documents/create-documents-folder.md).

   或

   要将现有文件夹拖到现有链接文件夹中，请转到所需子文件夹所在的“文档”区域，然后将其拖到链接的文件夹中。

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   将现有Workfront文件夹拖入链接的文件夹时，会受到以下限制：
   * 您拖动的文件夹无法链接，也不能包含任何已链接的内容。
   * 您拖动的文件夹（包括其内容）不能超过50 MB。


## 将文档添加到链接的文件夹

通过Workfront将文档添加到链接的文件夹时，它会自动添加为链接的文档。

1. 在 **文档** 将文档拖动到链接的文件夹中。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode"> <img src="assets/documents-linked-document-move-nwe-350x126.png" style="width: 350;height: 126;">Selection box is wonky on the left<br></p>
   -->

   或

   选择所需文档的链接文件夹，单击 **新增>文档**，然后浏览到文档并将其添加到文件夹。

   系统将在外部应用程序中自动创建文档的新版本并将其链接到Workfront。

## 删除链接的文档或文件夹

从外部应用程序中删除链接的文档或文件夹时，该文档或文件夹会一直保留在Workfront系统中，直到您还从Workfront中删除它为止。

1. 选择链接的文档或文件夹，然后单击 **删除**.
1. 在显示的确认框中，单击 **是，取消链接**.

   文档已从Workfront网站中取消链接。 它在外部应用程序中不受影响。

## 关于重命名链接的文档和文件夹

重命名链接的文档或文件夹时，所做的更改仅在创建该文档或文件夹的应用程序中可见。 例如，如果在Workfront中重命名链接的文档，则新名称仅在Workfront中可见。

如果希望名称在Workfront和外部应用程序中匹配，则必须同时在这两个位置对其重命名。

>[!IMPORTANT]
请勿在Workfront中重命名链接到Dropbox的文档；这样做会导致无法访问Workfront中的文件。 相反，请在Dropbox中重命名文件，然后重新同步该文件，如 [从外部应用程序链接文档](#synchronizing-changes-made-on-a-linked-document).
