---
title: 删除工作区
description: 如果工作区不再相关，您可以将其删除。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 删除工作区

{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。 有关更多信息，请参阅 [创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md).

您可以删除不再相关的工作区。

我们建议在删除工作区之前，在其他工作区中重新创建与您要删除的工作区相关联的部分或全部记录类型、记录、字段和视图。

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
   <p> 产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>您的组织必须注册到Workfront Planning的早期访问阶段 </p>
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
   <p>新增：标准</p>
   <p>当前：计划</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*有关访问要求的详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 有关删除工作区的注意事项

* 删除工作区时，也会删除所有记录类型、记录、其字段和视图。
* 已删除的工作区及其包含的信息无法恢复。

## 删除工作区

{{step1-to-planning}}

1. 单击要删除的工作区。

   此时将显示Workspace页面。

1. 单击 **更多** 菜单 ![](assets/more-menu.png) 在工作区名称旁边，然后单击 **删除**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Type &quot;**删除**&quot;，然后单击 **永久删除**. 不区分大小写。

   工作区已被删除，无法恢复。 任何与其关联的记录类型、记录、字段和视图也会被删除。 <!--ensure this is right at or before GA-->
