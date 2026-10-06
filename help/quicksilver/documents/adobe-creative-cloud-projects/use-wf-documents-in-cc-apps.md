---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: 在Creative Cloud应用程序中使用Workfront文档
description: 从Photoshop、Illustrator和InDesign中打开、编辑和保存Workfront文档，并请求获得批准。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: e8e94a483c700dc00466ce7fa37f9ddaf3e86004
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 2%
---
# 在Creative Cloud应用程序中使用Workfront文档

在Workfront项目面板中提供Creative Cloud项目后，您可以直接从Photoshop、Illustrator或InDesign处理其文档。

## 先决条件

* 您的组织必须采用支持Adobe云存储的Workfront版本。
* Workfront和Photoshop、Illustrator或InDesign必须有权使用同一个Adobe Identity Management System (IMS)组织。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront版本</td> 
   <td>工作流程Ultimate，启用了Adobe云存储</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>
      <p>查看对项目的访问权限以在Creative Cloud项目面板中查看它</p>
      <p>编辑对项目的访问权限以添加、编辑或删除项目</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 访问Workfront项目

Workfront项目中的“文档”文件夹结构会镜像到“项目”面板中。 当您从项目文件夹中打开文档、编辑该文档并保存时，您的更改将显示在Workfront中。

>[!NOTE]
>
>项目面板中不支持旧版Workfront存储项目 — 仅限Adobe云存储项目。


要在Photoshop、Illustrator或InDesign中访问Workfront项目，请执行以下操作：

1. 打开Photoshop、Illustrator或InDesign。
1. 在应用程序左侧的&#x200B;**项目**&#x200B;面板中，选择要打开的Workfront项目。

   项目面板中列出了![个Workfront项目](assets/cc-projects.png)

1. 在项目中打开文档以对其进行编辑。 保存更改后，这些更改将自动保存回Workfront项目。


>[!TIP]
>
>要编辑Photoshop、Illustrator或InDesign无法打开的文件类型，如Word或Excel文档，请改用Adobe Cloud Drive。 有关详细信息，请参阅[Adobe Cloud Drive概述](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md)。

## 从Creative Cloud应用程序将新文档保存到Workfront

1. 打开Photoshop、Illustrator或InDesign，然后创建新文件。
1. 在顶部菜单中，选择&#x200B;**文件>另存为**。
1. 在&#x200B;**另存为**&#x200B;对话框中，选择&#x200B;**保存到云文档**，然后选择所需的Workfront项目。

   >[!NOTE]
   >
   >保存已存在于Workfront项目中的文档时，另存为对话框未打开。 您可以选择一个Workfront项目，保存到其他文件夹或选择其他Workfront项目。


   ![在workfront中保存新文档](assets/save-new-to-wf.png)

1. 选择文档文件夹，然后单击&#x200B;**保存**。 如果不选择文件夹，文档将保存到项目根文件夹。

   ![选择文件夹以在workfront中保存新文档](assets/save-to-folder.png)

## 请求审批文档

您可以在Workfront中将文档审批添加到从Photoshop、Illustrator、InDesign或Adobe Cloud Drive上传的任何文档，这与任何其他文档相同。 有关详细信息，请参阅[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。



## 从Creative Cloud应用程序管理Workfront中的文档版本

将文档从Photoshop、Illustrator或InDesign保存到Workfront时，您保存的更改将显示在“版本”选项卡的“当前”文件中，并带有“新更改”标记。

您可以请求审批当前文件，而不是上传文档的新版本。 有关详细信息，请参阅[请求批准当前文件](#request-approval-on-the-current-file)。

![具有新更改徽章的当前文件](assets/current-file.png)

### 请求审批当前文件

要在Workfront中请求审批文档的当前文件，请执行以下操作：

1. 转到Workfront中的项目，该项目包含要申请批准的文档。
1. 打开文档，然后转到&#x200B;**版本**&#x200B;选项卡。
1. 在当前文件中，单击&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**请求审批**。
1. 在&#x200B;**请求审批**&#x200B;对话框中，按照[创建文档审批工作流](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)中的步骤创建审批。

   ![请求审批当前文件](assets/request-update-on-current-file.png)

