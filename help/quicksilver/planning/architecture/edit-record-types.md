---
title: 编辑记录类型
description: 保存记录类型后，您可以对其进行编辑。 记录类型是Adobe Workfront Planning的对象类型。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 编辑记录类型

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 您可以编辑您或其他人创建的记录类型的外观。 有关创建Workfront Planning记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

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
   <p> Adobe Workfront</p> <p>要将Adobe Workfront Planning记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console。</p> </td>
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
   <td> <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>只有系统管理员才能启用记录类型以从其他工作区连接</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅<a href="/help/quicksilver/planning/access/access-overview.md">访问概述</a>。 </p>  
</td>
  </tr>

</tbody>
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 编辑记录类型

{{step1-to-planning}}

1. 单击要编辑其记录类型的工作区，

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**
或
   * 单击记录类型卡以打开记录类型页面，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**编辑**。

   ![](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**编辑记录类型**&#x200B;框中，**外观**&#x200B;选项卡默认打开。

   ![](assets/edit-record-type-box-appearance-tab.png)

   在&#x200B;**外观**&#x200B;选项卡中更新以下信息：

   * 根据需要编辑记录类型名称。<!--did they add a field label for this?-->
   * **描述**：编辑或添加记录类型的描述，其中包含有关该记录类型的详细信息。
   * 编辑与记录类型关联的图标的颜色和形状。 执行以下操作：
      * 选择用于标识记录类型的颜色。 这是记录类型图标的颜色。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

1. （视情况而定）如果您是系统管理员，请单击&#x200B;**编辑记录类型**&#x200B;框中的&#x200B;**高级设置**&#x200B;选项卡。

   ![](assets/edit-record-type-box-advanced-settings-tab.png)

1. （视情况而定）作为系统管理员，在&#x200B;**高级设置**&#x200B;选项卡中更新以下信息：

   * **从其他工作区连接**：选择此切换可允许用户从其他工作区连接到此记录类型。 默认情况下，该选项处于取消选中状态。
   * **系统范围**：选择此选项可允许用户从系统中的所有工作区连接到此记录。
   * **特定工作区**：选择此选项可限制用户可以从中连接到此记录类型的工作区，然后展开下拉菜单并选择您希望用户从中连接到此记录类型的工作区。 您可以开始键入工作区的名称，并在工作区显示在列表中时将其选定。

1. 单击&#x200B;**保存**。

   工作区上的记录类型卡片在右上角显示一个连接图标![](assets/connect-from-other-workspaces-icon.png)，表示现在可以从其他工作区访问该记录。

1. （可选）单击工作区区域中的记录类型卡以打开记录类型的页面，然后重命名标题中的记录类型。

1. （可选）要编辑其他记录类型，请从记录类型页面中，展开记录类型名称右侧的向下箭头，搜索记录类型，然后在记录类型显示在列表中时将其选定。

   ![](assets/record-type-drop-down-on-record-type-page-with-search-box.png)