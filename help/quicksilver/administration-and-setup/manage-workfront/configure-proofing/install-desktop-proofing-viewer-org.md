---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 为贵组织安装桌面校对查看器
description: 桌面校对查看器主要用于校对交互式内容，它是必须安装在每个用户本地计算机上的应用程序。 作为Adobe Workfront管理员或Workfront校样管理员，您可以执行此安装。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: c89b21c6-fe70-4f46-aebd-5b82a667db72
source-git-commit: 58f976d9f4245e528a4ddf23d39b92d9fa405311
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---

# 为贵组织安装桌面校对查看器

桌面校对查看器主要用于校对交互式内容，它是必须安装在每个用户本地计算机上的应用程序。 作为Adobe Workfront管理员或Workfront校样管理员，您可以执行此安装。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium或Select</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须在校样权限配置文件中选择管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">配置用户的校对访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 系统要求

以下操作系统支持桌面校对查看器：

* Windows 7及更高版本、32位和64位
* Mac OS X 10.9及更高版本，64位

## 先决条件

要使用户能够使用桌面校对查看器，您必须

* 将系统配置为在安装之前启动桌面校样查看器，以将其作为交互式校样的默认视图。

## 将桌面校对查看器配置为交互式校样的默认查看器

为组织安装桌面校对查看器后，可以将其设置为交互式校样的默认查看器。

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。

1. 单击 **帐户设置** 在Workfront校样的右上角附近，单击 **设置**&#x200B;选项卡。

1. 在 **校样默认值**，在 **用于交互式校样的桌面校样查看器** 行，单击 **设置**.

   ![](assets/proof-defaults-350x265.png)

1. 单击 **启用和默认**，然后单击 **保存**.

## 为用户安装桌面校对查看器

* [在Mac上安装桌面校对查看器](#installing-the-desktop-proofing-viewer-on-mac)
* [在Windows上安装桌面校对查看器](#installing-the-desktop-proofing-viewer-on-windows)

### 在Mac上安装桌面校对查看器 {#installing-the-desktop-proofing-viewer-on-mac}

1. 在用户的计算机上，执行以下操作之一以下载应用程序：

   * 如果您使用的是生产环境，请单击  [Mac桌面校样查看器的Production Download。](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof-2.1.19.pkg)
   * 如果您使用预览环境，请单击  [Mac预览桌面校样查看器的下载。](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview-2.1.19.pkg)
)

1. 打开刚下载的文件以开始安装。
1. 在显示的安装框中，单击 **继续**，然后单击 **安装**.

   ![00000776.png](assets/00000776-350x244.png)

1. 确保每个用户都通过从Workfront的“文档”区域打开一个交互式校样来完成安装。

### 在Windows上安装桌面校对查看器 {#installing-the-desktop-proofing-viewer-on-windows}

1. 在用户的计算机上，执行以下操作之一以下载应用程序：

   * 在生产环境中，单击 [桌面校样查看器的Windows Production下载。](https://assets.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Setup+2.1.19.exe)
   * 在“预览”环境中，单击 [桌面校样查看器的Windows预览下载](https://assets.preview.proofhq.com/nativeviewer/desktop_viewer/Workfront+Proof+Preview+Setup+2.1.19.exe).

1. 打开刚下载的文件以开始安装。
1. 在出现的安全警告框中，单击 **运行**.

   ![Screen_Shot_2018-05-02_at_10.56.55_AM.png](assets/screen-shot-2018-05-02-at-10.56.55-am-350x271.png)

   桌面校样查看器安装并运行。

1. （视情况而定）如果您使用Internet Explorer安装应用程序，则在安装应用程序后在浏览器中刷新启动页面。
1. 确保每个用户都通过从Workfront的“文档”区域打开一个交互式校样来完成安装。
