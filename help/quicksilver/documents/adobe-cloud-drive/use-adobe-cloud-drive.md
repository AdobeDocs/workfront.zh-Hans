---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: 使用Adobe Cloud Drive
description: 使用Adobe Cloud Drive直接从Finder或文件资源管理器使用Adobe云存储项目。 在任意应用程序中打开和编辑文件、脱机工作以及解决冲突。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 19e1a78a32429ddba173583bf56af8acc5d72eb0
workflow-type: tm+mt
source-wordcount: '3955'
ht-degree: 1%
---
# 使用Adobe Cloud Drive

安装Adobe Cloud Drive后，您可以直接从Finder或文件资源管理器中使用您的Adobe云存储项目。 您可以在任意应用程序中打开和编辑文件、脱机工作，以及让Adobe云驱动器将更改同步到云。

有关安装Adobe云驱动器的信息，请参阅[安装Adobe云驱动器](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)。

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
      <p>查看对项目的访问权限以在Adobe Cloud Drive中查看它</p>
      <p>编辑对项目的访问权限以添加、编辑或删除其中的文件</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 访问您的项目

1. 打开Finder (Mac)或文件资源管理器(Windows)。
1. 导航到&#x200B;**Adobe Cloud Drive**。
1. 在Workfront中浏览您有权访问的项目列表。 打开任意项目文件夹以查看其文件和子文件夹。

   >[!NOTE]
   >
   >* 项目文件夹在顶级为只读。 不能重命名、删除或移动项目文件夹本身。
   >* 您可以处理项目文件夹中的文件和文件夹 — 打开、编辑、创建、删除等。
   >* 旧版Workfront项目不会显示在Adobe Cloud Drive中。 只有存储在Adobe云存储中的项目才可用。

## 文件状态指示器

Adobe Cloud Drive使用视觉指示器显示文件同步状态。 Windows和Mac的图标有所不同。

### Windows上的文件状态指示器

| 图标 | 状态 | 文件含义 | 文件夹含义 |
| --- | --- | --- | --- |
| ![仅在线图标](assets/acd-windows-online-only.png) | 仅联机 | 文件已同步，但仅在线可用。 | 中的所有文件均可以联机使用。 |
| ![正在同步图标](assets/acd-windows-syncing.png) | 正在同步 | 文件的最新更新正在同步到本地缓存或Adobe云存储。 | 文件夹中至少有一个文件正在同步。 |
| ![可用的脱机图标](assets/acd-windows-available-offline.png) | 可离线使用 | 文件已同步并可供脱机使用。 | 文件夹中至少有一个文件可脱机使用。 |
| ![固定图标](assets/acd-windows-pinned.png) | 已固定（始终保留在设备上） | 文件已同步并始终保持脱机。 Adobe Cloud Drive不会自动清除固定内容。 | 文件夹中的所有文件都位于本地缓存中，可以脱机使用。 |
| ![只读图标](assets/acd-windows-read-only.png) | 只读 | 文件是只读的。 | 文件夹为只读。 |
| ![同步错误图标](assets/acd-windows-sync-error.png) | 同步错误 | 无法同步文件。 将鼠标悬停在图标上可查看详细信息。 | 无法同步文件夹。 将鼠标悬停在图标上可查看详细信息。 |
| ![同步排除图标](assets/acd-windows-sync-excluded.png) | 同步已排除 | 文件无法同步，因为类型或名称不受支持。 | 由于名称不受支持，无法同步文件夹。 |

### Mac上的文件状态指示器

| 图标 | 状态 | 文件含义 | 文件夹含义 |
| --- | --- | --- | --- |
| （无图标） | 可离线使用 | 文件已同步并可供脱机使用。 | 所有文件都可以脱机使用。 |
| ![仅在线图标](assets/acd-mac-online-only.png) | 仅联机 | 文件已同步且仅在线可用。 | 文件夹中至少有一个文件处于联机状态。 |
| ![正在同步图标](assets/acd-mac-syncing.png) | 正在同步 | 文件的最新更新正在同步到本地缓存或Adobe云存储。 | 正在同步文件夹内容。 |
| ![同步错误图标](assets/acd-windows-sync-error.png) | 同步错误 | 文件无法更新或同步。 将鼠标悬停在图标上可查看详细信息。 | 无法更新或同步文件夹。 将鼠标悬停在图标上可查看详细信息。 |
| ![同步排除图标](assets/acd-windows-sync-excluded.png) | 同步已排除 | 文件已从同步中排除。 | 将从同步中排除文件夹。 |
| ![只读图标](assets/acd-mac-read-only.png) | 只读 | 文件是只读的。 | 文件夹为只读。 |
| ![固定图标](assets/acd-windows-pinned.png) | 已固定（始终保留在设备上） | 文件已固定为可脱机使用。 Adobe Cloud Drive不会自动清除固定内容。 | 文件夹已固定为可脱机使用。 |

### 错误工具提示

发生同步错误或问题时，将鼠标悬停在文件或文件夹图标上可查看描述问题的工具提示。

| 错误类别 | 工具提示 | 含义 |
|---|---|---|
| 同步已排除 | 不支持的文件类型 | Adobe Cloud Drive不支持该文件类型。 |
| 同步已排除 | 不支持的文件名 | Adobe Cloud Drive不支持该文件名。 |
| 同步已排除 | 已删除父项目 | 已删除父Workfront项目。 |
| 同步已暂停 | 文件内容不受支持 | 无法同步文件内容（例如，检测到安全问题）。 |
| 同步已暂停 | 文件名中的字符无效 | 文件名包含无效字符。 |
| 同步已暂停 | 完整路径过长 | 文件路径超出了允许的最大长度。 |
| 同步已暂停 | 无写入权限 | 您对此文件或项目的写入权限已撤销。 |
| 同步错误 | 身份验证问题 | 您的登录凭据存在问题。 |
| 同步错误 | 云存储不可用 | Adobe云服务暂时不可用。 |
| 同步错误 | 云存储已满 | 您的云存储配额已满。 |
| 同步错误 | 本地磁盘已满 | 您的本地磁盘没有足够的可用空间。 |
| 同步错误 | 无互联网连接 | 您的设备未连接到Internet。 |
| 同步错误 | 意外错误 | 同步期间发生意外错误。 |
| 同步错误 | 帐户被阻止 | 服务已阻止您的帐户。 |

>[!NOTE]
>
>系统级错误（例如已断开连接、身份验证失败、网络不可用、本地磁盘已满或云存储已满）显示在系统任务栏(Windows)或菜单栏(Mac)中，而不是显示在单个文件中。

### 同步排除列表

Adobe Cloud Drive从同步中排除某些系统生成的临时和锁定文件。 排除下列文件类型和模式：

| 类别 | 文件类型/模式 | 描述 |
|---|---|---|
| 系统文件 | `.DS_Store`, `Thumbs.db` | 操作系统元数据和缩略图缓存文件。 |
| 系统和虚拟内存文件 | `*.sys` （例如，`hiberfil.sys`，`pagefile.sys`，`swapfile.sys`） | 用于虚拟内存、休眠或其他操作系统功能的大型系统文件。 |
| macOS索引文件 | `.Spotlight-V100`, `.fseventsd` | macOS聚焦索引和文件系统事件跟踪文件。 |
| 临时和备份文件 | `*.tmp`, `*.swp`, `*~`, `*.bak` | 应用程序生成的临时、临时或备份文件。 |

## 打开文件

1. 在Adobe Cloud Drive中，导航到文件。
1. 双击文件。

   该文件在其默认应用程序中打开。

Adobe Cloud Drive支持计算机上安装的应用程序可以打开的任何文件类型，包括：

* Adobe Creative Cloud格式（PSD、AI、INDD、PRPROJ、AEP等）
* Microsoft Office文档(DOCX、XLSX、PPTX)
* 图像（JPG、PNG、GIF等）
* 视频文件（MP4、MOV等）

>[!NOTE]
>
>当您通过Adobe Cloud Drive访问Cloud Document格式（PDC、AIDC等）时，它们会打开作为相应的标准格式（PSD、AI等）。

## 编辑并保存文件

1. 从Adobe Cloud Drive打开文件。
1. 在应用程序中进行更改。
1. 选择&#x200B;**文件** > **保存**，或者按Ctrl+S (Windows)或Cmd+S (Mac)保存文件。

   您的更改会自动同步到Adobe云存储。

>[!IMPORTANT]
>
>使用&#x200B;**文件** > **保存**&#x200B;或键盘快捷键保存文件。 避免使用&#x200B;**另存为**&#x200B;创建副本，因为它在驱动器中生成重复的文件。

## 创建或添加新文件

您可以直接在项目中创建新文件，或从本地存储中添加现有文件。

### 从应用程序创建新文件

1. 打开要用于创建文件的应用程序。
1. 按常规方式创建文件。
1. 保存后，在Adobe Cloud Drive项目文件夹内选择一个位置。

   该文件将显示在Adobe云驱动器中，并同步到Adobe云存储。

### 将现有文件添加到项目

1. 在Finder (Mac)或文件资源管理器(Windows)中，打开Adobe云驱动器中的项目文件夹。
1. 将文件从本地存储拖放或复制到项目文件夹中。

   文件会自动同步到Adobe云存储。

## 使文件和文件夹脱机可用

当某个文件或文件夹可以脱机使用时，无需通过Internet连接即可打开和编辑它。 脱机文件使用本地磁盘空间。

### 在设备上保留文件或文件夹

1. 右键单击Adobe Cloud Drive中的文件或文件夹。
1. Select **始终保留在此设备上**。

   文件或文件夹将下载到本地缓存，即使您处于脱机状态，也可以使用它。

### 删除脱机访问以释放空间

1. 右键单击脱机文件或文件夹。
1. Select **释放空间**。

   文件或文件夹仍保留在云存储中，但它已从本地缓存中删除。

>[!NOTE]
>
>脱机文件和文件夹使用本地磁盘空间。 删除对不再需要释放空间的文件和文件夹的脱机访问。

## 将文件复制到本地存储

您可以将文件从Adobe Cloud Drive复制到本地驱动器。 原始文件保留在Adobe Cloud Drive中，副本将变为独立的本地文件。

1. 在Adobe Cloud Drive中右键单击文件。
1. Select **复制**，然后将文件粘贴到本地驱动器上所需的位置。

   文件将复制到目标。 原件留在Adobe Cloud Drive中。

>[!NOTE]
>
>复制到本地存储的文件是独立的副本。 您对本地副本所做的更改不会同步回Adobe云存储。

<!-- Courtney check me: New sections below (Upload to Cloud through Open in Workfront) added for Adobe Cloud Drive v1.2.0, per helpxNewFeature.pdf from Pulkit Goel. Verify content, placement, and heading order. -->

## 将文件上传到云（直接上传） {#direct-upload}

<!-- Courtney check me: Source PDF calls this "Upload to Cloud (Direct Upload)". Confirm heading wording. -->

直接上传会将文件从计算机直接发送到Adobe云存储，而无需先将文件复制到Adobe云驱动器文件夹。

<!-- Courtney check me: Removed folder mentions from the Direct Upload section (intro, heading, step 1, 500-file bullet, hidden files bullet, and the Sync Activity link text), per Pulkit: folder support isn't available yet. Confirm nothing else should change. -->

### 上载文件

1. 在Finder (Mac)或文件资源管理器(Windows)中右键单击文件。
1. Select **上传至Cloud**。
1. 在目标选取器中，选择Adobe Cloud Drive中某个项目内的位置，然后单击&#x200B;**在此处上传**。
1. 在同步活动窗口的&#x200B;**直接上传**&#x200B;部分中监视进度。

### 关于直接上传的注意事项

* 直接上传会将项目复制到云中。 原始项目将保留在其当前位置。
* 您可以选择同时上传多个项目。
* “直接上传”部分仅列出单个文件，最多500个。
* 您可以从用户主目录或任何连接的外部驱动器上传项目。 不支持其他云存储位置，如iCloud驱动器或`~/Library/CloudStorage`。
* 您必须使用授权的Adobe帐户登录。 您不需要Internet连接即可开始上传。 如果没有连接，上载将保持排队状态。
* 暂停同步会取消正在进行的上传。 当您恢复同步时，已排队的上载会自动恢复。
* 如果您在上传期间退出Adobe Cloud Drive，则进行中的上传将标记为已取消。 重新启动应用程序后，排队的上传会自动恢复。
* 不支持隐藏的文件、符号链接和别名。
* Adobe Cloud Drive控制同时运行的上传数量。 其余的上传将一直排队，直到插槽可用。
* 显示实时上传计数，包括失败的上传，例如“3个文件上传”。 当所有上传成功完成时，计数将更改为摘要，例如“已上传3个文件”。 Select **关闭**&#x200B;以将其删除。

<!-- Courtney check me: "Pausing sync cancels uploads in progress" and the quit behavior are from the PDF. Confirm with dev that both are intended. -->

### 上传状态

<!-- Courtney check me: Icons extracted from the PDF (48x48 px, low resolution) and named by table order. Verify each icon matches its status and ask Pulkit's team for higher-resolution originals. Add alt text review too. -->

| 图标 | 状态 | 描述 | 可用操作 |
| --- | --- | --- | --- |
| ![已排队图标](assets/acd-upload-status-queued.png) | 已排队 | 上传正在等待启动。 | **取消**&#x200B;取消此项。 |
| ![正在上传图标](assets/acd-upload-status-uploading.png) | 正在上传 | 上传正在进行中。 | **取消**&#x200B;取消此项。 |
| ![已完成图标](assets/acd-upload-status-completed.png) | 已完成 | 上载已成功完成。 | 在Workfront中打开&#x200B;**在Workfront Web界面中打开资产**。 |
| ![失败的图标](assets/acd-upload-status-failed.png) | 失败 | 无法完成上载。 | **显示源文件**&#x200B;显示原始文件。 **重试**&#x200B;重试上传。 重试仅适用于某些故障。 |
| ![已取消图标](assets/acd-upload-status-cancelled.png) | 已取消 | 上传已由您或系统停止。 | 无。 不会重试已取消的上传。 您必须开始新的上载。 |

要查看失败的原因，请将鼠标悬停在失败的项目上。

### 管理上载列表

每个操作仅在适用时才可用。

* **取消所有上传：**&#x200B;在上传排队或正在进行时可用。 全部取消。
* **重试失败的上传：**&#x200B;当存在可以重试的失败的上传时可用。 重试所有步骤。 无法重试的上传将保持不变。
* **清除：**&#x200B;当没有上载排队或正在进行中时可用。 删除所有已完成、失败和取消的项目。 已上传的本地文件和内容不会受到影响。
* **自动清除：**&#x200B;已完成、失败和已取消的项目，将在上次更新后24小时自动删除。 排队的项和进行中的项永远不会自动删除。

## 暂停并继续同步 {#pause-resume-sync}

如果您不想上载或下载文件（例如，通过慢速或按流量计费的Internet连接），可以暂停Adobe Cloud Drive。 同步暂停时，您的更改不会发送到云，并且云中的更改不会下载到您的计算机。 同步将保持暂停状态，直到您恢复同步。

### 暂停同步

1. 单击系统任务栏(Windows)或菜单栏(Mac)中的Adobe Cloud Drive图标。
1. 单击Adobe云驱动器窗口右上角的&#x200B;**菜单**&#x200B;图标(≡)。
1. Select **暂停同步**。

   >[!TIP]
   >
   >打开Adobe Cloud Drive窗口后，您还可以按Ctrl+P (Windows)或Command+P (Mac)。

   Adobe Cloud Drive窗口显示&#x200B;**同步已暂停**，并且消息&#x200B;**文件将在您继续操作**&#x200B;后才会同步。 将鼠标悬停在Adobe Cloud Drive图标上时，将显示&#x200B;**Adobe Cloud Drive（已暂停）**。

>[!NOTE]
>
>暂停同步仅在您登录并连接Adobe Cloud Drive后可用。

### 继续同步

1. 单击系统任务栏(Windows)或菜单栏(Mac)中的Adobe Cloud Drive图标。
1. 执行下列操作之一：

   * 单击&#x200B;**继续**。
   * 单击&#x200B;**菜单**&#x200B;图标(≡)，然后选择&#x200B;**继续同步**。 打开窗口后，您还可以按Ctrl+R (Windows)或Command+R (Mac)。

   Adobe Cloud Drive会再次开始同步，包括同步暂停时所做的任何更改。

## 查看和管理版本历史记录 {#version-history}

您可以使用Adobe Cloud Drive中的版本历史记录来浏览受支持文件的已保存云版本，查看版本详细信息和缩略图，以及还原到早期版本。 如果您具有所需的权限，您还可以编辑版本的名称和描述。

### 查看版本历史记录

1. 在Finder或文件资源管理器中导航到您的Adobe Cloud Drive文件夹。
1. Select支持的文件。
1. 右键单击该文件并选择&#x200B;**版本历史记录**。
1. Select版本以查看其可用详细信息和缩略图。

   如果文件没有以前的版本，则显示&#x200B;**没有以前的版本**。 缩略图可能不适用于每个文件或版本。

### 编辑版本信息

1. 打开文件的版本历史记录。
1. Select要更新的版本。
1. 打开版本的选项菜单，然后选择&#x200B;**编辑版本信息**。
1. 输入&#x200B;**版本名称**&#x200B;或&#x200B;**描述**。
1. 选择&#x200B;**保存**。

   更新后的信息将保存并在您重新打开“版本历史记录”时显示。

### 还原到早期版本

1. 打开文件的版本历史记录。
1. Select要恢复的版本。
1. Select **还原到此版本**（如果可用）。
1. 等待同步完成。
1. 重新打开文件以验证所选版本的内容是否为当前版本。

## 管理本地存储 {#manage-local-storage}

您可以使用Adobe云驱动器中的“管理本地存储”来监视本地磁盘使用情况、设置存储限制以及查看在此设备&#x200B;**上标记为**&#x200B;始终的文件。

<!-- Courtney check me: PDF says "Always on this device" here but this article uses "Always Keep On This Device" for the right-click option. Confirm which label the UI shows in each place. -->

### 查看本地存储使用情况

1. Select Adobe Cloud驱动器图标并打开其选项菜单。
1. Select **管理本地存储**。
1. 查看当前存储使用情况以及此设备&#x200B;**上标记为**&#x200B;始终的文件列表。
1. 按&#x200B;**名称**&#x200B;或&#x200B;**大小**&#x200B;对文件列表进行排序，以查找特定文件。

### 更改本地存储限制

1. 从Adobe Cloud Drive选项菜单中打开&#x200B;**管理本地存储**。
1. 输入所需的存储限制。
1. Select **保存**&#x200B;以应用更改。

>[!NOTE]
>
>在设置存储限制时，请确保设备上有足够的可用磁盘空间。

## 查看同步活动 {#sync-activity}

同步活动显示计算机上的Adobe Cloud Drive文件夹与Adobe Cloud Storage之间最近的活动。 使用它可以监视上载和下载，查看已完成的更改，并识别无法同步的项目。

### 查看同步活动

1. Select菜单栏(Mac)或系统任务栏(Windows)中的Adobe Cloud驱动器图标。
1. 使用同步活动状态摘要旁边的箭头展开该活动部分。
1. 查看列出的项目及其状态指示器。 将鼠标悬停在状态指示器上可查看传输进度、已完成的操作或错误消息。
1. Select项目旁边的更多操作菜单，可查看可用于该项目的操作。

### 关于同步活动的注意事项

* Normal sync会跟踪通过Adobe Cloud Drive文件夹所做的更改，包括上传、下载、创建、重命名、移动和删除。
* 普通同步列表包含最多500个最近的条目。 新条目或更新条目显示在顶部。 当列表达到其限制时，可能会删除旧条目。
* 在解析条目名称或元数据时，条目最初可以显示&#x200B;**正在准备……**。
* 摘要显示当前同步的项目数。 **同步完成**&#x200B;表示当前没有处于活动状态的项目。 检查列表中是否有失败或排除的项目，而不是将此摘要视为确认每个项目均成功。
* 从同步中排除的文件和文件夹可能会出现一个错误，该错误会说明不支持的名称、不支持的类型或其他排除原因。
* 注销时清除活动。 该列表是活动视图，而不是永久审核历史记录。

### 同步状态

<!-- Courtney check me: The PDF has two sync status tables (page 7 with 4 statuses, page 8 with 3 statuses and icons). I used the page 8 icons with the page 7 descriptions where they overlap. Confirm and decide whether to keep both tables. -->

| 图标 | 状态 | 描述 | 可用操作 |
| --- | --- | --- | --- |
| 等待指示器 | 正在等待同步 | 项目正在等待其操作开始。 | 在查找器中显示&#x200B;**** (Mac)或在资源管理器中显示&#x200B;**** (Windows)（如果适用）。 |
| ![正在上传图标](assets/acd-sync-status-uploading.png) | 上传/下载 | 正在传输文件内容。 将鼠标悬停在指示器上可查看传输方向和百分比（可用时）。 工具提示显示为100%，在处理完成之前可能显示&#x200B;**正在完成……**。 | **在Finder**&#x200B;中显示，或在Explorer **中显示（如果适用）。** |
| ![已完成图标](assets/acd-sync-status-completed.png) | 已同步/已完成的操作 | 操作已完成。 工具提示可以识别云中上传的、下载的、创建的、重命名的、重命名的、移动的、删除的或删除的。 | 在Finder中显示&#x200B;****&#x200B;或在资源管理器中显示&#x200B;****&#x200B;未删除的项目。 在Workfront中&#x200B;**打开**&#x200B;符合条件的已完成未删除项目。 |
| ![失败的图标](assets/acd-sync-status-failed.png) | 同步失败/已排除 | 该项目无法同步或已从同步中排除。 将鼠标悬停在指示器上可查看原因。 | **在Finder**&#x200B;中显示，或在Explorer **中显示（如果适用）。**&#x200B;在预期同步项目之前，请解决报告的问题。 |

已删除的项目无法显示在本地，也无法从其活动条目在Workfront中打开。

### 管理活动列表

| 操作 | 描述 |
| --- | --- |
| 展开或折叠 | 使用同步摘要旁边的箭头可显示或隐藏单个条目。 |
| 在Finder中显示/在资源管理器中显示 | 在Adobe Cloud Drive文件夹中找到未删除的项目。 |
| 在Workfront中打开 | 在浏览器的Workfront中打开一个符合条件的已完成项目。 此操作不可用于活动、失败或删除的普通同步条目。 |
| 清除 | 当没有活动正常同步项目时可用。 从活动视图中清除完成的条目，包括失败的条目。 清除历史记录不会删除本地文件或云内容，也不会解决同步失败。 |
| 关闭 | 清除已完成的批次后，可能会显示同步项目摘要。 Select的“关闭”按钮可关闭摘要。 |

>[!NOTE]
>
>Normal-sync行不提供直接上载使用的每项&#x200B;**重试**&#x200B;或&#x200B;**取消**&#x200B;操作。 有关直接上传的信息，请参阅[将文件上传到云（直接上传）](#direct-upload)。

## 在Workfront中打开项目 {#open-in-workfront}

在Workfront中打开会将您从Adobe Cloud Drive中的项目转到浏览器中Workfront中的相应位置。 使用它可在Workfront中继续使用云项目，而无需手动搜索。

### 从Finder或文件资源管理器中打开项目

1. 在Finder (Mac)或文件资源管理器(Windows)中打开Adobe云驱动器文件夹。
1. Select与Workfront项目关联的单个文件或文件夹。
1. 右键单击该项并选择&#x200B;**在Workfront中打开**。

   您的浏览器将打开相应的Workfront位置。 如果出现提示，请使用有权访问该项目的帐户登录。

### 从同步活动打开项目

1. Select菜单栏(Mac)或系统任务栏(Windows)中的Adobe Cloud驱动器图标。
1. 展开同步活动部分。
1. 对于符合条件的已完成未删除项目，请打开更多操作菜单，然后选择&#x200B;**在Workfront中打开**。
1. 对于通过直接上传上传上传的文件，在&#x200B;**直接上传**&#x200B;部分中对其已完成的条目使用相同的操作。

### 关于Workfront Open的须知事项

* Select一次只能有一个项目。 不支持在Workfront中打开多个选定项目。
* 在文件资源管理器中，对于Adobe Cloud Drive文件夹之外的项目和驱动器根目录本身，命令是隐藏的。 在选择了多个项目时，该功能处于禁用状态。
* 项目必须具有相应的Workfront位置。 某些文件夹或其他项目可能没有Workfront映射，即使它们在Adobe Cloud Drive中可见。
* 尚未完成上传的新本地项目可能还没有Workfront链接。 请等待上传完成，然后重试。
* 在正常同步活动中，该操作仅针对符合条件的已完成条目提供。 不提供活动、失败或删除的条目。
* 在直接上传中，为已完成的上传提供操作，而不是为已排队、上传、失败或已取消的条目提供操作。
* 您必须登录到Adobe云驱动器。 Workfront可能还会要求您在浏览器中单独登录，并且您的Workfront权限仍然适用。
* 您需要通过Internet连接来检索未缓存的链接并访问Workfront。 之前解析的链接不提供对Workfront的脱机访问。
* 此操作将在浏览器中打开Workfront。 它不会在其桌面应用程序中打开文件、上载其他副本或更改其本地脱机可用性。

### 在Workfront可用性中打开

| 项目或状态 | 在Workfront中打开行为 | 要做什么 |
| --- | --- | --- |
| Adobe Cloud Drive中的单个合格项目 | 打开相应的Workfront位置。 | Select **在Workfront中打开**。 |
| 多个选定项目 | 不支持打开多个项目。 文件资源管理器禁用该命令。 | Select单个项目。 |
| 新项目仍在上传 | Workfront链接可能还不可用。 | 请等待上传完成，然后重试。 |
| 已完成正常同步条目 | 在项目符合条件且未被删除时可用。 | 使用条目的更多操作菜单。 |
| 已完成的直接上传条目 | 上传完成后可用。 | 使用条目的更多操作菜单。 |
| 不具有Workfront映射的项目 | 将显示一条消息，指示该项目在Workfront中不可用。 | 直接在Workfront中检查项目或选择其他受支持的项目。 |
| 已删除normal同步条目 | 该操作不可用。 | 如果需要调查已删除的项目，请直接使用Workfront。 |

## 注销Adobe Cloud Drive

如果您注销Adobe Cloud Drive，则该驱动器在Finder或文件资源管理器中保持可见。 但是，在注销时您在驱动器内所做的任何更改以及在注销前未同步的任何更改，都不会同步到云。

接下来发生什么取决于您使用哪个帐户重新登录。

### 使用同一帐户重新登录

当您注销时，Adobe Cloud Drive会保留本地装入的文件夹。 如果您使用相同的凭据重新登录：

* Adobe Cloud Drive会自动重用现有的装载。
* 在注销之前所做的任何未同步更改都将保留，并且会在连接恢复后同步。
* 您无需执行任何操作。

### 使用其他帐户登录

如果您在注销后使用其他Adobe帐户登录：

* 当前装入的文件夹会自动重命名和备份。 备份文件夹名称使用此格式： `Adobe Cloud Drive <usermail>_<short_guid> (backup yyyy-MM-dd HH-mm-ss)`。
* 与往常一样，映射到新帐户的Adobe Cloud Drive在Finder或文件资源管理器中可用。
* 您可以在删除备份文件夹之前手动恢复任何未同步的工作。

>[!NOTE]
>
>备份文件夹保存在Mac上的`~/Library/CloudStorage`中，保存在Windows上的`C:\Users\<user>\`中。 如果多次切换帐户，则会创建多个带有时间戳的备份文件夹。 定期检查并清理备份，以释放磁盘空间。

## 解决文件冲突

在以下任何情况下都可能发生冲突：

* 多个用户同时编辑或删除同一文件。
* 当其他用户打开某个文件时，该文件会被修改。
* 网络中断会导致同步问题。

### Adobe Cloud Drive如何解决冲突

Adobe Cloud Drive使用复制策略来解决冲突：

* **没有文件锁定。** 多个用户可以同时编辑文件。
* **自动复制。** 当Adobe Cloud Drive检测到冲突时，它会保留两个版本。
* **清除命名。** 冲突文件包括采用以下格式的用户名和时间戳： `filename (Conflicted copy from username on date_time).extension`。 例如：`hero-banner (Conflicted copy from John on 2026-02-10_16-06-44).psd`。

### 手动解决冲突

1. 确定冲突文件。 冲突文件的文件名中有“冲突的副本”。
1. 查看两个版本以确定哪个版本正确。
1. 保留正确的版本并删除其他版本。
1. 为保留的文件指定合适的名称。

>[!TIP]
>
>要最大限度地减少冲突，请执行以下操作：
>
>* 在编辑文件之前检查同步状态。
>* 与团队成员沟通谁正在编辑哪些文件。
>* 经常保存，以便更改能够及时同步。
>* 完成编辑后关闭文件。

