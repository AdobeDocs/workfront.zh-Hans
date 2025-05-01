---
title: Adobe Workfront规划访问概述
description: 并非组织中的所有用户都具有相同的访问权限和权限来使用Adobe Workfront Planning。 本文介绍了用户使用Adobe Workfront Planning功能时可能拥有的访问权限和权限。
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 2%

---


# Adobe Workfront Planning访问概述

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning，它是Adobe Workfront的一项附加功能。
>
>贵公司必须购买Workfront Planning的附加许可证才能访问其功能。
>
>有关更多信息，请与您的客户经理联系
>
>有关Workfront Planning的更多信息，请参阅[Adobe Workfront Planning概述](/help/quicksilver/planning/general/planning-overview.md)。

使用Adobe Workfront Planning时，存在许可证和共享权限限制。

本文介绍了使用Workfront Planning功能所需的访问和设置。

## 访问要求

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

您必须具有以下权限才能访问Workfront Planning：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront规划<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront计划*</p></td>
   <td>
<p>以下任意Workfront计划：</p>
<ul><li>选择</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning不适用于旧版Workfront计划</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td>
   <td>
<p>以下任意Workfront规划计划：</p>
<ul><li>规划中</li>
<li>Planning Plus</li>
</ul>
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <ul><li><p>用于查看Workfront Planning信息的标准、浅色或参与者</p></li>
   <li><p>标准，用于创建工作区和视图</p></li></ul>
   <p>Workfront计划不适用于旧版Workfront许可证</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <ul>
   <li><p>查看对工作区、<span class="preview">记录类型</span>以及您未创建用于访问它们及其对象的视图的更高权限。</p></li>
   <li><p>向工作区<span class="preview">和记录类型</span>提供或更高权限，您未创建这些类型来编辑它们，创建、编辑或删除记录类型和记录。</p></li>
   <li><p>为您未创建的视图贡献或更高权限，以便编辑、删除和共享这些视图</p>
   </li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    <li><p>系统管理员无法访问他们未创建的视图。 </p></li></ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> <div class="preview">
<p>默认情况下，标准用户和系统管理员已启用Planning区域。</p>
<p> 必须为具有轻度或参与者许可证的用户分配一个布局模板，该模板包括以下区域的Planning选项：</p>
   <ul><li>主菜单</li>
   <li>项目、项目组合和程序的左侧面板</li>
   </ul>
   <p>有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">创建和管理布局模板</a>。</p>
   </div>
   <p><b>注释</b></p>
   <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning区域的布局模板。</p>
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。






## 使用布局模板共享Planning区域

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

在贵组织购买了其他Workfront Planning许可证后，系统管理员可以通过修改布局模板并将其分配给您，将Planning选项添加到以下区域：

* 主菜单
* 登陆页面
* 项目、项目组合和项目的左侧面板
* 固定

<div class="preview">

默认情况下，标准用户和系统管理员在以下区域中启用Planning区域：

* 主菜单
* 项目、项目组合或项目的左侧面板

</div>

要添加<span class="preview">或从Workfront实例的用户中删除</span>个Workfront Planning区域，请执行以下操作：

1. 以Workfront管理员身份登录到&#x200B;**Workfront**。

1. 转到&#x200B;**主菜单** > **设置** > **界面** > **布局模板**，然后打开或创建布局模板。

   有关自定义布局模板的信息，请参阅[创建和管理布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

1. 将布局模板分配给要访问Workfront Planning的用户。

   有关信息，请参阅[将用户分配给布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

   现在，分配给模板的所有用户都可以在他们的主菜单中访问Workfront Planning。

   用户可以开始创建工作区、记录类型、记录和字段。

## 授予访问权限

Workfront Planning没有Workfront访问控制。

拥有任何类型的Workfront许可证的用户都可以访问Workfront Planning。

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 授予权限

您必须向用户授予Workfront Planning工作区和您为其创建的视图的权限才能访问它们。

有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

您的Adobe Workfront许可证类型与Workfront Planning权限配合使用，可让您查看、贡献或管理Workfront Planning对象。

有关许可证类型如何影响Workfront Planning对象权限级别的信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。


