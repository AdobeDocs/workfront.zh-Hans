---
title: 删除工作区
description: 如果工作区不再相关，您可以将其删除。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 删除工作区

{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。 有关详细信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

您可以删除不再相关的工作区。

我们建议在删除工作区之前，在其他工作区中重新创建与您要删除的工作区相关联的部分或全部记录类型、记录、字段和视图。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>

</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 有关删除工作区的注意事项

* 删除工作区时，也会删除所有记录类型、记录、其字段和视图。
* 已删除的工作区及其包含的信息无法恢复。

## 删除工作区

{{step1-to-planning}}

1. （视情况而定）如果您是Workfront管理员，请单击&#x200B;**我所在的工作区**&#x200B;以访问您创建的工作区，或单击&#x200B;**其他工作区**&#x200B;以访问他人与您共享的工作区。

1. （可选）单击&#x200B;**显示全部**&#x200B;以显示其他工作区。 仅当您拥有两行以上的工作区信息卡时，才会显示&#x200B;**显示所有**&#x200B;链接。
1. （可选） ClicK **显示更少**&#x200B;以限制屏幕上显示的工作区数。
1. 要删除工作区，请执行下列操作之一：

   * 将鼠标悬停在工作区信息卡上，然后单击该信息卡右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)
或
   * 单击工作区卡以打开工作区，然后单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)。
1. 单击&#x200B;**删除**。

   ![](assets/permanently-delete-workspace-confirmation.png)

1. 在提供的空间中键入“**delete**”，然后单击&#x200B;**永久删除**。 不区分大小写。

   工作区已被删除，无法恢复。 任何与其关联的记录类型、记录、字段和视图也会被删除。<!--ensure this is right at or before GA-->
