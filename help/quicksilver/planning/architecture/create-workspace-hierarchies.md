---
title: 创建Workspace层级
description: 作为工作区管理员，您可以在Adobe Workfront Planning中的记录类型之间创建多个工作区层次结构。 在工作区中连接记录类型并创建层级后，记录类型会相互连接，其中一个记录类型指定为父级，而最多6个其他记录类型配置为子级。
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# 创建工作区层次结构

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以在Adobe Workfront Planning中的记录类型之间创建多个工作区层次结构。

在工作区中连接记录类型后，您可以创建一个层次结构来组织这些连接。 层次结构将记录和对象类型组织为父子关系，最多可以包含四个级别的对象类型。

如果两个记录类型之间的连接尚不存在，则可以在设置层次结构时创建该连接。 定义后，该层级将在工作区内的相关记录类型之间建立结构化路径。

层次结构将为记录类型及其各自的记录<!--ensure this is the case: does the breadcrumb show for both the RT and the record??-->生成痕迹导航，这些记录类型及其各自的记录将显示在其标题中。 这样，用户就可以在工作流的任何阶段了解自己在层级中的位置。

有关层次结构和痕迹导航的一般信息，请参阅[层次结构和痕迹导航概述](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md)。

## 访问权限要求

<!--check the access to see if you oversimplified???-->

+++ 展开以查看访问要求以执行本文中的步骤：  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning包</p></li>
或
<li><p>任何工作流和任何计划包</p></li></ul>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区的权限</p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr>  
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建工作区层级

{#step1-to-planning}

1. 单击工作区信息卡。
1. 单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**设置**。
默认情况下，**层次结构**&#x200B;部分打开。
1. 单击&#x200B;**层次结构**&#x200B;页面右上角的&#x200B;**新建层次结构**。
1. 单击&#x200B;**添加对象**&#x200B;并从下拉菜单中选择对象类型。 这将是层次结构中的第一个对象类型。<!--logged bug to correct to "Add object type"-->

   第一个对象类型只能是Planning记录类型。

   不能选择Workfront项目作为层次结构中其他对象类型的父级。

1. 单击“**添加对象**”可添加第二个对象类型，它是层级中的第一个子级，然后在下拉菜单中选择另一个对象类型。
每个附加对象类型都成为以前对象类型的子级。

   ![未选择字段的新层次结构框](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. 单击&#x200B;**选择连接的字段**&#x200B;以指示连接两个对象的字段。
1. （视情况而定）如果有多个连接字段，请从列表中选择一个，

   或

   单击&#x200B;**添加新连接**&#x200B;以添加新连接字段。

   这会根据您用作父项的记录类型创建一个连接字段，并根据您用作子项的记录类型创建一个与其对应的连接字段。

   如果您正在创建与Workfront项目的连接，则不会在该项目上创建字段。

1. （视情况而定）如果没有可用的连接字段，请单击“创建连接”****&#x200B;并添加新连接，然后单击“保存”****。

1. （视情况而定）如果要添加新连接，请执行以下操作：

   1. 在&#x200B;**名称**&#x200B;框中添加已连接字段的名称。
   1. 从以下连接类型中选择：

      * **多对多**
      * **一对多**
      * **多对一**
      * **一对一**

   1. 选择以下记录外观类型之一：

      * **名称和图像**
      * **名称**
      * **图像**

      有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

   1. 单击&#x200B;**保存**。

1. （视情况而定）如果在创建连接的字段时未选择&#x200B;**在链接的记录类型**&#x200B;上创建对应的字段，您将收到错误，必须首先执行以下操作：<!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. 在&#x200B;**新建层次结构**&#x200B;框中单击&#x200B;**取消**。
   1. 单击工作区名称左侧的返回箭头，然后单击要选择作为父项的记录类型的卡片。
   1. 打开您在上一步中选择的记录类型的表视图，然后转到包含要用作子级的对象类型的连接字段，将鼠标悬停在列标题上，然后单击&#x200B;**编辑**&#x200B;字段。
   1. 打开&#x200B;**在链接的记录类型**&#x200B;上创建对应的字段设置，然后单击&#x200B;**保存**。
   1. 返回工作区的&#x200B;**设置**&#x200B;区域，再次单击&#x200B;**新建层次结构**，然后按照步骤创建层次结构。

1. （可选）按照上述步骤，继续将最多4种对象类型添加到层级。 您可以先添加所有对象类型，然后添加它们之间的连接字段。
1. （可选）单击&#x200B;**删除**&#x200B;图标![删除图标](assets/minus-icon.png)以删除连接。
1. 单击&#x200B;**保存**&#x200B;以保存您的层次结构。

   >[!TIP]
   >
   >如果未设置所有连接的字段，**保存**&#x200B;按钮将灰显。

   出现以下情况：

   * 该层次结构已添加到工作区的&#x200B;**层次结构**&#x200B;部分。
   * 当您转到记录的页面时，填充连接字段的记录在其痕迹导航中显示所有连接。
1. （可选）将鼠标悬停在层次结构上，然后单击&#x200B;**更多**&#x200B;菜单。

   ![层次结构更多菜单已展开](assets/hierarchy-more-menu-expanded.png)

1. 单击下列选项之一：

   * **编辑**：这将打开&#x200B;**编辑层次结构**&#x200B;框，您可以在其中进行更改。
   * **删除**：这将永久删除层次结构。 无法恢复已删除的层次结构。 不删除连接字段。





