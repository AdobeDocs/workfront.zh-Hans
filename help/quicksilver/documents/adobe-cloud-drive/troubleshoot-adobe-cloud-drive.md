---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: adobe-cloud-drive
title: Adobe Cloud Drive疑难解答
description: 查看Mac和Windows上Adobe云驱动器的限制、性能注意事项以及常见问题的解决方案。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6ad89f8d00dd3a06eb160863c3213a9f80b1a44b
workflow-type: tm+mt
source-wordcount: 928
ht-degree: 0%

---

# Adobe Cloud Drive疑难解答

本文介绍了Adobe Cloud Drive的限制、要牢记的性能注意事项，以及您可能遇到的常见问题的解决方案。

有关使用Adobe云驱动器的信息，请参阅[使用Adobe云驱动器](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)。

## 限制

### 文件和文件夹操作

* 项目文件夹在顶级为只读。 您无法从Adobe Cloud Drive中重命名、删除或移动这些驱动器。 要创建、重命名或删除项目，请使用Workfront Web界面。
* 完全支持在项目文件夹中进行文件和文件夹操作。

### 文件和路径限制

* 文件名在任何平台上不能超过255个字符。
* 完整文件路径（所有文件夹名称加上文件名）不能超过1024个字符。 路径长于此限制的文件不会显示在Adobe Cloud Drive中，即使它们在Workfront Web界面中可见。
* 如果您在文件中看到&#x200B;**完整路径太长**&#x200B;错误，请缩短文件夹名称或减少文件夹嵌套深度，以将路径限制在限制范围内。

### 存储

* 保存在Adobe云驱动器中的文件会本地使用设备上的磁盘空间。
* 仅云文件不使用本地存储。
* 删除不再需要的文件的脱机访问权限。 有关详细信息，请参阅[使用Adobe云驱动器](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)中的[删除脱机访问以释放空间](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#remove-offline-access-to-free-up-space)。

## 性能注意事项

* **文件大小：**&#x200B;同步所需的时间取决于文件大小。 大型文件通常需要较长时间。
* **网络速度：**&#x200B;更快的连接可提供更好的同步性能。 同步会在中断后自动恢复。
* **首次访问：**&#x200B;首次访问时按需下载的文件。 后续访问速度更快，因为文件缓存在本地。

## 常见问题

### Adobe Cloud Drive未出现

**可能的原因：**

* 未安装Adobe Cloud驱动器。
* 安装未成功完成。
* 您的组织未使用支持Adobe云存储的Workfront版本。

**解决方案：**

* 验证是否已安装Adobe Cloud驱动器。 检查&#x200B;**应用程序** (Mac)或&#x200B;**程序** (Windows)。
* 手动启动Adobe云驱动器。
* 请联系您的Workfront管理员，以确认您的组织使用的是支持Adobe云存储的Workfront版本。
* 如有必要，请重新安装Adobe Cloud Drive。 有关详细信息，请参阅[安装Adobe云驱动器](/help/quicksilver/documents/adobe-cloud-drive/install-adobe-cloud-drive.md)。

### Adobe Cloud驱动器图标在菜单栏或任务栏中不可见

**可能的原因：**

* 菜单栏(Mac)或系统任务栏(Windows)没有足够的空间显示该图标。

**解决方案：**

* **Mac：**&#x200B;按住Cmd并拖动现有菜单栏图标以重新排列或移除它们，从而为Adobe Cloud Drive图标创建空间。
* **Windows：**&#x200B;单击任务栏中的向上箭头（**显示隐藏图标**）以查找Adobe Cloud Drive图标，然后将其拖动到可见区域。

### 项目未显示或缺少某些项目

**可能的原因：**

* 您无权访问任何项目。
* 同步尚未完成。
* 您遇到网络连接问题。

**解决方案：**

* 在Workfront Web界面中验证您对项目的访问权限。
* 检查网络连接。
* 注销Adobe Cloud Drive并重新登录。

### 文件未同步

**可能的原因：**

* 您遇到网络连接问题。
* 文件或文件夹存在同步错误。
* 磁盘空间不足。

**解决方案：**

* 检查互联网连接。
* 验证您是否有足够的可用磁盘空间。
* 检查文件状态指示器是否显示同步错误。 有关详细信息，请参阅[使用Adobe云驱动器](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md)中的[文件状态指示器](/help/quicksilver/documents/adobe-cloud-drive/use-adobe-cloud-drive.md#file-status-indicators)。
* 重新启动Adobe Cloud Drive。
* 在系统任务栏(Windows)或菜单栏(Mac)中检查Adobe云驱动器状态。

### 无法打开文件

**可能的原因：**

* 该文件为仅云文件，下载失败。
* 未安装打开文件所需的应用程序。
* 文件已损坏。

**解决方案：**

* 检查文件状态指示器。
* 确保安装了所需的应用程序。
* 右键单击文件，选择&#x200B;**始终保留在此设备上**，然后再次尝试打开它。
* 验证Workfront Web界面中的文件是否未损坏。

### 同步缓慢

**可能的原因：**

* 文件很大。
* 网络连接速度慢。
* 正在同步多个文件。

**解决方案：**

* 请耐心地处理大文件。 同步可恢复，因此它会在中断后从中断处恢复。
* 检查您的网络速度。
* 限制同时执行文件操作的次数。
* 除非您需要脱机访问，否则仅将大文件保留在云中。

### 脱机文件占用太多空间

**解决方案：**

* 右键单击脱机文件并选择&#x200B;**释放空间**。
* 请定期检查您的磁盘空间。
* 保留您很少在仅云模式下访问的大型文件。

### 无法创建、编辑或删除文件或文件夹

**可能的原因：**

* 您正在尝试创建、重命名或删除项目文件夹。 项目文件夹在顶级为只读。
* 对于您而言，该项目是只读的，因此您无法创建、编辑或删除其中的文件或文件夹。

**解决方案：**

* 要创建、重命名或删除项目，请使用Workfront Web界面。
* 要求项目所有者与您共享项目，并具有编辑权限。

## 获取帮助

有关许可证问题、项目访问问题或特定于组织的配置，请与Workfront管理员联系。

要与Adobe支持共享日志，请按照[运行Adobe日志收集器工具](https://helpx.adobe.com/cn/creative-cloud/apps/troubleshoot/diagnostics-repair-tools/run-log-collector-tool.html)中的步骤操作。

## 最佳做法

* **计划脱机工作。** 在旅行或在连通性差的地区工作之前下载文件。
* **监视器同步状态。** 在关闭应用程序之前，请检查文件指示器。
* **遵循项目的文件夹结构。** 按照项目所有者的意愿组织项目文件夹中的文件。
* **使用描述性文件名。** 帮助您的团队成员找到他们需要的内容。
* **避免创建重复项。** 不要为文件制作不必要的副本。
