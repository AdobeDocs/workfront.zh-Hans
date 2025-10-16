---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 通过将结果和活动转换为目标来调整目标
description: 您可以手动对齐两个目标，也可以将现有目标的结果和活动转换为另一个目标。 转换后的结果或活动成为原始目标的子目标。 有关手动对齐两个目标的信息，请参阅在Adobe Workfront目标中通过连接来对齐目标。
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 17%

---

# 通过将结果和活动转换为目标来调整目标

<!--Audited P&P only: 4/2025-->

您可以手动对齐两个目标，也可以将现有目标的结果和活动转换为另一个目标。 转换后的结果或活动成为原始目标的子目标。
有关手动对齐两个目标的信息，请参阅[通过在Adobe Workfront目标中连接来对齐目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)。

## 访问要求

>[!NOTE]
>
>如果您的公司以前购买过此包，则可能会选择继续使用Adobe Workfront Goals。 有关详细信息，请与您的客户代表联系。
>
>Adobe Workfront目标不再可供购买。

+++展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Adobe Workfront包</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证</p> </td> 
   <td> <p>参与者或更高版本</p> 
     <p>申请人或以上</p> </td> 
  </tr>

<td><p>访问级别配置</p> </td> 
   <td> <p>编辑对目标的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>管理目标的权限</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括系统管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅[Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
   Or
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

在开始之前，您必须具备以下条件：

* 包含现有结果和活动的现有目标。

  有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>一个目标最多可以有1000个进度指示器。

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## 将结果和活动转换为目标时的注意事项

有时候，结果或活动的范围可能比预期的要大，因此更合理的做法是它们会成为目标。 您可以将现有目标的结果和活动转换为新目标。 这是一种自下而上的协调目标的方法。

将结果和活动转换为目标时，请考虑以下事项：

* 转换后的结果或活动成为原始目标的子目标，并且两个目标变得一致。
* 如果原始目标没有其他结果或活动，则新创建的目标将成为原始目标的单一进度指标。您必须将结果和活动添加到子目标中，以便能够跟踪其进度。
* 将结果或活动转化为目标是不可逆转的。一旦转换，新的子目标将永远不会再次成为父目标的结果或活动。

## 将结果或活动转化为目标

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. 转到具有结果的目标或要转换为目标的活动。
1. 从目标的页面，单击左侧面板中的&#x200B;**进度指示器**。
1. 在进度指示器列表中选择一个结果或活动，然后单击进度指示器列表顶部的&#x200B;**转换为目标**&#x200B;图标![转换为目标](assets/convert-to-goal-icon-unshimmed.png)。 “转换为目标”框打开。

   ![转换为目标框](assets/convert-to-goal-box-unshimmed.png)
1. 更新以下信息：
   * **目标名称**：默认情况下，新目标与原始结果或活动具有相同的名称。
   * **期间**：默认情况下，新目标的期间为当前季度。 您可以选择&#x200B;**启用自定义日期**&#x200B;设置来为新目标定义自定义时间段。
   * **目标所有者**：默认情况下，新目标所有者是原始结果或活动的所有者。
   * **描述**：添加有关新目标的更多信息。
1. 单击&#x200B;**保存**

   结果或活动现在转换为原始目标的子目标。 它在原始目标的进度指示器列表中列为目标。



