---
title: 为记录类型配置跨工作区功能
description: 您可以将记录类型添加到另一个工作区或从另一个工作区连接。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

# 为记录类型配置跨工作区功能

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以在Adobe Workfront Planning中指定记录类型，以添加到另一个工作区或从另一个工作区连接。

必须先定义记录类型的跨工作区功能，然后工作区管理员才能从其他工作区连接记录类型或将记录类型导入其他工作区。

在创建或编辑记录类型时，可以定义记录类型的跨工作区功能。

有关信息，请参阅以下文章之一：

* [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)
* [编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)

## 访问要求

+++ 展开以查看访问要求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>  </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置将记录类型添加到其他工作区

作为工作区管理员，您可以在创建或编辑记录类型时，配置要添加到其他工作区的记录类型。

在配置将记录类型添加到其他工作区时，工作区管理员可以将记录类型及其所有信息导入到他们管理的某个工作区中。

要配置在编辑记录类型时将记录类型添加到另一个工作区，请执行以下操作：

{{step1-to-planning}}

1. 单击要编辑其记录类型的工作区，

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，然后单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)
或
   * 单击记录类型卡以打开记录类型页面，然后单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。
1. 单击&#x200B;**编辑**。

   ![记录类型卡片中的更多菜单选项](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**编辑记录类型**&#x200B;框中，选择&#x200B;**高级设置**&#x200B;选项卡。
1. 启用&#x200B;**允许将此记录类型添加到其他工作区**&#x200B;设置。

   ![使用“添加到其他工作区”编辑记录类型高级设置启用](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. 在&#x200B;**选择谁可以将该记录类型添加到他们管理的工作区**&#x200B;字段中，将您要添加该记录类型的用户添加到他们管理的工作区。

   您的姓名会自动添加到字段中。

   您可以将个人用户、组、团队、职位角色或要为其添加此记录类型的用户添加到其管理的工作区。

   保存记录类型后，可以编辑此字段。
1. （可选）从&#x200B;**选择谁可以将该记录类型添加到他们管理的工作区**&#x200B;字段中移除您的姓名。

1. 单击&#x200B;**保存**。

   出现以下情况：

   * 记录类型及其字段现在可以由您指定的人员添加到另一个工作区。
   * 记录类型卡显示全局图标![全局记录类型图标](assets/global-icon.png)，以指示该记录类型可以添加到您在配置中指定的管理员所在的任何工作区。
   * 系统生成的&#x200B;**Workspace**&#x200B;字段已添加到记录类型。

     Workspace字段显示从中创建每个记录的工作区。

     此字段为只读，无法删除。

## 配置连接到其他工作区中的记录类型

在创建或编辑记录类型时，可以配置记录类型以从其他工作区连接到。

要在编辑记录类型时配置记录类型以从其他工作区连接到，请执行以下操作：

{{step1-to-planning}}

1. 单击要编辑其记录类型的工作区，

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，然后单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**编辑**
或
   * 单击记录类型卡以打开记录类型页面，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**编辑**。

   ![记录类型卡片中的更多菜单选项](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**编辑记录类型**&#x200B;框中，选择&#x200B;**高级设置**&#x200B;选项卡。
1. 启用&#x200B;**允许从其他工作区**&#x200B;设置连接到此记录类型。<!-- check the setting name, this is the suggested UI text to be edited by Lilit and team-->

   ![启用从其他工作区连接的编辑记录类型“高级设置”选项卡](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   启用后，记录类型可访问，并可从其他工作区连接。

1. 选择可以访问记录类型的工作区。 从以下选项中进行选择：

   * **系统范围**：用户可以从其拥有管理权限的所有工作区连接到此记录类型。
   * **特定工作区**：添加工作区管理员可以连接到此记录类型的工作区的名称。
1. 单击&#x200B;**编辑**。

   出现以下情况：

   * 现在，记录类型及其字段可用于从指定的工作区连接。
   * 记录类型卡片显示一个跨工作区连接图标![跨工作区连接图标](assets/connect-from-other-workspaces-icon.png)，以指示可以从您在配置中指定的任何工作区连接记录类型。






