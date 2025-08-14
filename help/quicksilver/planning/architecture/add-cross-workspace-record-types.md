---
title: 添加跨工作区记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以从另一个工作区导入现有记录类型。
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# 添加跨工作区记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以导入现有记录类型或将现有记录类型添加到另一个工作区。

必须先将记录类型指定为集中类型，然后工作区管理员才能将其导入其他工作区。

在定义记录类型的跨工作区设置时，您可以在创建或编辑记录类型时将记录类型指定为集中类型。

有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

## 访问要求

+++ 展开以查看访问要求。  

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

## 集中记录类型概述

从其他工作区添加现有记录类型时的注意事项

* 当没有将记录类型配置为添加到另一个工作区时，在创建记录类型时不会显示从另一个工作区导入记录类型的选项。<!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* 从另一个工作区添加记录类型后，还将从现有记录类型添加以下信息：

   * 字段
   * 记录
   * 记录连接

* 只能在其原始工作区中编辑记录类型，包括其字段。 不能从添加该代码的工作区对其进行编辑。

## 从现有记录类型创建记录类型

1. 开始创建记录类型，如文章[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然后单击&#x200B;**添加现有**。<!--check this - the option might have been renamed in the UI-->

   ![模式以添加记录类型，并带有从其他工作区导入的选项](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. 单击&#x200B;**继续**。
1. 在&#x200B;**选择记录类型**&#x200B;框中，单击要从现有工作区添加的记录类型的卡片，然后单击&#x200B;**添加**。

   记录类型将添加到您选择的工作区，并且会发生以下情况：

   * **跨工作区记录类型**&#x200B;图标![跨工作区连接图标](assets/global-icon.png)已添加到导入记录类型的卡片中。
   * 只读&#x200B;**Workspace**&#x200B;字段已添加到导入的记录类型。 字段显示每个记录创建时所在的工作区。

     >[!NOTE]
     >
     >* 您无法编辑导入的记录类型或其字段。 您可以从原始工作区中编辑记录类型及其字段。

1. （可选）单击导入的记录类型卡片中的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，或该记录类型在其页面上的名称右侧，然后单击&#x200B;**删除**。
1. （视情况而定）在提供的字段中键入&#x200B;**删除**，然后单击&#x200B;**永久删除**。

   这会从所选工作区中删除导入的记录类型。 原始记录类型及其字段保留在其原始工作区中。

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



