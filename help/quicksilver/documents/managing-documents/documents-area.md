---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: “文档”区域
description: 在文档区域中，您可以组织、管理和查看上载到Adobe Workfront的文档的元数据。 您还可以看到验证决定。
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# “文档”区域

在文档区域中，您可以组织、管理和查看上载到Adobe Workfront的文档的元数据。 您还可以看到验证决定。

Workfront当前具有两个版本的文档区域：旧版文档区域和新版文档区域。 您的企业使用的版本取决于您的企业使用的是旧版Workfront存储还是企业级存储。 有关这些存储类型的详细信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 旧文档区域

文档区域有两种类型。 两者的特性和功能相同：

* **项目、项目组合、项目、任务或问题中的文档区域：**&#x200B;列出您有权访问特定项目、任务或问题的所有文档。 要访问此区域，请在查看项目、任务或问题时单击左侧面板中的&#x200B;**文档** ![文档图标](assets/document-icon-12x14.png)。

* **全局文档区域：**&#x200B;列出您在Workfront中有权访问的所有文档。 要访问此区域，请在主菜单&#x200B;**主菜单图标**&#x200B;中单击![文档](assets/document-icon.png) ![文档图标](assets/main-menu-icon.png)。

有关将文档上传到Workfront的信息，请参阅[将文档从您的文件系统添加到Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。


“单据”区域记录以下项目的计数：

* Workfront文件夹
* 从文件系统上传的文件
* 从集成添加到Workfront的文件
* 链接的Experience Manager Assets

### 摘要面板

在文档区域中选择文档时，可以使用右侧的摘要查看文档详细信息、管理文档更新和批准、查看文档版本以及为文档添加和编辑自定义Forms。

如果文档设置了校样，则“详细信息”部分包括校样截止日期和当前校样进度等信息。

当您需要有关文档的所有信息时，可以单击详细信息标题转到完整的文档详细信息区域。

![文档区域](assets/documents-area-v2-350x199.png)

有关摘要的信息，请参阅[文档摘要概述](../../documents/managing-documents/summary-for-documents.md)。

### 校对决定

做出验证决策后，该决策将显示在文档列表中。

![文档列表中的校对决定](assets/proof-decision---doc-list-350x168.png)

### 文件夹

在上传文档的项目、任务或问题中，您可以设置文件夹来组织文档。 有关详细信息，请参阅[创建文档文件夹](../../documents/organizing-documents/create-documents-folder.md)。

在全局文档区域中，可以设置两种类型的文件夹来组织您有权访问的文档：

* **智能文件夹：**&#x200B;仅显示要查看的文档。 有关详细信息，请参阅[创建和管理智能文件夹](../../documents/organizing-documents/create-manage-smart-folders.md)。

* **我的文件夹：**&#x200B;按照您想要的方式组织文档。 有关详细信息，请参阅[创建文档文件夹](../../documents/organizing-documents/create-documents-folder.md)。

### 已展开文档详细信息

“文档详细信息”页面提供了右侧摘要中文档详细信息的更完整版本。

## 新建文档区域

>[!NOTE]
>
>全局文档区域在新文档区域体验中不可用。 您只能访问项目、项目组合、项目、任务或问题中的文档。

### 使用摘要面板

在文档区域中选择文档时，可以使用右侧的“摘要”面板查看有关文档的详细信息、添加和编辑附加的自定义表单、创建和管理审批工作流、查看文档版本等。

#### 使用Frame.io进行审阅和批准

您可以使用Frame.io查看器审阅和批准新文档区域中的文档。

有关详细信息，请参阅[统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

#### 管理版本

您可以在新建文档区域上载文档的新版本。 上传新版本时，将保留以前的版本，并且可以从摘要面板访问。 版本会根据上传的日期和时间自动命名，但可以根据需要重命名。

您还可以为文档的特定版本启动新的审批工作流。

#### 查看文档历史记录

您可以在新建文档区域查看文档历史记录。 历史记录包括以下类型的信息：

* 上传文档的时间
* 上传新版本时
* 启动文档的审批工作流时
* 等等

### 用于文档权限的系统级文件夹

将第一个文档上传到任务或问题时，Workfront会自动创建系统级文件夹。 这些文件夹从任务或问题继承权限，并在项目级别的文档区域可见。 上传到该任务或问题的所有文档都存储在该文件夹中，并从该文件夹继承权限。 这是管理新文档区域中文档权限的主要方式。 有关详细信息，请参阅[Adobe企业存储模型的对象权限和访问级别概述](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work)。