---
title: 复制记录视图
description: 如果要保留视图的多个版本，并在这些版本之间进行细微更改，则可以在Adobe Workfront Planning中复制视图。 本文介绍了如何复制视图。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FIfAFfkIRbEE44pf4I4JGF2i3pPHaFGBQjhSlU0Cxq8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 4378eb4b7272ac17b0fb6f2f2e77de2c0b272050
workflow-type: tm+mt
source-wordcount: 295
ht-degree: 2%

---

# 复制记录视图

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

如果要保留视图的多个版本，并在这些版本之间进行细微更改，则可以在Adobe Workfront Planning中复制视图。

复制视图会创建现有视图的相同副本。

原始视图的共享权限不会转移到复制的视图。

在Workfront Planning中，所有类型的视图的复制视图都是相同的。

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
<li><p>带规划包的任何Workfront或工作流</p></li>
或
<li><p>作为独立产品购买时的任何Planning包</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>工作流标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>规划标准</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理视图的权限</p>  
   <p>查看对视图的权限以临时更改视图设置或复制它。</p> </td> 
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
   <td> <p>You must add both a Workflow and a Planning license type to the access level when you have both a Workflow and a Planning package</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it.</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## 复制记录视图

{{step1-to-planning}}

1. 单击工作区的卡片。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
   默认情况下，所选类型的所有记录都会显示在表格视图中。

1. 单击当前视图名称旁边的下拉图标![下拉图标](assets/drop-down-icon.png)，将鼠标悬停在视图名称上，单击&#x200B;**更多**，然后单击&#x200B;**复制**。

   带有选项的视图上的![更多菜单](assets/more-menu-for-views-expanded-with-delete-option.png)

   视图重复，新视图的名称遵循以下模式： `Original view's name (Copy)`。 新的视图选项卡将显示在所有视图选项卡的末尾。
