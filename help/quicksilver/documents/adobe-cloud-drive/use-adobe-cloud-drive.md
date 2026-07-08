---
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: 使用Adobe Cloud Drive
description: 使用Adobe Cloud Drive直接从Finder或文件资源管理器使用Adobe云存储项目。 在任意应用程序中打开和编辑文件、脱机工作以及解决冲突。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d5dd769447e81d5d95b4907f8a01016b118f2322
workflow-type: tm+mt
source-wordcount: 1723
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
1. 选择&#x200B;**始终保留在此设备上**。

   文件或文件夹将下载到本地缓存，即使您处于脱机状态，也可以使用它。

### 删除脱机访问以释放空间

1. 右键单击脱机文件或文件夹。
1. 选择&#x200B;**释放空间**。

   文件或文件夹仍保留在云存储中，但它已从本地缓存中删除。

>[!NOTE]
>
>脱机文件和文件夹使用本地磁盘空间。 删除对不再需要释放空间的文件和文件夹的脱机访问。

## 将文件复制到本地存储

您可以将文件从Adobe Cloud Drive复制到本地驱动器。 原始文件保留在Adobe Cloud Drive中，副本将变为独立的本地文件。

1. 在Adobe Cloud Drive中右键单击文件。
1. 选择&#x200B;**复制**，然后将文件粘贴到本地驱动器上所需的位置。

   文件将复制到目标。 原件留在Adobe Cloud Drive中。

>[!NOTE]
>
>复制到本地存储的文件是独立的副本。 您对本地副本所做的更改不会同步回Adobe云存储。

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
