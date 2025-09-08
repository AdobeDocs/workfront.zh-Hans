---
title: 添加现有记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以从另一个工作区导入现有记录类型。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 9b95b5a52576327a3df8d6955925b96c2e45848f
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 添加现有记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以导入现有记录类型或将现有记录类型添加到另一个工作区。

必须先将记录类型指定为集中类型，然后工作区管理员才能将其导入其他工作区。

在定义记录类型的跨工作区设置时，您可以在创建或编辑记录类型时将记录类型指定为集中类型。

有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

在将记录从集中记录类型添加到工作区之前，请参阅文章[集中记录类型概述](/help/quicksilver/planning/architecture/centralized-record-types-overview.md)。

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

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   

## 从现有记录类型创建记录类型

1. 开始创建记录类型，如文章[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然后单击&#x200B;**添加现有**。<!--check this - the option might have been renamed in the UI-->

   ![模式以添加记录类型，并带有从其他工作区导入的选项](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 单击&#x200B;**继续**。
1. 在&#x200B;**选择记录类型**&#x200B;框中，单击要从现有工作区添加的记录类型的卡片，然后单击&#x200B;**添加**。

   记录类型将添加到您选择的工作区。

   >[!TIP]
   >
   >当没有将记录类型配置为添加到另一个工作区时，在创建记录类型时不会显示从另一个工作区导入记录类型的选项。

   出现以下情况：

   * 还从现有的集中记录类型中添加了以下信息：

      * 所有原始字段
      * 所有记录连接
   * 只有在您至少具有其他工作区的“查看”权限时，才能查看从这些工作区添加的记录。
   * **集中式记录类型**&#x200B;图标![集中式记录类型图标](assets/global-icon.png)已添加到导入的记录类型的卡片中。
   * 只读&#x200B;**Workspace**&#x200B;字段已添加到导入的记录类型表视图。 字段显示每个记录创建时所在的工作区。

     >[!NOTE]
     >
     >* 无法编辑导入的记录类型的外观、高级设置或原始字段。 只能从原始工作区编辑记录类型及其所有原始字段和设置。

1. （可选）单击，然后将新添加的记录类型拖放到工作区中的任何部分。

1. （可选）单击导入的记录类型卡片中的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或该记录类型在其页面上的名称右侧，然后单击&#x200B;**共享**&#x200B;以与同一工作区中的其他用户共享。

1. （可选）单击导入的记录类型卡片中的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或该记录类型在其页面上的名称右侧，然后单击&#x200B;**删除**。
1. （视情况而定）在提供的字段中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。

   出现以下情况：

   * 从所选工作区中删除从集中式记录类型创建的记录类型。
   * 原始记录类型及其字段保留在其原始工作区中。
   * 从同一集中记录导入的所有其他记录类型都保留在其工作区中。
   * 从当前工作区添加到记录类型的记录将被删除。 从添加了集中记录类型的附加工作区中添加的所有其他记录都将保留。





