---
title: 为记录类型配置跨工作区功能
description: 您可以将记录类型添加到另一个工作区或从另一个工作区连接。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this imported record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# 为记录类型配置跨工作区功能

<!--this is linked to the UI in the info icon when you enable a record to be either centralized or connectable-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

以下是记录类型的跨工作区功能：

* 您可以将记录类型指定为集中记录类型。 用户可以将集中式记录类型添加到他们可以管理的其他工作区。
* 可以将记录类型指定为可连接。 用户可以从其他工作区连接到此记录类型。

必须先定义记录类型的跨工作区功能，然后工作区管理员才能从其他工作区连接记录类型或将记录类型导入其他工作区。

在创建或编辑记录类型时，可以定义记录类型的跨工作区功能。

有关信息，请参阅以下文章之一：

* [创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)
* [编辑记录类型](/help/quicksilver/planning/architecture/edit-record-types.md)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td role="rowheader"><p>Adobe Workfront包*</p></td> 
   <td> 
<ul><li><p>任何Workfront包</p></li>
与
<li><p>Planning Plus包</p></li></ul>
或：
<ul><li><p>任何工作流包</p> </li>
与
<li><p>规划Prime或Ultimate包</p></li></ul>
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
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

## 配置集中记录类型

<!--this is a UI term; don't change the title of this section-->
<!--IMPORTANT: not sure if we can call these centralized yet - checking with Lilit as of Sept 2; you might need to revert this to what the screen shot shows below?????-->

作为工作区管理员，您可以将记录类型配置为集中式记录类型。 集中记录类型可以添加到其他工作区。

工作区管理员可以将集中式记录类型添加到他们管理的工作区。 还会添加记录类型的原始字段。

用户可以从他们有权参与的任何工作区将记录添加到集中记录类型中，该记录类型被添加到何处，包括其主要工作区。 他们只能从他们有权查看的工作区中查看记录。

要将添加记录类型配置为集中记录类型，请执行以下操作：

{{step1-to-planning}}

1. 单击要编辑其记录类型的工作区。

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

1. 在&#x200B;**选择谁可以将此记录类型添加到他们管理的工作区**&#x200B;字段中，添加要允许将此记录类型添加到他们管理的工作区的用户。

   您的姓名会自动添加到字段中。

   您可以添加要允许其用户将此记录类型添加到其管理的工作区的单个用户或组、团队、职位角色或公司。

   保存记录类型后，可以编辑此字段。
1. （可选）从&#x200B;**选择谁可以将该记录类型添加到他们管理的工作区**&#x200B;字段中移除您的姓名。

1. 单击&#x200B;**保存**。

   出现以下情况：

   * 记录类型及其字段现在可以由您指定的人员添加到另一个工作区。

   >[!NOTE]
   >
   >只能从原始工作区中编辑记录类型及其字段。

   * 记录类型卡显示全局图标![全局记录类型图标](assets/global-icon.png)，以指示该记录类型可以添加到您在配置中指定的管理员所在的任何工作区。
   * 系统生成的&#x200B;**Workspace**&#x200B;字段已添加到记录类型。

     Workspace字段显示从中创建每个记录的工作区。

     此字段为只读，无法删除。
1. （可选）转到另一个工作区并使用现有记录类型创建记录类型。 选择在上述步骤中启用的记录类型。

   有关信息，请参阅[添加现有记录类型](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md)。

## 配置可连接的记录类型

<!--this is a UI term; don't change the title of this section-->

在创建或编辑记录类型时，可以配置要从其他工作区连接的记录类型。

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
1. 启用&#x200B;**允许连接到其他工作区中的此记录类型**&#x200B;设置。<!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![启用从其他工作区连接的编辑记录类型“高级设置”选项卡](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   启用后，记录类型可访问，并可从其他工作区连接。

1. 选择可以访问记录类型的工作区。 从以下选项中进行选择：

   * **系统范围**：用户可以从其拥有管理权限的所有工作区连接到此记录类型。
   * **特定工作区**：添加工作区管理员可以连接到此记录类型的工作区的名称。
1. 单击&#x200B;**编辑**。

   出现以下情况：

   * 现在，记录类型及其字段可用于从指定的工作区连接。
   * 记录类型卡片显示一个跨工作区连接图标![跨工作区连接图标](assets/connect-from-other-workspaces-icon.png)，以指示可以从您在配置中指定的任何工作区连接记录类型。

   记录类型变为可以从指定的工作区连接。
1. （可选）转到另一个工作区，并将连接添加到在上述步骤中为跨工作区连接性启用的记录类型。

   有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。









