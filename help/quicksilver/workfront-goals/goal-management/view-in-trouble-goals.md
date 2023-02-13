---
product-previous: workfront-goals
navigation-topic: goal-management
title: 查看Adobe Workfront目标中的问题解决目标
description: 《有麻烦的进展》有不可能实现的危险，以《Adobe Workfront目标》中的红色进展栏为代表。 您应该经常查看您的目标，并了解进度为何滞后。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# 查看Adobe Workfront目标中的问题解决目标

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

《有困难进展的目标》有不能实现的危险，以《Adobe Workfront目标》中的红色进展栏为代表。 您应该经常查看您的目标，并了解进度为何滞后。 有关目标进度的信息，请参阅 [Adobe Workfront目标中的目标进度和条件概述](../../workfront-goals/goal-management/calculate-goal-progress.md).

## 访问要求

<!--drafted for P&P release: replace the existing requirements with this:

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
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## Recommendations阻止目标实现

在目标达到“处于危险中”进度之前，您可以经常监控目标并在目标达到“处于危险中”进度时调整其进度。 面临风险的目标有陷入麻烦的危险。 有关目标进度的更多信息，请参阅 [Adobe Workfront目标中的目标进度和条件概述](../../workfront-goals/goal-management/calculate-goal-progress.md)

在您的目标实现“遇到麻烦”进度之前，我们建议您执行以下操作：

* 审核通常具有“处于风险”条件的目标，这些目标会分配给您，以及分配给您的团队、组或您的组织的组织目标，这些目标可能会因目标进度而受到影响。 风险目标有可能成为麻烦目标。 风险目标上标有黄色进度条。 使用目标列表可查看属于您、您的团队、组或您组织的目标。


## 查看目标列表中的故障诊断目标

您可以查看“Workfront目标”的任何部分中的目标。 有关Workfront目标部分的信息，请参阅 [Adobe Workfront目标部分概述](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

本文介绍了如何查看目标列表中的目标。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 中。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   此时将打开Workfront目标区域，默认情况下将显示目标列表部分。

1. （推荐）调整“目标列表”区域的以下过滤器，以审查风险目标：

   * 单击 **公司**，则 **我的团队**，则 **我的组**，则 **个人** 目标，以便查看属于您的组织、团队、群组的目标，然后查看您自己的目标。

      >[!TIP]
      >
      >在Adobe Workfront目标中，公司过滤器会显示选择贵组织作为其所有者的目标。
      >
      >
      >您无法使用此字段搜索公司。 默认情况下，只会选择拥有您的Workfront实例的组织。

   * 对于您在上面选择的每个组织单位，单击 **新建过滤器** > **进度** > **遇到麻烦** >**应用。**
   * （可选）选择要查看其目标的时间段。

      对于目标列表中的每个目标，进度条指示器以红色显示。

      有关使用右侧面板中的所有其他标准过滤目标的更多信息，请参阅 [在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 将鼠标悬停在进度条指示器上，可查看当天的实际进度百分比和预期值。

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （可选）使用过滤器查找属于特定所有者的目标。

   目标列表中会显示选定用户的故障诊断目标。

1. 单击目标名称以打开目标页面，然后单击 **进展指标** 中。 在 **实际进度** 列。

   有关更新结果和活动的信息，请参阅 [更新Adobe Workfront目标中的目标进度](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >您只能更新“进度指标”列表中的结果和活动。 您必须通过访问这些目标来更新子目标的进度指标，并且必须更新连接项目的任务以更新项目的进度。


