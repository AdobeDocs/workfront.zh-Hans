---
title: 在Adobe Workfront Planning中创建请求表单
description: 在Adobe Workfront Planning区域中选择记录类型后，您可以创建与该记录类型关联的请求表单，并与其他内部或外部用户共享指向该记录类型的链接。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# 在Adobe Workfront Planning中创建请求表单

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

在Adobe Workfront Planning区域中选择记录类型后，您可以创建请求表单并将其与该记录类型关联。 然后，您可以与其他内部或外部用户共享指向该页面的链接。<!--double-check on the external part of it-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能访问Workfront Planning：

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
   <td role="rowheader"><p>Adobe Workfront规划计划*</p></td>
   <td>
<p>任何 </p>   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>标准</p>
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
   <td>
   <ul>
   <li><p>管理工作区的权限</p></li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    </ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为记录类型创建请求表单

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。

1. 单击页眉中记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-menu.png)，然后单击&#x200B;**创建请求表单**。
1. 更新请求表单的名称。 默认情况下，表单的名称为&#x200B;**无标题的请求表单**。<!--check this; you logged a bug to rename it to this but was it fixed?-->
1. （可选）为请求表单添加&#x200B;**描述**。

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. 单击&#x200B;**创建**。此时将打开所选记录类型的请求表单。

   默认情况下，请求表单包含以下信息：

   * **默认的分区**：这是Workfront应用于请求表单的默认分区界限。 无法重命名或删除默认部分。
   * **主题**&#x200B;字段：将在Workfront中标识该请求的字段。 此功能尚不可用。
   * 与记录类型关联的所有字段。

   向此记录类型提交请求的每个人均可看到请求表单中包含的字段。

1. （可选）删除&#x200B;**主题**&#x200B;字段，因为此字段在Workfront Planning中不可见。<!--remove this step when we connect intake with the Requests area in Workfront-->
1. 将鼠标悬停在要删除的表单上的任何字段上。 它们已添加到表单左侧的&#x200B;**字段**&#x200B;选项卡中。
1. 单击任意字段，然后使用表单右侧的控件定义有关这些字段的以下任意信息：

   * **标签**：这是显示在请求表单中的字段名称。 这不会更改记录字段的名称。
   * **说明**：添加有关该字段的更多信息。
   * **生成必填字段**：选定后，该字段必须具有值。 否则，无法提交表单。
   * **添加逻辑**：定义必须满足哪些条件才能显示或隐藏字段。

1. 单击表单右侧的“内容元素”选项卡，然后添加以下任意元素：

   * 描述性文本
   * 分节符

   有关构建自定义表单的详细信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。





