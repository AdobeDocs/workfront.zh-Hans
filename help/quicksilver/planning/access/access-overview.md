---
title: Adobe Workfront规划访问概述
description: 并非组织中的所有用户都具有相同的访问权限和权限来使用Adobe Workfront Planning。 本文介绍了用户使用Adobe Workfront Planning功能时可能拥有的访问权限和权限。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QuLxjUMlRgN0FvlDwR0JVQ-m-wV-z3C6sh30lJYRKfU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ab0d036ea3bbcdad2daaed6b09864272fd1beb11
workflow-type: tm+mt
source-wordcount: 1010
ht-degree: 1%

---

# Adobe Workfront Planning访问概述

<!--do not use the snippet for IMPORTANT , as it links to this article-->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning。 Workfront Planning是独立的产品，或者是Adobe Workfront另外购买的功能。
>
>
>本文包含有关客户同时购买Workfront或Workflow包时Workfront Planning的一般信息。
>
>有关包含Workfront Planning文档的文章的完整列表，请参阅[Adobe Workfront Planning的一般信息和文章索引](/help/quicksilver/planning/planning-information.md)。
>
>有关Workfront Planning作为独立产品的信息，请参阅[Adobe Workfront Planning作为独立产品入门](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。

本文介绍了使用Workfront Planning功能所需的访问权限和设置。

## 访问权限要求

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

您必须具有以下权限才能使用Workfront Planning：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
   <tr>
   <tr>
   <td role="rowheader"><p>Adobe Workfront 包</p></td>
   <td>
   <p>任何Workfront或工作流计划包
   和任何Workfront规划包</p>
   <p><b>注释</b></p>
   <p>要访问可连接的记录类型，请执行以下操作：</p>
   <ul><li><p>任何Workfront包和规划包</p></li>
   <li><p>任何工作流和计划Prime和Ultimate包</p></li></ul>

<p>要访问全局记录类型，请执行以下操作：</p>
   <ul><li><p>任何Workfront包和Planning Plus包</p></li>
   <li><p>任何工作流包以及计划Prime和Ultimate包</p></li></ul> </td></tr>
   <!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
   </tr>
   -->
   <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <ul><li><p>任何工作流和任何Planning许可证，用于查看Workfront Planning信息</p></li>
   <li><p>工作流标准和计划标准，用于创建工作区和视图</p></li></ul>
    </td>
   </tr>
   <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>访问级别的任何工作流和任何Planning许可证类型</p>  
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <ul>
   <li><p>查看您未创建的工作区、记录类型和视图的更高权限，以访问它们及其对象。</p></li>
   <li><p>向工作区和记录类型分配或更高权限，而您未创建这些工作区和记录类型以编辑它们，以及创建、编辑或删除记录类型。</p></li>
   <li><p><span class="preview">管理编辑、共享或删除记录的权限。</p>
   <li><p>为您未创建的视图贡献或更高权限，以便编辑、删除和共享这些视图</p>
   </li>
    <li><p>Planning管理员可以管理他们未创建的工作区。 </p></li>
    <li><p>Planning管理员无法访问他们未创建的视图。 </p></li></ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 
   <p>Planning Standard用户和管理员默认启用Planning区域。</p>
   <p> 必须为具有工作流指示灯或Planning参与者许可证的用户分配一个布局模板，该模板包括以下区域中的Planning选项：</p>
   <ul><li>主菜单</li>
   <li>项目、项目组合和程序的左侧面板</li>
   </ul>   
   </td>
  </tr>
 </tbody>
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


## Workfront Planning访问级别和许可证

当用户以管理员身份添加到Adobe Admin Console时，可为用户分配Planning管理员许可证。

有关信息，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。

您不能在Workfront Planning中修改Planning管理员访问级别。

在Workfront中配置访问级别时，您可以分配以下许可证类型：

* 工作流许可证类型
* Planning许可证类型

用户必须同时具有分配至其访问级别的许可证类型才能访问Workfront Planning。

您可以将以下Planning许可证分配给访问级别：

* **Planning Standard**：如果用户需要创建和管理所有Planning对象，而不需要成为管理员，则授予用户此访问权限。
* **Planning参与者**：如果用户需要贡献到记录，但不需要创建Planning对象，则授予用户此访问权限。

  >[!TIP]
  >
  >如果您的组织购买的工作流和规划许可证数量不等，则规划参与者许可证类型不可用。


* **无**：在分配此Planning许可证类型时，将专门删除分配给此访问级别用户的所有Planning访问权限。

  >[!IMPORTANT]
  >
  >规划许可证和工作流许可证可协同工作，以授予用户访问Workfront的权限。
  >
  >您可以在Workflow和Planning之间为用户授予不同级别的访问权限，但Workflow许可证不得低于Planning许可证。
  >
  >例如，您可以为用户提供Workflow Standard许可证和Planning Contributor许可证，但不能为他们提供Workflow Contributor许可证和Planning Standard许可证。
  >
  >如果用户必须访问工作流或Planning，则工作流许可证类型不能为空。

有关详细信息，请参阅使用Adobe Workfront Planning时的[许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。

## 配置访问级别

有关在Workfront中配置访问权限的信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

## 向用户分配许可证

您可以在编辑或创建用户时为其分配访问级别，从而为其分配许可证。

有关信息，请参阅[编辑用户配置文件](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 授予权限

您可以在Workfront Planning中向以下实体授予权限：

* 工作区
* 记录类型
* 视图
* 记录

有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

您的Adobe Workfront许可证类型与Workfront Planning许可证类型和Planning权限配合使用，可让您查看、贡献或管理Workfront Planning对象。

有关许可证类型如何影响Workfront Planning对象权限级别的信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。

## 使用布局模板共享Planning区域

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

默认情况下，标准用户和系统管理员在以下区域中启用Planning区域：

* 主菜单
* 项目、项目组合或项目的左侧面板

如果您拥有任何其他Workfront许可证并且需要对Workfront规划工作做出贡献，您的系统管理员必须将Planning区域添加到您。

管理员可以通过修改布局模板并将您分配给该模板，将Planning选项添加到以下区域：

* 主菜单
* 登陆页面
* 项目、项目组合和项目的左侧面板
* 固定

要从Workfront实例的用户中添加或删除Workfront Planning区域，请执行以下操作：

1. 以Workfront管理员身份登录到&#x200B;**Workfront**。

1. 转到&#x200B;**主菜单** > **设置** > **界面** > **布局模板**，然后打开或创建布局模板。

   有关自定义布局模板的信息，请参阅[创建和管理布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

1. 将布局模板分配给要访问Workfront Planning的用户。

   有关信息，请参阅[将用户分配给布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

   现在，分配给模板的所有用户都可以在他们的主菜单中访问Workfront Planning。

   用户可以开始创建工作区、记录类型、记录和字段。


