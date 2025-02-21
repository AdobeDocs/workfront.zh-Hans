---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 将活动添加到Adobe Workfront目标中的目标
description: 活动衡量目标的进度。 如果没有关联的结果、活动或一致的目标，则无法激活目标，并且无法记录其进度。
author: Alina
feature: Workfront Goals
exl-id: 4d6ef324-4b5c-402b-b64d-b1a2a7d2ab57
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 1%

---

# 将活动添加到Adobe Workfront目标中的目标

活动衡量目标的进度。 如果不关联结果、活动、项目或瞄准的目标，则无法激活目标，也无法记录相关进度。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> 
   <p>对于新计划和许可证结构：
  <ul><li>Ultimate计划 </li></ul>
   </p>
<p>对于当前计划和许可证结构： 
<ul><li> Pro或更高版本 </li>
  <li>除了Adobe Workfront许可证之外，还提供了Workfront目标许可证。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证*</td>
 <td>
 <p>新许可证：参与者或更高版本</p>
 或
 <p>当前许可证：请求或更高版本</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
 <p> 新产品要求，为以下项之一： </p>
<ul>
<li>Select或Prime Adobe Workfront计划和附加Adobe Workfront Goals许可证。</li>
<li>Ultimate Workfront计划，默认情况下包括Workfront目标。 </li></ul>
 <p>或</p>
 <p>当前产品要求： Workfront计划和Adobe Workfront Goals的附加许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">访问级别*</td>
 <td> <p>编辑对目标的访问权限</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的权限或更高以查看目标</p>
  <p>管理目标的权限以编辑它</p>
  <p>有关共享目标的信息，请参阅<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

您必须具有现有目标才能向其添加活动。

有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。

>[!IMPORTANT]
>
>一个目标最多只能包含1000个活动、结果或一致的目标。

有关活动的更多信息，请参阅[Adobe Workfront目标中的结果和活动入门](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)。

## 将活动添加到目标

<!--
Adding activities to goals differs depending on which environment you use.

### Add an activity to a goal in the Production environment

1. Go to the goal for which you want to add an activity and click the name to open the **Goal Details** panel.
1. Click **Add activities**.

   ![Add activity inside goal](assets/add-activity-inside-goal-details-highlighted-350x152.png)

1. From the **Activity Type** drop-down menu, select the type of activity you want to associate with your goal.&nbsp;Select **Manual progress bar** or **Project**. Manual progress bar is the default selection. 
1. (Conditional) Depending on which activity type you selected, do the following:

   1. If you selected **Manual progress bar**:

      1. Start typing a name for your activity in the **Activity** field. 
      1. (Optional) If you want to set the activity owner as someone other than yourself, click your name in the **Owner** field and begin typing the name of the user that you want to assign as the activity owner, then click it when it appears in the drop-down list.

         >[!NOTE]
         >
         >You cannot assign a team or group as an activity owner.

         When you update the progress of an activity, the progress of the goal automatically updates.

   1. If you selected **Project**:

      1. Click the **Connect projects** field.

         Existing projects that you have access to View display in the Connect projects list. Projects that are in a status of Dead do not display in the list. 
      
      1. Click the name of a project to add it as an activity to the goal. You can select several projects at one time.

         Workfront uses the project percent complete of all the attached projects to calculate the progress of the goal.

         For more information about associating projects with goals, see [Add projects to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

         >[!TIP]
         >
         >   
         >   * The owner of the project becomes the owner of this activity. If the project has no owner, then the activity has no owner. 
         >   * You cannot manually update the progress of a project. Workfront calculates the progress of the project based on the project percent complete. When the project percent complete updates in Workfront this also updates the connected project in Workfront Goals including the percent complete of the goal. 
         >   
         >

1. Click **Save**.

   The activity is saved for the selected goal. After you activate the goal, the progress of the goal automatically updates when you update the progress of an activity or when the percent complete of a project updates. For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

-->


1. 单击&#x200B;**主菜单** ![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。
1. 从目标列表中，单击目标的名称以打开目标的页面。
1. 单击左侧面板中的&#x200B;**进度指示器**。
1. 从“新建进度指示器”下拉菜单中，单击&#x200B;**创建活动**。

   将打开“新建活动”框。

   ![新活动框](assets/new-activity-box-unshimmed.png)

1. 在活动名称字段中输入活动的名称。 这是必填字段。
1. （可选）如果要将活动分配给其他用户，请从&#x200B;**活动所有者**&#x200B;字段中移除您的名称。 默认情况下，您是所创建活动的所有者。

   >[!NOTE]
   >
   >您不能将团队、组或公司分配为活动所有者。

1. 单击&#x200B;**创建活动**&#x200B;以保存该活动并将其添加到所选目标。

   活动显示在目标页面的进度指示器部分中的活动分组下。





