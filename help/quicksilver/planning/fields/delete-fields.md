---
title: 删除字段
description: 在Adobe Workfront Planning中，您可以删除不再相关的自定义字段。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EusoK7-jmYJHg9nqyvvQamsfVeUy802p36EyDmLGwik
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 733
ht-degree: 1%

---

# 删除字段

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

在Adobe Workfront Planning中，您可以创建自定义字段以存储有关记录的信息。

有关在Workfront Planning中创建自定义字段的信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

您可以删除不再相关的Workfront Planning字段。

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
<ul> 
<li><p>任何Workfront和任何Planning包</p></li>
或
<li><p>任何工作流和任何计划包</p></li></ul>

<p>要从全局记录类型中删除字段，请执行以下操作：</p>
<ul><li><p>任何Workfront包和Planning Plus包</p></li>
或
<li><p>任何工作流和计划Prime和Ultimate包</p></li></ul>

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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table>
-->

## 有关删除Workfront Planning字段的注意事项：

* 只能删除记录类型表格视图中的字段。
* 您无法删除记录的主字段。
* 存储在字段中的任何信息都将被删除并且无法恢复。
* 删除连接的记录字段时，所有连接的查找字段也会从您连接的记录类型中删除。 您连接到的记录类型的已连接记录字段也会从您连接的记录中删除。

  例如，如果将Campaigns连接到另一个记录类型“产品”，并从营销活动中删除“已连接产品”字段和“产品状态”查找字段，则会删除以下内容：

   * 营销活动中的已连接产品字段
   * 营销活动中的产品状态查找字段
   * 产品中的“Campaign已连接”字段

  有关详细信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* 不能从全局记录中删除已从辅助工作区添加到辅助工作区的字段。

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

1. <span class="preview">（视情况而定）如果您要删除的字段是请求表单的一部分，则显示&#x200B;**删除字段**&#x200B;框以指示将受到更改影响的表单。 执行以下操作之一：</span>

   <div class="preview">

   * 单击向右箭头以显示受更改影响的表单，然后单击表单名称以在新选项卡中打开表单并决定是保留表单上的字段还是对表单进行其他更改。
   * 单击&#x200B;**删除**，这将从显示字段的所有区域删除该字段。

   </div>

   无法恢复已删除的字段。

   根据您删除的字段类型，会发生以下情况：

   * 如果删除属于所选记录的字段，则该字段会被删除，并且无法再与任何记录相关联。 如果此字段作为查找字段添加到其他记录中，则这些字段也会被删除。
   * 如果删除连接字段，则该字段将从您选择的记录中删除。 此外，其原始记录中的对应连接字段也被删除。
   * 如果删除从已连接记录中添加的查找字段，则该字段将从您选择的记录类型中删除，但它将保留在其原始记录类型中。
   * 如果从全局记录类型的主工作区中删除字段，则该字段会从已添加该记录类型的所有工作区中删除。 不能从全局记录类型的辅助工作区中删除字段。
