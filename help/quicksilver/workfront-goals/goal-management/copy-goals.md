---
product-previous: workfront-goals
navigation-topic: goal-management
title: 复制Adobe Workfront目标中的目标
description: 您可以复制Adobe Workfront目标中的目标以创建目标。 一些原始目标信息会传输到新目标。
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 复制Adobe Workfront目标中的目标

您可以复制Adobe Workfront目标中的目标以创建目标。 一些原始目标信息会传输到新目标。

## 访问要求

<!--drafted for P&P release: 

You must have the following:

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
   <td> <p>编辑对目标或更高版本的访问权限</p> <p><b>注释</b>

<p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
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
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 复制目标的注意事项

您必须在访问级别中拥有编辑目标的访问权限，然后才能复制目标。 有关授予对Goals的访问权限的信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

您可能希望复制现有目标的一些原因包括：

* 在时间段（季度或年）结束时，您希望为下一时间段重新创建相同目标。
* 在时间段结束时，当目标无法完成，并且您想要在另一个时间段内处理目标。
* 当多个团队成员具有相似的目标，并且您可能需要为每个成员创建一个目标时。

>[!TIP]
>
>您可以复制任何状态的目标。 有关目标状态的信息，请参阅 [Adobe Workfront目标中的目标状态概述](../../workfront-goals/goal-management/goal-status-overview.md).

复制目标时请考虑以下事项：

* 有关目标的所有信息也会复制到新目标。
* 您可以选择复制现有目标的结果。 将结果的名称传输到新目标，但现有目标上的结果当前进度不会复制到新目标。 默认情况下，复制的结果会分配给同一所有者。

   >[!NOTE]
   >
   >如果原始所有者从Workfront中删除或停用，则会将新结果分配给已登录的用户。

* 在复制目标时，您无法复制目标的活动。

## 复制目标

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. 转到目标并单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **复制目标**.

   ![](assets/copy-goal-box-unshimmed.png)

1. 更新已复制目标的以下信息：
   * **目标名称**:新目标的名称。 复制的目标的默认名称为“ &lt;original goal=&quot;&quot;>&quot;
   * **句点**:您想要实现目标的时间段。 从下拉菜单中选择时间段

      或

      选择 **启用自定义日期** 为目标指定自定义日期 **开始** 和 **结束日期**. 默认情况下，启用自定义日期设置处于禁用状态。

      >[!TIP]
      >
      >   取消选择启用自定义日期将还原为原始目标的时间段。

      * **目标所有者**:目标所有者。 它可以是用户、团队、组或公司。 默认为原始目标的所有者。
      * **描述**:有关目标的其他信息。
      * **复制结果**:如果要将结果从当前目标转移到复制的目标，请选择此选项。 此操作会复制原始结果，并将其附加到复制的目标。 复制目标的结果与原始目标的结果具有相同的所有者、名称和测量值。

         >[!NOTE]
         >
         >* 原始结果的进度不会转移到复制的目标。
         >* 如果原始所有者从Workfront中删除或停用，则会将新结果分配给已登录的用户。


1. 单击 **复制目标**.

   将创建与原始目标类似的目标，该目标处于“草稿”状态。

   >[!NOTE]
   >
   >如果尚未复制原始目标的结果，则必须先将新目标与进度指示器关联，然后才能激活新目标并开始努力实现它。
   >有关将目标与进度指标关联的信息，请参阅以下文章：
   >* [将结果添加到Adobe Workfront目标中的目标](../results-and-activities/add-results-to-goals.md)
   >* [将活动添加到Adobe Workfront目标中的目标](../results-and-activities/add-activities-to-goals.md)
   >* [在Adobe Workfront目标中通过将目标连接起来来调整目标](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >有关激活目标的信息，请参阅 [激活目标](../goal-management/activate-goals.md).

