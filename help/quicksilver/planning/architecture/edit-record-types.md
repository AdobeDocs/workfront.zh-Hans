---
title: 编辑记录类型
description: 保存记录类型后，您可以对其进行编辑。 记录类型是Adobe Workfront Planning的对象类型。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 2%

---


# 编辑记录类型

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
   <td>   <p>管理工作区</a>的权限 </p>  
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

<!--
OLD:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

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

1. （视情况而定）如果您是系统管理员，请单击&#x200B;**编辑记录类型**&#x200B;框中的&#x200B;**高级设置**&#x200B;选项卡。

   ![编辑记录类型框高级设置选项卡](assets/edit-record-type-box-advanced-settings-tab.png)

1. （视情况而定）作为系统管理员，在&#x200B;**高级设置**&#x200B;选项卡中更新以下信息：

   * **从其他工作区连接**：选择此切换可允许用户从其他工作区连接到此记录类型。 默认情况下，该选项处于取消选中状态。
   * **系统范围**：选择此选项可允许用户从系统中的所有工作区连接到此记录。
   * **特定工作区**：选择此选项可限制用户可以从中连接到此记录类型的工作区，然后展开下拉菜单并选择您希望用户从中连接到此记录类型的工作区。 您可以开始键入工作区的名称，并在工作区显示在列表中时将其选定。

1. 单击&#x200B;**保存**。

   工作区上的记录类型卡片在右上角显示一个连接图标![从其他工作区连接图标](assets/connect-from-other-workspaces-icon.png)，表示现在可以从其他工作区访问该记录。

1. （可选）单击工作区区域中的记录类型卡以打开记录类型的页面，然后重命名标题中的记录类型。

1. （可选）要编辑其他记录类型，请从记录类型页面中，展开记录类型名称右侧的向下箭头，搜索记录类型，然后在记录类型显示在列表中时将其选定。

   带有搜索框的记录类型页面上的![记录类型下拉列表](assets/record-type-drop-down-on-record-type-page-with-search-box.png)