---
title: 从其他Workspace添加现有记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以添加在另一个工作区中创建的现有记录类型。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 从另一个工作区添加现有记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以将存在于另一个工作区中的记录类型添加到您在Adobe Workfront Planning中管理的工作区。

本文介绍了如何从现有记录类型添加记录类型，以及在不再需要记录类型时如何删除记录类型。

工作区管理员必须先将记录类型指定为全局记录类型，然后才能将其添加到作为现有记录类型管理的工作区中。

在创建或编辑记录类型时，您可以在定义其跨工作区设置时将记录类型指定为全局记录类型。

有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

在从全局记录类型向工作区中添加记录之前，请参阅文章[跨工作区记录类型概述](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。


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
<ul><li><p>任何Workfront包</p></li>
<p>与</p>
<li><p>用于创建可连接记录类型的任意Planning包</p></li>
<li><p>用于创建全局记录类型的Planning Plus包</p></li>
</ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户经理。 </p> 
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

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 从现有记录类型创建记录类型

1. 开始创建记录类型，如文章[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然后单击&#x200B;**添加现有**。<!--check this - the option might have been renamed in the UI-->

   ![模式以添加记录类型，并带有从另一个工作区添加的选项](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 单击&#x200B;**继续**。
1. 在&#x200B;**选择记录类型**&#x200B;框中，单击要从现有工作区添加的记录类型的卡片，然后单击&#x200B;**添加**。

   记录类型将添加到您选择的工作区。

   >[!TIP]
   >
   >当没有将记录类型配置为添加到另一个工作区时，不显示从另一个工作区添加它们的选项。

   出现以下情况：

   * 还从现有全局记录类型中添加了以下信息：

      * 所有原始字段
      * 所有记录连接
   * 只有在您至少具有这些工作区的“查看”权限时，才能查看从使用相同全局记录类型的其它工作区添加的记录。
   * **全局记录类型**&#x200B;图标![全局记录类型图标](assets/global-icon.png)已添加到新记录类型的卡片中。
   * 只读&#x200B;**Workspace**&#x200B;字段已添加到新记录类型表视图中。 字段显示每个记录创建时所在的工作区。

     >[!NOTE]
     >
     >您无法编辑新记录类型的外观、其他设置或原始字段。 只能从原始工作区编辑记录类型及其所有原始字段和设置。

1. （可选）单击，然后将新添加的记录类型拖放到工作区中的任何部分。

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

## 从辅助工作区中删除全局记录类型

如果不再需要某个记录类型，您可以将其从另一个工作区中删除。 删除它只会将其从辅助工作区中删除，并且将删除该工作区中添加的记录。 原始记录类型会保留在其原始工作区中，以及已添加该记录的其他工作区中。

要从辅助工作区中删除全局记录类型，请执行以下操作：

1. 转到辅助工作区中的全局记录类型。

1. （可选）单击记录类型卡片上的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或记录类型名称页面右侧，然后单击&#x200B;**删除**。
1. （视情况而定）在提供的字段中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。

   出现以下情况：

   * 从所选工作区中删除从全局记录类型创建的记录类型。
   * 原始记录类型及其字段保留在其原始工作区中。
   * 记录类型将保留在添加该记录的所有其他工作区中。
   * 从当前工作区添加到记录类型的记录将被删除。 从添加全局记录类型的附加工作区中添加的所有其他记录都将保留。





