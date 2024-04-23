---
title: 编辑工作区
description: 您可以编辑现有工作区的信息，如重命名它。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# 编辑工作区

{{maestro-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。

工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。

有关创建工作区的信息，请参见 [创建工作区](/help/quicksilver/maestro/architecture/create-workspaces.md).

您对工作区所做的所有更改均对至少具有工作区查看权限的所有用户可见。

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
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>您必须将Planning区域添加到布局模板中。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

有关访问要求的详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 编辑工作区

{{step1-to-maestro}}

这将打开Workfront Planning的“工作区”区域。

1. 单击新工作区标题中工作区的名称以对其进行重命名，然后按键 **输入**.
1. 单击 **更多** 菜单 ![](assets/more-menu.png)工作区名称右侧，然后单击 **编辑**.

   ![](assets/edit-workspace-box.png)

   在中更新以下信息 **编辑工作区** 框：

   * 添加工作区的名称。 <!--did they add a label for this field?-->
   * **描述**：添加有关工作区的信息。
   * 选择要与工作区关联的图标。

1. 单击 **保存** 以关闭“编辑工作区”框并应用更改。

1. （可选）要添加新工作区部分，请执行以下操作之一：

   * 单击 **添加分区** 位于工作区的底部。
   * 将鼠标悬停在区域名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **添加以上部分** 或 **在下面添加部分**.

1. （可选）要更改节的位置，请执行下列操作之一：

   * 将鼠标悬停在区域名称上，然后单击 **抓取** 图标 ![](assets/grab-icon.png)，然后将其拖放到右侧。
   * 将鼠标悬停在区域名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **上移** 或 **下移**. 部分在工作区中向上或向下移动。

1. （可选）要删除工作区部分，请执行以下操作：

   1. 将鼠标悬停在区域名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **删除**. <!--add screen shot when UI is final?-->
   1. 选择新分区以将所有记录类型移动到该分区，然后单击 **删除**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      所有记录类型都将移到选择部分，并删除该部分。

1. （可选）单击 **添加记录类型** 向工作区添加记录类型。

   有关信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

1. （可选）将鼠标悬停在记录类型卡片上，单击 **更多** 菜单 ![](assets/more-menu.png) 图标，然后单击 **编辑** 修改记录类型的外观。

   有关信息，请参阅 [编辑记录类型](/help/quicksilver/maestro/architecture/edit-record-types.md).

1. （可选）将鼠标悬停在记录类型卡片上，单击 **更多** 菜单 ![](assets/more-menu.png) 图标，然后单击 **删除** 删除记录类型。

   有关信息，请参阅 [删除记录类型](/help/quicksilver/maestro/architecture/delete-record-types.md).

1. （可选）单击视图选项卡中的视图名称以编辑现有视图，或单击 **+视图** 创建视图。

   有关信息，请参阅 [管理记录视图](/help/quicksilver/maestro/views/manage-record-views.md).

1. （可选）单击 **共享** （位于工作区的右上角）与他人共享工作区。

   有关信息，请参阅 [共享工作区](/help/quicksilver/maestro/access/share-workspaces.md).
