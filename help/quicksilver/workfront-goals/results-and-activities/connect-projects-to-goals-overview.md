---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 将项目添加到Adobe Workfront目标中的目标
description: 您可以将项目连接到目标，以根据项目的实际进度指示目标的进度。 项目会成为目标的进度指示器。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 1%

---

# 将项目添加到Adobe Workfront目标中的目标

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

您可以将项目连接到目标，以根据项目的实际进度指示目标的进度。 项目会成为目标的进度指示器。

通过将项目与目标连接，您可以将组织的战略计划（目标）与人员每天执行和完成的实际工作（项目）联系起来。

>[!IMPORTANT]
>
>在项目的业务案例区域中创建的项目级别目标不与Workfront目标中创建的战略目标相关联。 有关业务案例项目目标的信息，请参阅[创建业务案例目标](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。


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
  <ul><li>最终计划 </li></ul>
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
<li>Select或Prime Adobe Workfront计划和其他Adobe Workfront Goals许可证。</li>
<li>默认包含Workfront目标的Ultimate Workfront计划。 </li></ul>
 <p>或</p>
 <p>当前产品要求： Workfront计划和Adobe Workfront Goals的附加许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">访问级别</td>
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

## 有关将项目连接到目标的注意事项

* 您可以将满足以下条件的项目添加到目标中：

   * 您必须至少具有查看它的权限。

     >[!NOTE]
     >
     >如果在将项目附加到目标后失去了查看项目的权限，您仍可以看到目标上的项目信息，但您无法再访问项目。

   * 项目不得处于“停止”状态。

* 您可以将多个项目与一个目标关联。
* 您可以将同一项目与多个目标关联。
* 您无法从附加项目的目标中手动更新项目进度。 相反，Workfront计算项目的完成百分比，Workfront目标使用此完成百分比计算目标进度。 这会在项目百分比更新后实时更新目标。
* 项目持续时间可以超出目标的时间段。 如果项目的持续时间超过目标的截止日期，您仍可以关闭目标并认为它已完成，但目标完成百分比不会为100%。 项目的完成百分比不再在目标上更新。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 当您删除附加到目标的项目时，该项目也会从目标中删除。

  >[!CAUTION]
  >
  >如果在删除项目之前目标处于活动状态，且目标上没有其他进度指示器，则该目标将变为非活动状态。


## 将项目添加到目标

1. 单击&#x200B;**主菜单** ![](assets/main-menu-icon.png)(为Shell绘制此菜单：或单击左上角的&#x200B;**主菜单** ![](assets/three-line-main-menu-icon.png)（如果可用）。)，然后单击&#x200B;**目标**。
1. 从目标列表中，单击目标的名称以打开目标页面。
1. 单击左侧面板中的&#x200B;**进度指示器**。
1. 从&#x200B;**新建进度指示器**&#x200B;下拉菜单中，单击&#x200B;**添加现有项目**。

   此时会显示将项目添加到目标框。
1. （可选）通过单击列表右上角的相应图标来更新&#x200B;**视图**、**筛选器**&#x200B;或&#x200B;**分组**，以修改项目列表的显示方式。
1. （可选）单击&#x200B;**搜索**&#x200B;图标![](assets/search-icon.png)并开始键入项目名称以在列表中快速找到该项目。
1. 选择要添加到目标的项目，然后单击&#x200B;**添加**。

   选定项目将添加到目标，并显示在目标页面的&#x200B;**项目**&#x200B;分组下的进度指示器部分。

   激活目标后，当项目进度更新时，目标的进度会自动更新。 有关激活目标的信息，请参阅[在Adobe Workfront目标中激活目标](../goal-management/activate-goals.md)。

## 找到目标的项目信息

<p>
目标页面的进度指示器部分可在目标级别看到以下项目信息：

</p>

<table>
  <tr>
   <td>项目名称
   </td>
   <td>对项目名称所做的任何更改也会反映在连接的项目中。
   </td>
  </tr>
  <tr>
   <td>项目所有者
   </td>
   <td>项目所有者的任何更改也会反映在连接的项目中。
   </td>
  </tr>
    <tr>
   <td>实际进度
   </td>
   <td> <p>项目的完成百分比。 您无法从目标手动更新项目完成百分比。 Workfront会根据任务的完成百分比自动计算此值。 </p>
   </td>
  </tr>
  <tr>
   <td>进度
   </td>
   <td>用条形表示的项目完成百分比。 对项目完成百分比的任何更改都会自动更新目标进度，除非关闭目标。
   </td>
  </tr>

</table>

## 查找项目的目标信息

以下目标信息在项目列表或报表中可见：

| 目标信息 | 描述 |
|---|---|
| 目标 | 包含所有目标的列表，这些目标具有与其关联的项目。 |
| 目标层级 | 目标所属的层次结构。 只有目标和目标的父级会显示在此字段中。 子目标不显示。 |
| 链接的目标数 | 链接到某个项目的目标数。 |
