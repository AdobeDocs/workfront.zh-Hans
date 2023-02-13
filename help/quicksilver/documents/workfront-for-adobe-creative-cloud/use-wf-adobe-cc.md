---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: 使用适用于Illustrator的Workfront扩展和InDesign
description: 您可以使用Workfront扩展将您在Adobe Illustrator和Adobe InDesign中保存和创建的数字内容导出到Workfront。 这可加快文档审阅和批准流程。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# 使用适用于Illustrator的Workfront扩展和InDesign

>[!IMPORTANT]
>
>我们将用以下内容替换适用于Illustrator和InDesign的Workfront扩展 [更新了Creative Cloud插件](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). 从2022年底开始，将不再支持此扩展，并且可按原样使用。


您可以使用Workfront扩展将您在Adobe Illustrator和Adobe InDesign中保存和创建的数字内容导出到Workfront。 这可加快文档审阅和批准流程。

以下应用程序支持Workfront 2017及更高版本的Adobe Creative Cloud扩展：

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >我们建议使用 [Adobe Workfront for Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) 插件。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>除了Adobe Creative Cloud许可证之外，您还必须拥有Workfront许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对要与之交互的对象的访问权限。</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 从Illustrator或InDesign登录Workfront扩展 {#log-in-to-workfront-extension-from-illustrator-or-indesign}

当您从其中一个受支持的Adobe应用程序登录Workfront时，您将登录到所有受支持的Adobe应用程序。

1. 转到要在其中使用Workfront扩展的Adobe应用程序。

   有关每个受支持应用程序支持的格式列表，请参阅 [支持的导出文件格式](#supported-exported-file-formats) 在本文中。

1. 单击 **窗口** > **扩展** >Workfront。

1. （可选）将Workfront面板拖动到您希望在Adobe应用程序中显示它的位置。
1. 按照提示登录Workfront。

   >[!NOTE]
   >
   >* Workfront使用OAuth 2.0连接到Adobe Creative Cloud,OAuth 2.0是一个安全标准，大多数基于Web的集成都使用它来进行用户身份验证和授权。
   >* 当系统提示您输入 [域或主机] 在您的Workfront帐户中，使用以下格式键入： *yourCompany&#39;sDomain.my.workfront.com*. 您公司的域通常是您公司的名称。


   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

## 将文件上传到Workfront项目、任务或问题 {#upload-a-file-to-a-workfront-project-task-or-issue}

您可以从计算机文件系统上传文件，或将当前在Adobe Creative Cloud应用程序中打开的文件导出到Workfront项目、任务或问题。 

从Adobe Creative Cloud上传或导出文件时，请考虑以下事项：

* 您的访问级别必须允许将文档上传到Workfront。 有关更多信息，请参阅 [授予对文档的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* 您必须有权将文档上传到所需项目。 有关更多信息，请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* 文件将上传到您选择的Workfront对象的“文档”区域。
* 不能将文档导出到“主菜单”中的“文档”区域 ![](assets/main-menu-icon.png) 来自Adobe Creative Cloud应用程序。

本节将介绍以下内容：

* [上传文件](#upload-a-file)
* [导出当前在Illustrator或InDesign中打开的文件](#export-a-file-currently-open-in-illustrator-or-indesign)
* [从Illustrator或InDesign上传文件的新版本](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### 上传文件 {#upload-a-file}

您无需离开Adobe Creative Cloud应用程序，即可将文件上传到项目、任务或问题。

1. 如果在打开Workfront应用程序时未看到Adobe Creative Cloud扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 单击要将文件上传到的项目、任务或问题的名称。

   您可以通过在 **搜索** 框和选择 **项目**, **任务**&#x200B;或 **问题** 从右侧的下拉菜单 **搜索** 框中。 如果工作项的名称未显示在列表中，请按 **输入** 以搜索您有权查看的所有Workfront项目。

1. 单击 **选择**&#x200B;位于Workfront扩展的右下角。
1. 在 **单击以选择格式** 下拉菜单中，单击要在Workfront中保存文件的格式。

   有关每个受支持应用程序支持的格式列表，请参阅 [支持的导出文件格式](#supported-exported-file-formats) 在本文中。

1. （视情况而定）如果要上载文件的工作项包含文档文件夹，请在&#x200B;**单击以选择文档文件夹** 字段，然后单击 **选择**.

1. 单击 **上载本地文件**.
1. 在 **打开文件** 框中，在文件系统中找到文件，然后单击 **打开**.

1. （可选）为文件键入新名称。 

   ![](assets/rename-file-uploading.png)

1. 单击 **上传**.

   在Workfront中，文档现在列在您指定的项目、任务或问题的“文档”区域中。  

1. （可选）单击文档的名称以在Workfront中打开其“文档详细信息”页面。

   Workfront将在新的浏览器选项卡中打开。

### 导出当前在Illustrator或InDesign中打开的文件 {#export-a-file-currently-open-in-illustrator-or-indesign}

1. 在支持的Adobe Creative Cloud应用程序中，打开要导出到Workfront的文件。 
1. 如果未显示Workfront扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 单击要将文件导出到的项目、任务或问题的名称。

   您可以通过在 **搜索** 框和选择 **项目**, **任务**&#x200B;或 **问题** 从右侧的下拉菜单 **搜索** 框中。 如果工作项的名称未显示在列表中，请按 **输入** 以搜索您有权查看的所有Workfront项目。

1. 在 **单击以选择格式** 下拉菜单中，单击要在Workfront中保存文件的格式。

   有关每个受支持应用程序支持的格式列表，请参阅 [支持的导出文件格式](#supported-exported-file-formats) 在本文中。

1. （视情况而定）如果要上载文件的工作项包含文档文件夹，请在&#x200B;**单击以选择文档文件夹** 字段，然后单击 **选择**.
1. （可选）要重命名文档，请单击文档名称并键入新名称。

   ![](assets/rename-doc-exporting.png)

1. 单击 **导出**. 

   此时将显示一条消息，确认文档已成功导出到Workfront。

   在Workfront中，文档列在您在Workfront中指定对象的“文档”区域中。

1. （可选）单击文档的名称以在Workfront中访问该文档。

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront将在新的浏览器选项卡中打开。

### 从Illustrator或InDesign上传文件的新版本 {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. 如果要将在受支持的Adobe应用程序中处理的文件导出为Workfront中文件的新版本，请在Adobe应用程序中打开该文件。 
1. 如果未显示Workfront扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 单击列出现有文档的项目、任务或问题的名称。

   您可以通过在 **搜索** 框和选择 **项目**, **任务**&#x200B;或 **问题** 从右侧的下拉菜单 **搜索** 框中。 如果工作项的名称未显示在列表中，请按 **输入** 以搜索您有权查看的所有Workfront项目。

   上传到项目、任务或问题的所有文档都会显示在列表中，无论这些文档是否是从Adobe应用程序上传的。

1.  
1. 在 **单击以选择格式** 下拉菜单中，单击要在Workfront中保存文件的格式。

   如果要导出在Adobe应用程序中打开的文件，则需要此操作。 有关每个受支持应用程序支持的格式列表，请参阅 [支持的导出文件格式](#supported-exported-file-formats) 在本文中。

1. 如果要导出在Adobe应用程序中打开的文件作为所选Workfront文档的新版本，请单击 **导出**.

   或

   如果要从计算机文件系统上传文件作为所选Workfront文档的新版本，请单击 **上载本地文件**，在显示的框中查找文件，单击 **打开**，然后单击 **上传**.

1. （可选）单击文档的名称，以在Workfront中查看其新版本。 

   >[!NOTE]
   >
   >默认情况下，Workfront中文档的名称会填充，且无法编辑。 它也不会更改您上传或导出为新版本的文件的名称。
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## 对Illustrator或InDesign中Workfront文档的注释 {#comment-on-a-workfront-document-from-illustrator-or-indesign}

您可以直接在Adobe应用程序内向Workfront文档添加注释。 在Workfront中，您的注释显示在文档的“更新”区域和保存文档的Workfront项目的“更新”区域中。 

1. 打开一个支持的Adobe应用程序。
1. 如果未显示Workfront扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 单击列出现有文档的项目、任务或问题。

   您可以通过在 **搜索** 框和选择 **项目**, **任务**&#x200B;或 **问题** 从右侧的下拉菜单 **搜索** 框中。 如果工作项的名称未显示在列表中，请按 **输入** 以搜索您有权查看的所有Workfront项目。

1. 单击现有文档的名称，然后单击 **选择**&#x200B;位于Workfront扩展的右下角。
1. 单击 **注释** ，然后在显示的框中键入更新。

1. （可选）要将其他Workfront用户或团队包含在评论中，请在 **通知人员或团队** 框中，然后在名称出现在下拉列表中时单击该名称。
1. （可选）要请求对文档进行批准，请选择 **发出批准请求**.
1. 单击 **更新**.

   更新会发布在文档的“更新”选项卡中。 包含在评论中的Workfront用户会收到应用程序内通知，并且根据Workfront的配置方式，也可能会收到电子邮件通知。

   有关Workfront中通知的更多信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   有关接收电子邮件通知的更多信息，请参阅 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 从Illustrator或InDesign请求文档批准

您可以直接从Workfront应用程序请求Adobe文档批准。

您可以从以下实体请求文档批准：

* Workfront用户
* 没有Workfront帐户的外部用户

您可以通过以下方式从Adobe应用程序请求文档批准：

* 将审批者附加到文档。
* 通过对文档进行评论，在您评论时通知该人。 并将它们作为审批者附加到文档。

   有关在注释文档时请求批准的信息，请参阅 [对Illustrator或InDesign中Workfront文档的注释](#comment-on-a-workfront-document-from-illustrator-or-indesign) 在本文中。

要从Adobe申请中请求对文档进行批准，请执行以下操作：

1. 打开一个支持的Adobe应用程序。
1. 如果未显示Workfront扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 单击列出现有文档的项目、任务或问题，然后单击现有文档的名称。

   您可以通过在 **搜索** 框和选择 **项目**, **任务**&#x200B;或 **问题** 从右侧的下拉菜单 **搜索** 框中。 如果工作项的名称未显示在列表中，请按 **输入** 以搜索您有权查看的所有Workfront项目。

1. 单击现有文档的名称，然后单击 **选择**&#x200B;位于Workfront扩展的右下角。
1. 单击 **批准** 选项卡。
1. 要添加审批者，请在 **开始键入名称框** 执行以下操作之一：

   * 键入审批者的名称，然后在列表中显示时选择该名称。

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * 键入外部用户的电子邮件地址。

1. 单击 **请求批准**.

   您包含在评论中或添加为审批者的Workfront用户会收到应用程序内通知，并且根据Workfront的配置方式，也可能会收到电子邮件通知。\
   外部用户会收到一封电子邮件通知，通过该通知，他们可以决定批准事宜。

   有关Workfront中通知的信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 有关接收电子邮件通知的信息，请参阅 [Adobe Workfront通知](../../workfront-basics/using-notifications/wf-notifications.md).

## 从Illustrator或InDesign生成校样 {#generate-a-proof-from-illustrator-or-indesign}

如果贵组织使用自动工作流模板，则可以为您在Adobe应用程序中创建的文档生成校样，而无需离开该应用程序。 有关创建校样的信息，请参阅 [创建校样](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). 有关自动化工作流模板的信息，请参阅 [自动化工作流模板](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) in [自动化工作流概述](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. 打开一个支持的Adobe应用程序。
1. 如果未显示Workfront扩展，请单击 **窗口** > **扩展** >Workfront。

   如果项目处于当前状态，则会显示分配给您的工作项列表。 如果列表未显示，请登录Workfront。

   个人任务列在 **无项目**.

1. 如果文档已上传到Workfront，请在列出文档的Workfront扩展中选择项目、任务或问题，然后单击文档的名称。

   或

   将Adobe文档上传到Workfront对象，如部分中所述 [将文件上传到Workfront项目、任务或问题](#upload-a-file-to-a-workfront-project-task-or-issue) 在本文中，单击文档的名称。

1. 在 **单击以选择格式** 下拉菜单中，单击要在Workfront中保存文件的格式。

   在此后的步骤中启用校对功能后，某些格式将不可用。 有关更多信息，请参阅 [支持的导出文件格式](#supported-exported-file-formats) 在本文中。

1. 单击 **上传为新校样** 来启用它。
1. 选择 **工作流模板** 您希望用户在审阅文档时使用。

   您的Workfront管理员可设置自动化工作流模板，如中所述。 如果有问题，请咨询管理员。

   1. 至少添加一个 **新收件人** 到工作流模板中的每个阶段。

      您可以开始键入名称，并在显示的下拉列表中看到该名称后将其选中。

   1. 指定 **校样角色** 和频率 **电子邮件警报** 对于您添加的每个收件人。

   1. （可选）在 **电子邮件通知** 部分，选择是否向添加的所有校样收件人发送包含校样可选自定义消息的电子邮件通知。

1. 单击 **创建校样**.

   您可以查看校样创建过程的进度。 警报在生成完成后会显示。 您可以打开创建校样的任务，该任务将列在此处。

## 无需离开Illustrator或InDesign即可上传校样的新版本

1. 单击具有校样的现有文档，然后单击 **选择** 在右下角。
1. 单击 **上传为新校样版本** 来启用它。
1. （可选）选择 **工作流模板** 您希望用户在查看新版本时使用。

   如果不选择其他模板，则为早期版本选择的模板仍然有效。 此外，如果已为早期版本修改了模板，则所做的更改将对新版本生效。

   您的Workfront管理员可设置自动化工作流模板，如中所述。 如果有问题，请咨询管理员。

   1. 至少添加一个 **新收件人** 到工作流模板中的每个阶段。

      您可以开始键入名称，并在显示的下拉列表中看到该名称后将其选中。

   1. 指定 **校样角色** 和频率 **电子邮件警报** 对于您添加的每个收件人。
   1. （可选）在 **电子邮件通知** 部分，选择是否向添加的所有校样收件人发送包含校样可选自定义消息的电子邮件通知。

1. 单击 **创建新校样版本**.

   您可以查看校样创建过程的进度。 警报在生成完成后会显示。 您可以打开创建校样的任务，该任务将列在此处。

## 注销Workfront扩展

1. 在Adobe应用程序中，单击 **窗口** > **扩展** >Workfront。

1. 单击 **更多** 菜单 ![](assets/more-menu.png) 中。

1. （可选）单击 **反馈** 要打开一个简短的调查并向Workfront发送有关Workfront for Adobe Creative Cloud的反馈，请执行以下操作： 
1. 单击 **注销**.\
   此时会显示“登录”屏幕。 有关登录的信息，请参阅 [从Illustrator或InDesign登录Workfront扩展](#log-in-to-workfront-extension-from-illustrator-or-indesign) 在本文中。

## 支持的导出文件格式 {#supported-exported-file-formats}

* [支持的导出文件格式Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [支持的导出文件格式Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### 支持的导出文件格式Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

Workfront支持以下文件格式将文件从InDesign导出到Workfront:

* EPS — 封装的PostScript
* ePub — 固定版式电子出版物
* ePub — 可重排的电子出版物 &#42;
* HTML — 超文本标记语言
* IDML -InDesign标记语言 &#42;
* JPG、JPEG — 联合摄影专家组
* PDF-Adobe可移植文档文件
* PNG — 可移植网络图形
* SWF-Flash Player &#42;
* XML — 可扩展标记语言 &#42;

&#42; 当 **上传新校样** 已启用(有关此选项的信息，请参阅 [从Illustrator或InDesign生成校样](#generate-a-proof-from-illustrator-or-indesign) )。 如果在启用之前已选择此文件格式 **上传新校样**，则系统会将文件格式更改为PDF。 您可以从列表中选择其他格式。

### 支持的导出文件格式Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront支持以下文件格式将文件从Illustrator导出到Workfront:

* DWG - AutoCAD绘图、AutoCAD互换文件 &#42;
* JPG、JPEG — 联合摄影专家组
* PNG — 可移植网络图形
* PSD- Photoshop文档
* SWF-Flash Player &#42;
* TIFF — 标记的图像文件格式

&#42; 当 **上传新校样** 已启用(有关此选项的信息，请参阅 [从Illustrator或InDesign生成校样](#generate-a-proof-from-illustrator-or-indesign) )。 如果在启用之前已选择此文件格式 **上传新校样**，则系统会将文件格式更改为PNG。 您可以从列表中选择其他格式。
