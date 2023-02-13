---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 将项目添加到Adobe Workfront目标中的目标
description: 您可以将项目连接到目标，以根据项目的实际进度指示目标的进展情况。 项目将成为目标的进度指标。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# 将项目添加到Adobe Workfront目标中的目标

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

您可以将项目连接到目标，以根据项目的实际进度指示目标的进展情况。 项目将成为目标的进度指标。

通过将项目与目标相连，您可以将贵组织的战略规划（目标）与您的人员正在执行的实际工作联系起来，并每天完成（项目）。

>[!IMPORTANT]
>
>在项目的“业务案例”区域中创建的项目级目标与在Workfront目标中创建的战略目标无关。 有关业务案例项目目标的信息，请参阅 [创建业务案例目标](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## 访问要求

<!--drafted for P&P release: replace the table below with this: 

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
   <td> <p>编辑对目标的访问权限</p> <p><b>注释</b>

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

有关访问Workfront目标的其他信息，请参阅 [使用Workfront目标的要求](../goal-management/access-needed-for-wf-goals.md).

## 有关将项目连接到目标的注意事项

* 您可以向目标添加符合以下标准的项目：

   * 您必须至少拥有查看该页面的权限。

      >[!NOTE]
      >
      >如果在将项目附加到目标后您失去了查看项目的权限，则仍可以查看有关该目标的项目信息，但无法再访问该项目。

   * 项目不得处于“已停用”状态。

* 您可以将多个项目与一个目标关联。
* 您可以将同一项目与多个目标相关联。
* 您无法从项目附加到的目标手动更新项目的进度。 相反，Workfront会计算项目完成百分比，Workfront目标会使用此完成百分比计算目标进度。 这会在项目百分比更新后实时更新目标。
* 项目持续时间可以超出目标的时间段。 如果项目持续的时间超过目标的截止时间，您仍可以关闭目标并将其视为已完成，但目标完成百分比不会是100%。 项目完成百分比不再更新目标。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 删除附加到目标的项目时，也会从目标中删除该项目。

   >[!CAUTION]
   >
   >如果目标在您删除项目之前处于活动状态且该目标没有其他进度指标，则该目标将变为“不活动”。


## 将项目添加到目标

1. 单击 **主菜单** ![](assets/main-menu-icon.png) (为Shell起草此内容：或单击 **主菜单** ![](assets/three-line-main-menu-icon.png) （如果可用），则 **目标**.
1. 在目标列表中，单击目标名称以打开目标页面。
1. 单击 **进展指标** 中。
1. 从 **新进展指标** 下拉菜单中，单击 **添加现有项目**.

   此时会显示将项目添加到目标框。
1. （可选）更新 **查看**, **过滤器**&#x200B;或 **分组** 单击列表右上角的相应图标可修改项目列表的显示方式。
1. （可选）单击 **搜索** 图标 ![](assets/search-icon.png) 然后开始键入项目的名称，以便快速在列表中找到该项目。
1. 选择要添加到目标的项目，然后单击 **添加**.

   所选项目将添加到目标，并会显示在目标页面进度指示器部分(位于 **项目** 分组。

   在您激活目标后，当项目进度更新时，目标的进度会自动更新。 有关激活目标的信息，请参阅 [在Adobe Workfront目标中激活目标](../goal-management/activate-goals.md).

## 查找有关目标的项目信息

<p>
在目标页面的“进度指标”部分的目标级别，可看到以下项目信息：

</p>

<table>
  <tr>
   <td>项目名称
   </td>
   <td>项目名称中的任何更改也会反映在连接的项目中。
   </td>
  </tr>
  <tr>
   <td>项目所有者
   </td>
   <td>项目所有者中的任何更改也会反映在连接的项目中。
   </td>
  </tr>
    <tr>
   <td>实际进度
   </td>
   <td> <p>项目完成百分比。 您无法手动更新目标中的项目完成百分比。 Workfront会根据任务完成百分比自动计算该值。 </p>
   </td>
  </tr>
  <tr>
   <td>进度
   </td>
   <td>项目完成百分比，由条形图表示。 项目完成百分比的任何更改都会自动更新目标进度，除非目标已关闭。
   </td>
  </tr>

</table>

## 查找有关项目的目标信息

以下目标信息在项目列表或报表中可见：

| 目标信息 | 描述 |
|---|---|
| 目标 | 所有目标列表，其中包含与其关联的项目。 |
| 目标层次结构 | 目标所属的层次结构。 此字段中仅显示目标和目标的父项。 不显示子项目标。 |
| 链接目标的数量 | 链接到一个项目的目标数。 |
