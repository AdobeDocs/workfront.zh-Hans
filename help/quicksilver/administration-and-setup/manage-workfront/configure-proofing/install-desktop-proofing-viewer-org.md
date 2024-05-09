---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 为您的组织安装桌面验证查看器
description: 桌面校对查看器是必须安装在每个用户的本地计算机上的应用程序，主要用于校对交互式内容。 作为Adobe Workfront管理员或Workfront Proof管理员，您可以执行此安装。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 5cc1acffff12d78e48228f3ae223514c0ff379ef
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# 为您的组织安装桌面验证查看器

<!--Audited: 05/2024-->

桌面校对查看器是必须安装在每个用户的本地计算机上的应用程序，主要用于校对交互式内容。 作为Adobe Workfront管理员或Workfront Proof管理员，您可以执行此安装。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：Premium或Select</p> <p>有关验证不同计划的访问权限的详细信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须在验证权限配置文件中选择管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">配置用户的验证访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 系统要求

以下操作系统支持桌面校对查看器：

* Windows 7及更高版本，32位和64位
* Mac OS X 10.9及更高版本，64位

## 先决条件

要使用户能够使用桌面验证查看器，您必须配置系统以启动桌面验证查看器，作为安装之前交互式验证的默认视图。

## 将桌面校对查看器配置为交互式校对的默认查看器

为您的组织安装桌面验证查看器后，可将其设置为交互式验证的默认查看器。

{{step1-to-proofing}}

1. 单击 **帐户设置** 在Workfront Proof的右上角附近，然后单击 **设置** 选项卡。

1. 下 **校对默认值**，位于的结尾 **交互式校对的桌面校对查看器** 行，单击 **设置**.

   ![校对默认值](assets/proof-defaults.png)

1. 单击 **启用和默认**，然后单击 **保存**.

## 为用户安装桌面验证查看器

* [在Mac上安装桌面验证查看器](#installing-the-desktop-proofing-viewer-on-mac)
* [在Windows上安装桌面校对查看器](#installing-the-desktop-proofing-viewer-on-windows)

### 在Mac上安装桌面验证查看器 {#installing-the-desktop-proofing-viewer-on-mac}

1. 在用户计算机上，执行以下操作之一以下载应用程序：

   * 如果您使用的是生产环境，请单击 [适用于桌面校对查看器的Mac生产下载](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg).
   * 如果您使用的是“预览”环境，请单击 [桌面验证查看器的Mac预览下载](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg).

1. 打开您刚刚下载的文件以开始安装。
1. 在出现的安装框中，单击 **继续**，然后单击 **安装**.

   ![安装框](assets/install-wf-proof-box.png)

1. 确保每位用户都通过从Workfront的“文档”区域打开交互式验证来完成安装。

### 在Windows上安装桌面校对查看器 {#installing-the-desktop-proofing-viewer-on-windows}

1. 在用户计算机上，执行以下操作之一以下载应用程序：

   * 在生产环境中，单击 [桌面校对查看器的Windows生产下载](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe).
   * 在“预览”环境中，单击 [桌面校对查看器的Windows预览下载](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. 打开您刚刚下载的文件以开始安装。
1. 在出现的安全警告框中，单击 **运行**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   桌面校对查看器安装并运行。

1. （视情况而定）如果使用Internet Explorer安装应用程序，请在应用程序安装后刷新浏览器中的启动页面。
1. 确保每位用户都通过从Workfront的“文档”区域打开交互式验证来完成安装。
