---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中复制目标
description: 您可以复制Adobe Workfront目标中的目标以创建目标。 一些原始目标信息传输到新目标。
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 4%

---

# 在Adobe Workfront目标中复制目标

<!--Audited for P&P only: 4/2025-->

您可以复制Adobe Workfront目标中的目标以创建目标。 一些原始目标信息传输到新目标。

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

## 复制目标的注意事项

在复制目标之前，您必须拥有在访问级别中编辑目标的访问权限。 有关授予目标访问权限的信息，请参阅[授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)。

您可能希望复制现有目标的一些原因包括：

* 在时段（季度或年）结束时，希望为下一时段重新创建相同的目标。
* 在时段结束时，当目标无法完成，并且您想在另一个时段中处理它时。
* 当多个团队成员具有相似目标时，您可能需要为每个团队成员分别创建一个目标。

>[!TIP]
>
>您可以复制处于任何状态的目标。 有关目标状态的信息，请参阅Adobe Workfront目标中的[目标状态概述](../../workfront-goals/goal-management/goal-status-overview.md)。

复制目标时，请考虑以下事项：

* 有关目标的所有信息也会复制到新目标。
* 您可以选择复制现有目标的结果。 结果名称将传递到新目标，但现有目标上的结果的当前进度未复制到新目标。 默认情况下，复制的结果将分配给同一所有者。

  >[!NOTE]
  >
  >如果从Workfront中删除或停用原始所有者，则会将新结果分配给登录用户。

* 复制目标时，无法复制目标的活动。

## 复制目标

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Copy**. 

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


1. 转到目标并单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**复制目标**。

   ![复制目标框](assets/copy-goal-box-unshimmed.png)

1. 为复制的目标更新以下信息：
   * **目标名称**：新目标的名称。 复制目标的默认名称是“&lt;原始目标>的副本”。
   * **时段**：您希望实现目标的时段。 从下拉菜单中选择一个时间段

     或

     选择&#x200B;**启用自定义日期**&#x200B;以指定目标的&#x200B;**开始**&#x200B;和&#x200B;**结束日期**&#x200B;的自定义日期。 默认情况下，“启用自定义日期”设置处于禁用状态。

     >[!TIP]
     >
     >   取消选择启用自定义日期将恢复到原始目标的时间段。

      * **目标所有者**：目标的所有者。 可以是用户、团队、组或公司。 其默认为原始目标的所有者。
      * **描述**：有关目标的其他信息。
      * **复制结果**：如果要将结果从当前目标传输到复制的目标，请选择此选项。 这将复制原始结果并将它们附加到复制的目标。 复制的目标的结果与原始目标的结果具有相同的所有者、名称和测量值。

        >[!NOTE]
        >
        >* 原始结果的进度不会转移到复制的目标。
        >* 如果从Workfront中删除或停用原始所有者，则会将新结果分配给登录用户。

1. 单击&#x200B;**复制目标**。

   将创建一个与原始目标相似的目标，且此目标处于“草稿”状态。

   >[!NOTE]
   >
   >如果您尚未复制原始目标的结果，则必须先将新目标与进度指示器关联，然后才能激活它并开始努力实现它。
   >有关将目标与进度指示器关联的信息，请参阅以下文章：
   >* [将结果添加到Adobe Workfront目标中的目标](../results-and-activities/add-results-to-goals.md)
   >* [将活动添加到Adobe Workfront目标中的目标](../results-and-activities/add-activities-to-goals.md)
   >* [通过在Adobe Workfront目标中连接目标来调整目标](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >有关激活目标的信息，请参阅[激活目标](../goal-management/activate-goals.md)。

