---
title: 删除工作区
description: 如果工作区不再相关，您可以将其删除。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 74db651f8865965f943bc89e58e7130cffe0c450
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 删除工作区

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

在Adobe大师中，工作区是团队计划工作的集中位置。 有关更多信息，请参阅 [创建工作区](../architecture/delete-workspaces.md).

您可以删除不再相关的工作区。

我们建议在删除工作区之前，在其他工作区中重新创建与您要删除的工作区关联的部分或全部记录类型和分类。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关删除工作区的注意事项

* 您可以删除自己或组织中的任何人已创建的任何工作区。 <!--this will change with access levels and permissions-->
* 删除工作区时，也会删除所有记录类型、分类及其字段。 <!--asked Lilit because the confirmation says the records don't delete, but not sure how they can exist outside of a workspace?!-->
* 已删除的工作区及其包含的信息无法恢复。

## 删除工作区

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 位于Workfront的右上角，或者 **主菜单** 图标 ![](assets/main-menu-shell.png)  （如果可用），然后单击 **大师** ![](assets/maestro-icon.png).

   这将打开您上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要删除的工作区。
1. 单击 **更多** 菜单 ![](assets/more-menu.png) 在工作区名称旁边，然后单击 **删除**.
1. 单击 **删除** 以确认。

   工作区已被删除，无法恢复。 任何记录类型、分类、其记录以及与它们关联的字段也会被删除。 <!--ensure this is right after closed beta-->
