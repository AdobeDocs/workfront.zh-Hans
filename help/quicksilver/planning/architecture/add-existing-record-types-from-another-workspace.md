---
title: 从其他Workspace添加现有记录类型
description: 记录类型是Adobe Workfront Planning的对象类型。 在Workfront Planning中，您可以添加在另一个工作区中创建的现有记录类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---


# 从另一个工作区添加现有记录类型

{{planning-important-intro}}

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

作为工作区管理员，您可以将存在于另一个工作区中的记录类型添加到您在Adobe Workfront Planning中管理的工作区。

工作区管理员必须先将记录类型指定为全局记录类型，然后才能将其添加到作为现有记录类型管理的工作区中。 通过定义记录类型的跨工作区设置，Workspace管理员可以在创建或编辑记录类型时将记录类型指定为全局记录类型。

有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

本文介绍了如何从现有记录类型添加记录类型。

在从全局记录类型向工作区中添加记录之前，另请参阅文章[跨工作区记录类型概述](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)。


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
<ul><li><p>任何Workfront包和Planning Plus包</p></li>
<p>或</p>
<li><p>任何工作流和计划Prime或Ultimate包</p></p></li></ul>
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
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
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
</table>-->

## 通过从另一个工作区添加现有记录类型来创建记录类型

>[!NOTE]
>
>确保在至少一个其他工作区中至少有一个指定为全局的记录类型。
>
>有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

1. 开始创建记录类型，如文章[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)中所述，然后单击&#x200B;**添加现有**。<!--check this - the option might have been renamed in the UI-->

   ![模式以添加记录类型，并带有从另一个工作区添加的选项](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >当没有记录类型配置为添加到系统中的其他工作区时，不显示&#x200B;**添加现有**&#x200B;选项。

1. 单击&#x200B;**继续**。
1. 在&#x200B;**选择记录类型**&#x200B;框中，单击要从现有工作区添加的记录类型的卡片，然后单击&#x200B;**添加**。

   记录类型已添加到您选择的工作区，**全局记录类型**&#x200B;图标![](assets/global-icon.png)将显示在记录类型的卡片上。

   出现以下情况：

   * 还从现有全局记录类型中添加了以下信息：

      * 所有原始字段
      * 所有记录连接
   * 只有在您至少具有这些工作区的“查看”权限时，才能查看从使用相同全局记录类型的其它工作区添加的记录。
   * 只读&#x200B;**Workspace**&#x200B;字段已添加到新记录类型表视图中。 字段显示创建每个记录的工作区。

     >[!NOTE]
     >
     >您无法编辑新记录类型的外观、其他设置或原始字段。 只能从原始工作区编辑记录类型及其所有原始字段和设置。

1. （可选）单击，然后将新添加的记录类型拖放到工作区中的任何部分。
1. （可选）单击新记录类型卡片上的&#x200B;**更多**&#x200B;菜单或其页面上的记录类型名称右侧，然后单击&#x200B;**删除**。

   有关详细信息，请参阅文章[删除记录类型](/help/quicksilver/planning/architecture/delete-record-types.md)中的“删除全局记录类型”部分。

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;！ — 使用Lilit检查我们是否可以将自动化或请求表单添加到辅助全局RT?? — 添加步骤以及这些文章的链接（如果/当是时） — >







