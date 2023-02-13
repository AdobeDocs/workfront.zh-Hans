---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: 禁用，公共，共享，校样，公共，url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 禁用通过公共URL或嵌入代码共享校样
description: 您可以关闭与公共URL共享校样或按校样基础为用户或个人用户嵌入代码的功能。
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# 禁用通过公共URL或嵌入代码共享校样

您可以关闭与公共URL共享校样或按校样基础为用户或个人用户嵌入代码的功能。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 按校样禁用

您必须是校样的所有者或创建者，或者您必须具有“作者”或“审核者”校样角色。

1. 在包含校样的项目中，单击 **文档** 中。
1. 将鼠标悬停在校样上并选择 **文档详细信息** .
1. 在左侧面板中，单击 **校对查看器设置**，然后禁用 **允许通过公共URL或嵌入代码共享校样** 复选框。

   ![](assets/proofing-viewer-settings-350x200.png)

1. 单击&#x200B;**保存**。

## 按用户禁用

您可以为Workfront实例中的各个用户禁用公共校样设置。 您必须具有管理员的校样权限配置文件才能进行此更改。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **校对**.
1. 单击 **帐户设置** 在右上角附近。
1. 单击 **用户** 选项卡，然后单击用户的名称。
1. 在 **默认校样设置** 部分，禁用 **公共共享** 复选框。

   ![](assets/default-proof-settings--public-sharing-350x210.png)
