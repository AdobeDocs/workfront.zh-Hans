---
title: 编辑记录类型
description: 保存记录类型后，您可以对其进行编辑。 记录类型是Adobe Workfront Planning的对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 2%

---


# 编辑记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 您可以编辑您或其他人创建的记录类型的外观。 有关创建Workfront Planning记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

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
<p>贵组织的Workfront实例必须载入Adobe Unified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
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
   <td>   <p>管理工作区<span class="preview">和记录类型</span>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
   <p>只有系统管理员才能启用记录类型以从其他工作区连接</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## 编辑记录类型

{{step1-to-planning}}

1. 单击要编辑其记录类型的工作区，

   此时会打开工作区页面，并显示记录类型。
1. 执行下列操作之一：

   * 将鼠标悬停在记录类型的卡片上，然后单击记录类型卡片右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**编辑**
或
   * 单击记录类型卡以打开记录类型页面，单击记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**编辑**。

   ![记录类型卡片中的更多菜单选项](assets/more-menu-options-from-record-type-card.png)

1. 在&#x200B;**编辑记录类型**&#x200B;框中，**外观**&#x200B;选项卡默认打开。

   ![编辑记录类型框外观选项卡](assets/edit-record-type-box-appearance-tab.png)

   在&#x200B;**外观**&#x200B;选项卡中更新以下信息：

   * 根据需要编辑记录类型名称。<!--did they add a field label for this?-->
   * **描述**：编辑或添加记录类型的描述，其中包含有关该记录类型的详细信息。
   * 编辑与记录类型关联的图标的颜色和形状。 执行以下操作：
      * 选择用于标识记录类型的颜色。 这是记录类型图标的颜色。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

1. （视情况而定）如果您是系统管理员，请单击&#x200B;**编辑记录类型**&#x200B;框中的&#x200B;**高级设置**&#x200B;选项卡。<!--the info here is duplicated in the Create record types article-->

   ![编辑记录类型框高级设置选项卡](assets/edit-record-type-box-advanced-settings-tab.png)

1. （视情况而定）在&#x200B;**高级设置**&#x200B;选项卡中更新以下信息：

   * 启用&#x200B;**从其他工作区连接**&#x200B;设置。 启用后，记录类型可访问，并可从其他工作区连接。
   * 选择可以访问记录类型的工作区。 从以下选项中进行选择：

      * **系统范围**：用户可以从其拥有管理权限的所有工作区连接到此记录类型。
      * **特定工作区**：添加工作区管理员可以连接到此记录类型的工作区的名称。

1. 单击&#x200B;**保存**。

   工作区上的记录类型卡片在右上角显示一个连接图标![从其他工作区连接图标](assets/connect-from-other-workspaces-icon.png)，表示现在可以从其他工作区访问该记录。

1. （可选）单击工作区区域中的记录类型卡以打开记录类型的页面，然后重命名标题中的记录类型。

1. （可选）要编辑其他记录类型，请从记录类型页面中，展开记录类型名称右侧的向下箭头，搜索记录类型，然后在记录类型显示在列表中时将其选定。

   带有搜索框的记录类型页面上的![记录类型下拉列表](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
