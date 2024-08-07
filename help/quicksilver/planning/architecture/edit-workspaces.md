---
title: 编辑工作区
description: 您可以编辑现有工作区的信息，如重命名它。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 1a46fa3a8e87a5f345558cef57a4d66171320c9b
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 编辑工作区

{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。

工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。

有关创建工作区的信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

您对工作区所做的所有更改均对至少具有工作区查看权限的所有用户可见。

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
   <td> <p>Workfront Planning没有访问级别控制</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理对工作区的权限 </p>  
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

## 编辑工作区

{{step1-to-planning}}

1. （视情况而定）如果您是Workfront管理员，请单击&#x200B;**我的工作区**&#x200B;以访问您创建的工作区，或单击&#x200B;**其他工作区**&#x200B;以访问他人与您共享的工作区。<!--change it to Workspaces I'm on-->

1. 单击工作区信息卡以打开工作区。

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To edit a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **Edit**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,**********-->

1. 单击新工作区标题中工作区的名称以对其进行重命名，然后按&#x200B;**Enter**。
1. 单击标题中工作区名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**。

   ![](assets/edit-workspace-box.png)

   在&#x200B;**编辑工作区**&#x200B;框中更新以下信息：

   * 添加工作区的名称。<!--did they add a label for this field?-->
   * **描述**：添加有关工作区的信息。
   * 选择要与工作区关联的图标。

1. 单击&#x200B;**保存**&#x200B;以关闭“编辑工作区”框并应用更改。

1. （可选）要添加新工作区部分，请执行以下操作之一：

   * 单击工作区底部的&#x200B;**添加部分**。
   * 将鼠标悬停在节名称上，然后单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**添加节上方**&#x200B;或&#x200B;**添加节下方**。

1. （可选）要更改节的位置，请执行下列操作之一：

   * 将鼠标悬停在区域名称上并单击&#x200B;**抓取**&#x200B;图标![](assets/grab-icon.png)，然后将其拖放到右侧位置。
   * 将鼠标悬停在节名称上并单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**上移**&#x200B;或&#x200B;**下移**。 部分在工作区中向上或向下移动。

1. （可选）要删除工作区部分，请执行以下操作：

   1. 将鼠标悬停在节名称上，单击&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**删除**。<!--add screen shot when UI is final?-->
   1. 选择新分区以将所有记录类型移动到该分区，然后单击&#x200B;**删除**。<!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      所有记录类型都将移到选择部分，并删除该部分。

1. （可选）单击&#x200B;**添加记录类型**&#x200B;以将记录类型添加到工作区。

   有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

1. （可选）将鼠标悬停在记录类型卡片上，单击右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**&#x200B;以修改记录类型的外观。

   有关信息，请参阅[编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)。

1. （可选）将鼠标悬停在记录类型卡片上，单击右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**删除**&#x200B;以删除记录类型。

   有关信息，请参阅[删除记录类型](/help/quicksilver/planning/architecture/delete-record-types.md)。

1. （可选）按一下记录类型卡以将其拖放到新位置。 您可以将记录类型从一个工作区区域拖放到另一个工作区区域。

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （可选）单击工作区右上角的&#x200B;**共享**&#x200B;以与他人共享工作区。

   有关信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)。
