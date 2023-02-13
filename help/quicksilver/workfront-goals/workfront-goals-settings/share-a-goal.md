---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: 在Workfront目标中共享目标
description: 当您共享某个目标时，您会为未创建该目标的人员授予“管理”该目标的权限。
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# 在Adobe Workfront目标中共享目标

当您共享某个目标时，您会为未创建该目标的人员授予“管理”该目标的权限。

## 访问要求

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>
-->

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront目标购买额外的许可证才能访问本文所述的功能。 </p> <p>有关信息，请参阅 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对目标或更高版本的访问权限</p> <p><b>注释</b><p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予对Adobe Workfront目标的访问权限</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <div> 
     <p>管理目标的权限</p> 
     <p>有关共享目标的信息，请参阅 <a href="#" class="MCXref xref selected">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 关于共享目标的注意事项

* 用户可以拥有以下目标权限：

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>目标权限</b></p></td> 
      <td>
      <p><b>描述</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>查看</p></td> 
      <td>
      <p>用户有权查看目标，但无法编辑目标的信息，无法添加或编辑结果或活动的信息、更新状态或删除目标。</p>      
      <p>默认情况下，所有有权访问“目标”的用户都可以查看系统中的所有目标。 如果用户在其访问级别中具有“编辑”目标访问权限，则用户可以复制目标。</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>管理</p></td> 
      <td> <p>用户可以编辑目标的所有信息，包括结果或活动的信息，包括删除这些信息。</p> 
      <p>只有专门为目标授予“管理”权限的目标创建者或用户才能管理目标。</p> 
      只有对某个目标具有“管理”权限的用户才能与他人共享该目标，以向他们授予该目标的“管理”权限。 </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 您可以与其他人共享以下类型的目标：

   * 您创建的目标
   * 您被授予“管理”权限的其他人创建的目标。

* 如果您拥有目标的“管理”权限，则可以更改目标创建者对目标的权限。 默认情况下，他们在创建目标时具有“管理”权限，但您可以更改其“查看”权限。

## 共享目标

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 中。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   此时将显示目标列表。

1. 在列表中单击目标的名称。 随即会打开目标页面。

1. 单击 **“更多”图标** 在目标名称旁边，单击 **共享**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   此时将显示“目标访问”框。

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 执行下列操作之一：

   * 选择 **管理系统范围** 设置，以向系统中在访问级别具有“编辑”目标访问权限的每个人授予“管理”权限。 默认情况下，所有新目标都将取消选中此选项。
   * 开始键入要在 **授予管理访问权限** 框中。 当名称显示在列表中时，选择该名称。

      >[!TIP]
      >
      >您只能与其他用户共享目标。 您不能与组、团队或公司共享目标。

1. 单击 **共享**.

   目标将与您指定的用户共享。 “目标详细信息”面板的“管理访问权限”字段中会显示“系统范围”标签或具有目标管理权限的用户名称。

## 目标权限选项

下表列出了在共享目标时可授予的权限。 有关用户根据其许可证获得的访问权限的更多信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>操作</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>查看</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>查看目标</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看结果或活动</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>复制目标* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>将结果或活动转换为其他目标*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>查看作为活动添加的项目** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>编辑目标</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑结果或活动</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>为目标添加结果或活动</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>将项目作为活动关联到目标**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>删除目标</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>删除结果或活动</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>断开项目与目标的连接</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必须在访问级别拥有“编辑”目标访问权限，才能将结果和活动转换为目标。

**您必须对已添加或要添加到目标中以查看项目的项目拥有“查看项目”和“查看”权限。

有关项目访问级别的信息，请参阅 [授予对项目的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

有关项目权限的信息，请参阅 [在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
