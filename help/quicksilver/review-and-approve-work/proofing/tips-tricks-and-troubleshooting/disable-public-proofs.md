---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable，public，共享，proof，public，url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: 禁止通过公共URL或嵌入代码共享验证
description: 您可以关闭与公共URL共享验证或基于验证嵌入代码的功能，或关闭为个人用户共享验证的功能。
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# 禁止通过公共URL或嵌入代码共享验证

您可以关闭与公共URL共享验证或基于验证嵌入代码的功能，或关闭为个人用户共享验证的功能。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 根据验证禁用

您必须是验证所有者或创建者，或者您必须具有作者或审查方验证角色。

1. 在包含校对的项目中，单击左侧面板中的&#x200B;**文档**。
1. 将鼠标悬停在验证上并选择&#x200B;**文档详细信息** 。
1. 在左侧面板中，单击&#x200B;**验证查看器设置**，然后禁用&#x200B;**允许通过公共URL或嵌入代码共享验证**&#x200B;复选框。

   ![](assets/proofing-viewer-settings-350x200.png)

1. 单击&#x200B;**保存**。

## 为每个用户禁用

您可以在Workfront实例中为个别用户禁用公共验证设置。 您必须拥有管理员的验证权限配置文件才能进行此更改。

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**校对**。
1. 单击右上角附近的&#x200B;**帐户设置**。
1. 单击&#x200B;**用户**&#x200B;选项卡，然后单击用户的名称。
1. 在&#x200B;**默认验证设置**&#x200B;部分中，禁用&#x200B;**公共共享**&#x200B;复选框。

   ![](assets/default-proof-settings--public-sharing-350x210.png)
