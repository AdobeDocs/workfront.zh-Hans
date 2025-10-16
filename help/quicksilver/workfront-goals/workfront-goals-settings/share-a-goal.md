---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: 在Workfront目标中共享目标
description: 当您共享目标时，您会将目标的管理权限授予未创建该目标的人员。
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 5%

---

# 在Adobe Workfront目标中共享目标

当您共享目标时，您会将目标的管理权限授予未创建该目标的人员。

## 访问要求

>[!NOTE]
>
>如果您的公司以前购买过此包，则可能会选择继续使用Adobe Workfront Goals。 有关详细信息，请与您的客户代表联系。
>
>Adobe Workfront目标不再可供购买。

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront包</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证</td>
 <td>
 <p>参与者或更高版本</p>
<p>请求或更高版本</p></td>
 </tr>
  <tr>
 <td role="rowheader">访问级别配置</td>
 <td> <p>编辑对目标的访问权限</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的权限或更高以查看目标</p>
  <p>管理目标的权限以编辑它</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括系统管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 有关共享目标的注意事项

* 用户可以对目标具有以下权限：

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
      <td role="rowheader"><p>视图</p></td> 
      <td>
      <p>用户有权查看目标，但他们不能编辑目标的信息，不能添加或编辑结果或活动的信息，不能更新状态或删除目标。</p>      
      <p>默认情况下，所有有权访问“目标”的用户都可以查看系统中的所有目标。 如果用户在访问级别具有对目标的编辑访问权限，则可以复制目标。</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>管理</p></td> 
      <td> <p>用户可以编辑目标的所有信息（包括结果或活动），包括删除这些信息。</p> 
      <p>只有目标创建者或明确授予目标管理权限的用户才能管理目标。</p> 
      只有对目标具有管理权限的用户才能与他人共享目标，以便他们获得目标的管理权限。 </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 您可以与其他人共享以下类型的目标：

   * 您创建的目标
   * 由您有权管理的其他人创建的目标。

* 如果您具有目标的管理权限，则可以更改目标创建者的目标权限。 默认情况下，他们在创建目标时拥有管理权限，但您可以将他们的权限更改为“查看”。

## 共享目标

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png) > **目标**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   此时将显示“目标列表”。

1. 单击列表中目标的名称。 此时将打开目标页面。

1. 单击目标名称旁边的&#x200B;**更多图标**，然后单击&#x200B;**共享**。

   ![更多菜单](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   此时将显示“目标访问”框。

   ![目标访问权限](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 执行下列操作之一：

   * 选择&#x200B;**管理系统范围**&#x200B;设置，将管理权限授予系统中对其访问级别中的目标具有编辑访问权限的每个人。 默认情况下，所有新目标均会取消选择此选项。
   * 开始在&#x200B;**将管理权限授予**&#x200B;框中键入要为其授予管理权限的用户名称。 当其名称出现在列表中时选择该名称。

     >[!TIP]
     >
     >您只能与其他用户共享目标。 您无法与组、团队或您的公司共享目标。

1. 单击&#x200B;**共享**。

   目标将与您指定的用户共享。 “系统范围”标签或具有目标管理权限的用户名称将显示在目标详细信息面板的访问管理字段中。

## 目标权限选项

下表列出了在共享目标时可以授予的权限。 有关用户根据其许可证获得的访问权限的详细信息，请参阅[授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)。

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
   <td>查看添加为活动的项目** </td> 
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
   <td>添加目标的结果或活动</td> 
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
   <td>从目标断开项目连接</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*您必须拥有访问级别中目标的“编辑”访问权限，才能将结果和活动转换为目标。

**您必须具有查看项目的访问权限，以及对已添加或要添加到目标以查看项目的查看权限。

有关项目访问级别的信息，请参阅[授予项目访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

有关项目权限的信息，请参阅[在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

 
