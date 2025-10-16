---
title: 为记录类型配置跨工作区功能
description: 您可以在Adobe Workfront Planning中启用记录类型，将其添加到另一个工作区或从另一个工作区连接。
hidefromtoc: true
hide: true
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type.

-->

# 为记录类型配置跨工作区功能

{{planning-important-intro}}

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

您可以在Adobe Workfront Planning中将记录类型配置为可在多个工作区中使用。

可以将记录类型指定为下列类型之一：

* **全局记录类型**：用户可以将全局记录类型添加到其可以管理的其他工作区。
* **可连接的记录类型**：用户可以从其他工作区连接到此记录类型。

必须先定义记录类型的跨工作区功能，然后工作区管理员才能将其添加到其他工作区或从其他工作区连接该记录类型。

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
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>要配置可连接的记录类型，请执行以下操作： </p>
<ul> 
<li><p>任何Workfront包和任何Planning包</p></li>
<p>或</p>
<li><p>工作流和规划Prime和Ultimate包</p></li></ul>

<p>要配置全局记录类型，请执行以下操作：</p>

<ul> 
<li><p>任何Workfront包和Planning Plus包</p></li>
<p>或</p>
<li><p>工作流和规划Prime和Ultimate包</p></li></ul>
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

<!--Old:

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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Workflow Prime or Ultimate package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> -- >

## Configure global record types

<!--this is a UI term; don't change the title of this section-->

作为工作区管理员，您可以将记录类型配置为全局记录类型。 全局记录类型可以添加到其他工作区。

工作区管理员可以将全局记录类型添加到他们管理的工作区。 记录类型的原始字段也会添加到辅助工作区。

用户可以从他们具有Contribute权限以及已添加全局记录类型（包括其原始工作区）的任何工作区将记录添加到全局记录类型。 用户可以从其只有“查看”权限的工作区中查看记录。

有关详细信息，请参阅[跨工作区记录类型概述](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。

要将记录类型配置为全局，请执行以下操作：

{{step1-to-planning}}

1. 单击要将其记录类型配置为全局的工作区。

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，然后单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。<!--add new screen shot without Share for now-->

     ![记录类型卡片中的更多菜单选项](assets/more-menu-options-from-record-type-card.png)

   * 单击记录类型卡以打开记录类型页面，然后单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。
1. 单击&#x200B;**编辑**&#x200B;或&#x200B;**设置**。

   >[!TIP]
   >
   >将记录类型添加到另一个工作区时，它将显示为该工作区中的全局记录类型。 在这种情况下，“编辑”和“设置”选项将灰显。

1. （视情况而定）如果您单击&#x200B;**编辑**，请在&#x200B;**编辑记录类型**&#x200B;框中单击&#x200B;**跨工作区设置**&#x200B;选项卡

   或者，如果您单击了&#x200B;**设置**，请单击左侧面板中的&#x200B;**跨工作区设置**&#x200B;部分。
1. 启用&#x200B;**允许将此记录类型添加到其他工作区**&#x200B;设置。

   ![启用“添加到其他工作区”的情况下编辑记录类型跨工作区设置](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >将全局记录类型添加到另一个工作区后，无法再禁用此设置。

1. 在&#x200B;**选择谁可以将此记录类型添加到他们管理的工作区**&#x200B;字段中，添加要允许将此记录类型添加到他们管理的工作区的实体。

   您的姓名会自动添加到字段中。

   您可以添加个人用户、组、团队、职位角色或公司，希望允许其用户将此记录类型添加到他们管理的工作区。

   保存记录类型后，可以编辑此字段。

1. （可选）从&#x200B;**选择谁可以将该记录类型添加到他们管理的工作区**&#x200B;字段中移除您的姓名。

   >[!TIP]
   >
   >必须至少指定一个实体（用户、团队、组、角色或公司）才能启用此设置。

1. （视情况而定）在&#x200B;**编辑记录类型**&#x200B;框中单击&#x200B;**保存**，或者单击页眉中&#x200B;**设置**&#x200B;左侧的返回箭头以保存更改。

   出现以下情况：

   * 记录类型及其字段现在可以由您指定的人员添加到另一个工作区。

   >[!NOTE]
   >
   >只能从其原始工作区中编辑记录类型的外观和设置及其原始字段。

   * 记录类型卡片显示&#x200B;**全局记录类型**&#x200B;图标![全局记录类型图标](assets/global-icon.png)，以指示该记录类型可以添加到其他工作区。
   * 系统生成的&#x200B;**Workspace**&#x200B;字段已添加到记录类型及其记录详细信息的表视图。

     Workspace字段显示从中创建每个记录的工作区。

     此字段为只读，无法删除。
1. （可选）转到另一个工作区并使用现有记录类型创建记录类型。 选择在上述步骤中启用的记录类型。

   有关信息，请参阅[从另一个工作区添加现有记录类型](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。

   从辅助工作区中的全局记录类型添加的记录类型还显示&#x200B;**全局记录类型**&#x200B;图标![全局记录类型图标](assets/global-icon.png)。
1. （可选）返回创建全局记录类型的原始工作区，并按照以上<!--ensure this stays accurate-->的步骤1-4编辑该记录类型
1. （可选）查看在使用此记录类型的&#x200B;**工作区第**&#x200B;节中添加了全局记录的工作区列表。 工作区所有者的名称也会列在工作区名称旁边。

   ![使用此记录类型的工作区](assets/workspaces-where-this-record-type-is-used.png)


## 配置可连接的记录类型

<!--this is a UI term; don't change the title of this section-->

在创建或编辑记录类型时，可以配置要从其他工作区连接的记录类型。

将记录类型配置为可连接：

{{step1-to-planning}}

1. 单击要将其记录类型配置为可连接的工作区。

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，然后单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)

     ![记录类型卡片中的更多菜单选项](assets/more-menu-options-from-record-type-card.png) <!--add new screen shot without Share for now-->

   * 单击记录类型卡以打开记录类型页面，然后单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。
1. 单击&#x200B;**编辑**&#x200B;或&#x200B;**设置**。

1. （视情况而定）如果您单击&#x200B;**编辑**，请在&#x200B;**编辑记录类型**&#x200B;框中单击&#x200B;**跨工作区设置**&#x200B;选项卡

   或者，如果您单击了&#x200B;**设置**，请单击左侧面板中的&#x200B;**跨工作区设置**&#x200B;部分。

1. 启用&#x200B;**允许连接到其他工作区中的此记录类型**&#x200B;设置。<!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![启用从其他工作区连接的编辑记录类型跨工作区设置选项卡](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   启用后，记录类型可访问，并可从其他工作区连接到。

1. 选择可以访问记录类型的工作区。 从以下选项中进行选择：

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **所有工作区**：用户可以从其拥有管理权限的所有工作区连接到此记录类型。
   * **特定工作区**：从下拉菜单中，添加工作区管理员可以连接到此记录类型的工作区的名称。
1. （视情况而定）在&#x200B;**编辑记录类型**&#x200B;框中单击&#x200B;**保存**，或者单击页眉中&#x200B;**设置**&#x200B;左侧的返回箭头以保存更改。

   出现以下情况：

   * 现在，记录类型及其字段可用于从指定的工作区连接到。
   * 记录类型卡显示可连接的记录类型图标![可连接的记录类型图标](assets/connect-from-other-workspaces-icon.png)，以指示可从配置中指定的任何工作区连接到该记录类型。

1. （可选）转到另一个工作区，并将连接添加到在上述步骤中为跨工作区连接性启用的记录类型。

   有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。









