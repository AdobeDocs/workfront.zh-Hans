---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中激活目标
description: 在创建目标时，Adobe Workfront目标会将其保存为草稿。 起草的目标不是目标管理的一部分。
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 1%

---

# 在Adobe Workfront目标中激活目标

<!--Audited for P&P only: 4/2025-->

在创建目标时，Adobe Workfront目标会将其保存为草稿。 起草的目标不是目标管理的一部分。

要跟踪您通过更新进度接近目标的程度，您必须激活目标。 这会将它的状态更改为“活动”。

有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>您必须先激活目标，然后才能更新其结果和活动的进度。


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
 <td role="rowheader">访问级别配置</td>
 <td> <p>编辑对目标的访问权限</p> </td>
 </tr>
 <tr>
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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## 先决条件

要激活目标，需要将该目标与活动、结果、项目等进度指示器关联，或者将其与其他活动目标对齐。

请至少执行以下操作之一，以便能够激活目标：

* 将结果添加到目标

  有关信息，请参阅[在Adobe Workfront目标中添加结果](../../workfront-goals/results-and-activities/add-results-to-goals.md)。

* 将活动添加到目标

  有关信息，请参阅[在Adobe Workfront目标中添加活动](../../workfront-goals/results-and-activities/add-activities-to-goals.md)。

* 将项目连接到目标

  有关信息，请参阅[在Adobe Workfront目标中添加项目](../results-and-activities/connect-projects-to-goals-overview.md)。

* 将另一个目标与要激活的目标保持一致

  有关信息，请参阅[通过在Adobe Workfront目标中连接目标来调整目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

## 激活目标

您可以激活已创建的目标或您对其具有管理权限的目标。

1. 转到要激活的目标。 此时将打开目标页面。

1. 单击目标名称右侧的&#x200B;**更多**&#x200B;菜单![更多图标](../goal-management/assets/more-icon.png)，然后单击&#x200B;**激活**。

   ![更多菜单已展开](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   目标状态将更改为“活动”。 您现在可以跟踪目标的进度，目标显示在签入部分中，并且在Workfront目标的图形部分中会被考虑
