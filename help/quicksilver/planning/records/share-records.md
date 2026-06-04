---
title: 使用链接共享记录
description: 您可以与其他人共享记录以提高协作能力。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ct6I5wnivCVr3V86Zj4F7stm2IVUJVH50yvTRyWFuUA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a93c6c9faf26d5eab1c223bd4a2646af896bf97d
workflow-type: tm+mt
source-wordcount: 721
ht-degree: 0%

---

<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# 使用链接共享记录

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

要与其他用户协作，您可以与他人共享记录。

您可以通过以下方式共享Adobe Workfront Planning记录：

* 打开记录页面时，从浏览器复制该页面的链接。

* 在记录类型的表视图中查看记录时，复制指向记录页面的链接。

* 在生产环境中：

   * 通过共享工作区和记录类型，您可以与其他用户共享工作区中的所有记录。

     有关更多信息，请参阅以下文章：

      * [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

      * [共享记录类型](/help/quicksilver/planning/access/share-record-types.md)

<div class="preview">

* 在“预览”环境中：

   * 您可以与人员、团队、角色、组或公司共享单个记录。

     有关信息，请参阅[共享记录](/help/quicksilver/planning/access/share-records.md)。

</div>



<!--take out the sentence below when we release record-level sharing-->

本文介绍了如何从记录类型的表视图中复制指向记录页面的链接。

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
<p>任何Workfront和任何Planning包</p> <p>任何工作流和任何计划包</p>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>参与者或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>查看工作区或更高权限以及使用链接共享记录的记录类型</p>
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
   <td><p> Contributor or higher license </p>
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
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>
-->


## 从记录类型表格视图中共享记录链接

{{step1-to-planning}}

您上次访问的工作区随即打开。

1. 单击记录类型卡片。

   此时将打开记录类型页面。

1. （视情况而定）从表右上角的&#x200B;**视图**&#x200B;下拉菜单中，选择一个表视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。

1. 右键单击记录行

   或

   将鼠标悬停在记录名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**复制链接**。

   ![记录行的上下文菜单](assets/contextual-menu-for-record-row.png)

   该链接将会复制到您的剪贴板中。

1. 将链接粘贴到电子邮件或聊天窗口中，以便与其他用户共享。 当用户收到链接时，将打开记录页面。

   >[!TIP]
   >
   >记录页面中的字段与记录的“表”视图中可用的字段相同。


   <!--add there when it will be available: if they have access to this record-->

## 通过共享工作区来共享工作区中的所有记录

与他人共享工作区时，您可以共享工作区中的所有记录。

默认情况下，记录类型和记录从工作区继承相同的权限。

只有对工作区具有管理权限的用户才能与他人共享该工作区。

有关详细信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)。

## 通过共享记录类型共享记录类型中的所有记录

默认情况下，记录从记录类型继承权限。

默认情况下，记录类型从工作区继承权限。

但是，您可以执行以下任一操作：

* 禁用从工作区继承的记录类型权限。 这将删除对记录的更高权限，但保留对工作区、记录类型和记录的查看权限。
* 手动将权限授予记录类型的用户，即使他们无权访问工作区。 这将自动授予他们查看工作区的权限。 默认情况下，这将授予用户对记录的查看权限。

只有对工作区具有管理权限的用户才能与其他人共享其记录类型和记录。

有关详细信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。

<div class="preview">

## 共享个人记录

默认情况下，用户从工作区和记录类型继承记录权限。

要仅向具有记录类型权限的select用户授予仅管理某些记录的权限，您可以禁用对选定记录的继承权限，并仅向这些用户授予对这些记录的“管理”访问权限。

您可以批量调整一个记录的权限，或同时调整多个记录的权限。

有关详细信息，请参阅[共享记录](/help/quicksilver/planning/access/share-records.md)。

</div>

