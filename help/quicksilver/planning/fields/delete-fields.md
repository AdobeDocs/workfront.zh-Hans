---
title: 删除字段
description: 在Adobe Workfront Planning中，您可以删除不再相关的自定义字段。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1dc2791bed0dfada109ee102e09c25ae9a52e6b0
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---



# 删除字段

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中，您可以创建自定义字段以存储有关记录的信息。

有关在Workfront Planning中创建自定义字段的信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

您可以删除不再相关的Workfront Planning字段。

## 有关删除Workfront Planning字段的注意事项：

* 只能删除记录类型表格视图中的字段。
* 您无法删除记录的主字段。
* 存储在字段中的任何信息都将被删除并且无法恢复。
* 删除连接的记录字段时，所有连接的查找字段也会从您连接的记录类型中删除。 您连接到的记录类型的已连接记录字段也会从您连接的记录中删除。

  例如，当您将营销活动连接到另一个记录类型“产品”，并从营销活动中删除“已连接产品”字段和“产品状态”查找字段时，将删除以下内容：

   * 营销活动中的已连接产品字段
   * 营销活动中的产品状态查找字段
   * 产品中的“Campaign已连接”字段。

  有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td>   <p>管理工作区<span class="preview">和记录类型</span> </a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p></td> 
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

## 删除字段

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 单击要删除其记录字段的工作区。

   此时会打开工作区，并显示记录类型。

1. 单击记录类型的卡。

1. （视情况而定）如果尚未选择，请单击记录类型页面上&#x200B;**表视图**&#x200B;的选项卡。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。

1. 在列标题中查找要删除的字段，将鼠标悬停在列标题上，然后单击字段名称后的向下箭头。

   在表标题中突出显示的字段名称后面的![箭头菜单](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 单击&#x200B;**删除**。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 单击&#x200B;**删除**&#x200B;以确认。

   该字段已删除，无法恢复，并且无法再与任何记录关联。
