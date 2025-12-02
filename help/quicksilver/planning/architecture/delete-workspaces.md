---
title: 删除工作区
description: 如果工作区不再相关，您可以将其删除。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---


# 删除工作区

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

在Adobe Workfront Planning中，工作区是团队计划工作的集中位置。 有关详细信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

您可以删除不再相关的工作区。

我们建议在删除工作区之前，在其他工作区中重新创建与您要删除的工作区相关联的部分或全部记录类型、记录、字段和视图。

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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 有关删除工作区的注意事项

* 删除工作区时，也会删除所有记录类型、记录、其字段和视图。
* 已删除的工作区及其包含的信息无法恢复。

## 删除工作区

{{step1-to-planning}}

1. （视情况而定）如果您是Workfront管理员，请单击&#x200B;**我所在的工作区**&#x200B;以访问您创建的工作区，或单击&#x200B;**其他工作区**&#x200B;以访问他人与您共享的工作区。

1. （可选）单击&#x200B;**显示全部**&#x200B;以显示其他工作区。 仅当您拥有两行以上的工作区信息卡时，才会显示&#x200B;**显示所有**&#x200B;链接。
1. （可选） ClicK **显示更少**&#x200B;以限制屏幕上显示的工作区数。
1. 要删除工作区，请执行下列操作之一：

   * 将鼠标悬停在工作区信息卡上，然后单击该信息卡右上角的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)
或<!--Add this to the bullet below: <span class="preview">Search for a workspace by name and </span>-->
   * 单击工作区卡以打开工作区，然后单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)。
1. 单击&#x200B;**删除**。

   ![永久删除工作区确认](assets/permanently-delete-workspace-confirmation.png)

1. 在提供的空间中键入“**delete**”，然后单击&#x200B;**永久删除**。 不区分大小写。

   工作区已被删除，无法恢复。 任何与其关联的记录类型、记录、字段和视图也会被删除。<!--ensure this is right at or before GA-->
