---
title: 授予对Adobe大师的访问权限
description: 了解如何在Adobe大师中授予访问权限和共享信息。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 85f499a429d4223c62b7b13dc0b1d10e8e79e9ed
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# 授予对Adobe大师的访问权限

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能访问Maestro
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

贵组织的所有用户都可以访问Maestro，前提条件如下：

<!--the first requisite will be removed when we go to GA-->

* 贵公司已注册AdobeMaestro封闭测试版计划。
* 作为系统管理员，必须使用布局模板将Maestro区域添加到主菜单。

  默认情况下，任何用户（包括系统管理员）都不会在主菜单中显示Maestro。

  有关信息，请参阅 [使用布局模板自定义主菜单](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>没有与用户或Maestro中的信息关联的访问级别或权限。 所有在其环境中启用了Maestro的用户都可以查看、编辑和删除任何其他用户添加到Maestro的所有信息。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>任何使用Maestro</p>
   <p>系统管理员或计划在布局模板中共享Maestro区域</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须将Maestro区域添加到您的布局模板中。 </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

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

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->