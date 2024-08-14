---
title: 创建工作区
description: 工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。 记录类型按工作区中的部分组织。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: f252140e4fec01c7bb8092804532d79954cef618
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 创建工作区

{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。

工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。

有关工作区的一般信息，请参阅[工作区概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

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
   或
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
   <td> <p>您将获得所创建工作区的管理权限。 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您必须将Planning区域添加到布局模板中。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

有关访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 创建 Workspace

您可以创建一个工作区并向其中添加记录类型，以便在Workfront Planning中组织对象。 有关编辑工作区的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

{{step1-to-planning}}

1. 单击&#x200B;**创建工作区**

   此时会显示“创建工作区”框。 您可以从头开始创建工作区，也可以使用某个可用模板创建工作区。

1. （可选且有条件）单击以下任何预定义Workspace模板中的&#x200B;**预览**：

   * 基本：营销管理
   * 高级：营销管理
   * 企业：营销管理
   * 销售管理
   * 产品管理

   模板预览框打开。

   指示与每个模板关联的操作记录类型、分类以及字段数。

   ![](assets/previewing-a-workspace-template.png)

   有关Workfront Planning工作区模板的信息，请参阅[工作区模板列表](/help/quicksilver/planning/architecture/workspace-templates.md)。

1. 在模板预览框中，单击&#x200B;**使用模板**&#x200B;以开始从所选模板创建工作区

   或

   单击&#x200B;**上一步**，然后单击&#x200B;**新建工作区**&#x200B;从头开始创建工作区。

   将创建以下工作区类型之一：

   * 一个名为&#x200B;**无标题Workspace**&#x200B;的空工作区，您可以在其中开始手动添加记录类型，以便从头开始创建工作区。
   * 以您选择的模板命名的工作区，该模板填充了示例记录类型。 您可以进一步自定义记录类型和工作区。

   对于Workfront管理员，新工作区显示在&#x200B;**我的工作区**&#x200B;选项卡上。<!--replace this with: **Workspaces I'm on** tab-->
1. 单击新工作区标题中工作区的名称以对其进行重命名，然后按Enter键。

1. （可选且有条件）如果是从模板创建工作区，请单击&#x200B;**操作记录类型**&#x200B;或&#x200B;**分类**&#x200B;部分的名称

   或

   将鼠标悬停在节名称上，单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**重命名**&#x200B;以重命名节。

   >[!TIP]
   >
   >您可以从任何工作区重命名任何分区，即使您未创建该分区也是如此。

   有关编辑工作区（包括编辑工作区节）的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （可选）单击&#x200B;**添加记录类型**&#x200B;以将记录类型添加到任意节中的工作区。

   有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   有关在工作区中编辑和删除记录类型的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。


