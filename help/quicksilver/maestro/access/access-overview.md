---
title: 访问概述
description: 组织中的所有用户都可以访问AdobeMaestro。 目前，没有与用户或Maestro中的信息相关的访问级别或权限。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 50e6b09d626325ee2836dc0ebaf79fc1e8cc9da9
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 1%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

# 访问概述

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能访问Maestro。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

AdobeMaestro没有访问级别限制。

您组织中的所有用户都可以访问Maestro，无论其访问级别如何。

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

## 访问要求

您必须具备以下条件才能使用Adobe经理：

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
<p>贵公司必须注册AdobeMaestro封闭测试版计划。  </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别</p></td>
   <td> <p>任何</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront管理员必须添加主菜单中的Maestro区域到布局模板。</p> 
   <p>有关信息，请参阅 <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">使用布局模板自定义主菜单</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--After we enable permissions, replace the section content above with this:

There are license and sharing permission restrictions to use Adobe Maestro capabilities. (*********** this should be the intro right under the title; also update the metadata with this when live*******)

You must have the following settings to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement*</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p>
   To create workspaces, users must have the following license: 
   <ul><li><p>New: Standard</p> </li>
   <li><p>Current: Worker or higher</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro objects</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>Contribute or higher permissions to workspaces and views that you did not create to edit, delete, and share them</p>
    <p>System Administrators can manage workspaces and views they did not create </p>
   <p>For information about sharing permissions for Maestro objects, see  
   <a href="../access/sharing-permissions-overview.md">Overview of sharing permissions in Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your system administrator must add the Maestro area in the Main Menu to your layout template.</p> 
   <p>For information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Customize the Main Menu using a layout template</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*To find out your Workfront plan, license, or access level, contact your Workfront administrator. 

-->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


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

## 授予权限

没有与Maestro对象关联的权限。

所有在其环境中启用了Maestro的用户都可以查看、编辑和删除任何其他用户添加到Maestro的所有信息。

<!--
Take out the text above and replace with this: 

For more information, see [Access overview](/help/quicksilver/maestro/access/access-overview.md)-->


