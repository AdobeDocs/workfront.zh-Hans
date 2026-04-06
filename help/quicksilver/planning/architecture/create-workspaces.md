---
title: 创建工作区
description: 工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。 记录类型按工作区中的部分组织。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ca8f1375d641531eaf11e3889ccb67a6fbe1788f
workflow-type: tm+mt
source-wordcount: '1200'
ht-degree: 0%

---


# 创建工作区

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。

工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区。

有关工作区的一般信息，请参阅[工作区概述](/help/quicksilver/planning/architecture/workspaces-overview.md)。

## 访问权限要求

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
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何Workfront或工作流包</p> 
<p>任何Workfront规划包</p>
<p>Workfront Planning Prime或更高版本包<span class="preview">一次创建多个工作区</span></p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   <p><span class="preview">系统管理员使用最佳实践模板包同时创建多个工作区</p>
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

<!--
Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 创建工作区

您可以创建一个工作区并向其中添加记录类型，以便在Workfront Planning中组织对象。

有关编辑工作区的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

您可以通过以下方式创建工作区：

* 从头开始或从模板创建一个工作区

  有关信息，请参阅本文中的[从头开始或从模板创建工作区](#create-a-workspace-from-scratch-or-from-a-template)部分。
* 使用AI支持的Planning Designer创建一个工作区。 此功能目前仅在Beta项目中有限数量的客户可用。

  有关信息，请参阅[Adobe Workfront规划Designer入门](/help/quicksilver/planning/general/planning-ai-designer.md)。

<div class="preview">

* 使用最佳实践多工作区模板包创建多个工作区

  有关信息，请参阅本文中的[使用最佳实践多工作区模板包创建多个工作区](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle)部分

  >[!TIP]
  >
  >仅当使用最佳实践模板包时，才能一次创建多个工作区。


</div>

### 从头开始或从模板创建工作区

{{step1-to-planning}}

1. 单击&#x200B;**创建工作区**

   此时会显示“创建工作区”框。 您可以从头开始创建工作区，也可以使用某个可用模板创建工作区。

1. （可选且有条件）单击以下任何预定义Workspace模板中的&#x200B;**预览**：

   * 基本：营销管理
   * 高级：营销管理
   * 企业：营销管理
   * 销售管理
   * 产品管理

   模板预览框打开。

   指示与每个模板关联的操作记录类型、分类以及字段数。

   ![预览工作区模板](assets/previewing-a-workspace-template.png)

   有关Workfront Planning工作区模板的信息，请参阅[工作区模板列表](/help/quicksilver/planning/architecture/workspace-templates.md)。

1. 在模板预览框中，单击&#x200B;**使用模板**&#x200B;以开始从所选模板创建工作区

   或

   单击&#x200B;**上一步**，然后单击&#x200B;**新建工作区**&#x200B;从头开始创建工作区。

   将创建以下工作区类型之一：

   * 一个名为&#x200B;**无标题Workspace**&#x200B;的空工作区，您可以在其中开始手动添加记录类型，以便从头开始创建工作区。
   * 以您选择的模板命名的工作区，该模板填充了示例记录类型。 您可以进一步自定义记录类型和工作区。

   对于Workfront管理员，新工作区显示在我所在的&#x200B;**工作区的**&#x200B;选项卡上。

   对于可以创建工作区的所有其他用户，新工作区显示在&#x200B;**工作区**&#x200B;区域中。

1. 单击新工作区标题中工作区的名称以对其进行重命名，然后按Enter键。

1. （可选且有条件）如果是从模板创建工作区，请单击&#x200B;**操作记录类型**&#x200B;或&#x200B;**分类**&#x200B;部分的名称

   或

   将鼠标悬停在节名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**重命名**&#x200B;以重命名节。

   >[!TIP]
   >
   >您可以从任何工作区重命名任何分区，即使您未创建该分区也是如此。

   有关编辑工作区（包括编辑工作区节）的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （可选）单击&#x200B;**添加记录类型**&#x200B;以将记录类型添加到任意节中的工作区。

   有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   有关在工作区中编辑和删除记录类型的详细信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

1. （可选）单击新工作区左侧的返回箭头以打开Planning主页。 在&#x200B;**选项卡上的**&#x200B;工作区中，为新工作区创建了新工作区信息卡。

   创建工作区的用户的名称将作为所有者保存在工作区信息卡上。

   >[!NOTE]
   >
   >对于当前正在过渡到Adobe Identity Management System (IMS)的用户，非IMS用户的仅Workfront用户创建的工作区将显示为&#x200B;**系统**&#x200B;所创建。
   >
   >有关IMS的信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

<div class="preview">

### 使用最佳实践多工作区模板包创建多个工作区

>[!IMPORTANT]
>
>只有在满足以下先决条件时，才能使用最佳实践模板捆绑包一次创建多个工作区：
>
>* 贵组织购买了Workfront Planning Prime或Ultimate包。
>* 您是系统管理员

只需单击一下，即可使用多工作区模板包创建6个工作区。

捆绑包中包含的模板包含工作区、记录类型、记录、视图和字段，以帮助您开始实施Planning。

>[!IMPORTANT]
>
>捆绑中包含的工作区和记录的名称只是示例，并非您自己环境的反映。
>
>根据我们的建议，记录类型和字段的名称可在任何组织用作任何行业中实施的标准。
>

{{step1-to-planning}}

1. 单击&#x200B;**创建工作区**

   此时会显示“创建工作区”框。 您可以从头开始创建工作区，也可以使用某个可用模板创建工作区。

1. 在&#x200B;**从此处开始（推荐）**&#x200B;区域单击&#x200B;**查看工作区设置**。
1. （可选）单击以下任何预定义Workspace模板中的&#x200B;**预览**&#x200B;以打开每个模板的“预览”框：

   * 1.全局分类和分类

     全局分类和分类模板包含我们建议您为您的环境中创建的所有记录类型和字段，以便成功实施Workfront Planning。

     您以后可以在您创建的其他工作区中链接或导入此模板中的记录类型。
   * 2.Fréscopa全球营销
   * 3.Fréscopa社交营销
   * 4.弗雷斯科帕媒体与公关
   * 5.弗雷斯科帕全球活动
   * 6.Fréscopa执行公司领导层

1. 打开每个工作区模板的&#x200B;**预览**&#x200B;框后，单击“返回”以返回&#x200B;**创建工作区**&#x200B;框，或单击“使用模板”以使用捆绑包中包含的模板和创建工作区。

   工作区是在系统管理员的&#x200B;**工作区**&#x200B;和&#x200B;**所有工作区**&#x200B;选项卡中创建和显示的。 系统管理员创建所有Standard-license用户并与他们共享新工作区后，这些用户都将在其“工作区”区域中看到工作区。

1. 开始编辑您创建的工作区，并添加与组织相关的记录类型、记录、视图和字段。

   有关实施Workfront的最佳实践的更多信息，请参阅[Adobe Workfront规划最佳实践：文章索引](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md)部分中的文章。

   有关编辑工作区的信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。

</div>



