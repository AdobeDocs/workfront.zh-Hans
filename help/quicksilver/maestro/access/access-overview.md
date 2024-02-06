---
title: 访问概述
description: 使用Adobe专家功能时，存在许可证和共享权限限制。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# 访问概述

{{maestro-important-intro}}

使用Adobe专家功能时，存在许可证和共享权限限制。

## 访问要求

您必须具有以下设置才能使用Adobe经理：

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>任何</p>
   <p>要创建工作区，您必须具有以下许可证：</p>
   <ul>
   <li>
   新增：标准
   </li>
   <li>
   当前：工作人员或更高版本
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro对象没有访问级别控制</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>对象权限</p></td>
   <td>
   <p>为您未创建的工作区和视图分配或更高权限，以便编辑、删除和共享它们，以及创建、编辑或删除记录类型和记录。</p>
    <p>系统管理员可以管理他们未创建的工作区和视图 </p>
   <p>有关共享Maestro对象权限的信息，请参阅  
   <a href="../access/sharing-permissions-overview.md">在Adobe大师中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的Maestro区域。 </p> <p>有关信息，请参阅 <a href="/help/quicksilver/maestro/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 与他人共享主菜单中的大师区域

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

贵组织在注册Maestro测试版计划后，可以使用版面模板将Maestro区域添加到所有用户的主菜单。

1. 登录 **Workfront** Workfront管理员。

1. 添加 **大师** 图标 ![](assets/maestro-icon.png) 到 **主菜单** 使用 **布局模板**.

   有关信息，请参阅 [使用布局模板自定义主菜单](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. 将布局模板分配给要访问Maestro的用户。

   有关信息，请参阅 [将用户分配给布局模板](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   现在，分配给模板的所有用户都可以在他们的主菜单中访问Maestro。

   用户可以开始创建工作区、记录类型、记录和字段。

## 授予访问权限

Maestro没有访问控制。

拥有任何许可证类型的用户可以访问Maestro。

有关在Workfront中授予访问权限的信息，请参阅 [创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 授予权限

您必须向非系统管理员用户授予您创建的工作区和视图的权限，以便他们能够访问这些工作区和视图。

有关更多信息，请参阅 [在Adobe大师中共享权限概述](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

您的Adobe Workfront许可证类型与您的Maestro权限配合使用，授予您查看、贡献或管理Maestro对象的权限。

有关许可证类型如何影响Maestro对象权限级别的信息，请参阅 [Adobe大师中的许可证类型概述](/help/quicksilver/maestro/access/license-type-overview.md).


