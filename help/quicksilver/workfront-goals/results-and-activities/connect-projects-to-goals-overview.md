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
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 1%

---

# 将项目添加到Adobe Workfront目标中的目标

<!--Audited for P&P only: 10/2025-->

您可以将项目连接到目标，以根据项目的实际进度指示目标的进度。 项目会成为目标的进度指示器。

通过将项目与目标连接，您可以将组织的战略计划（目标）与人员每天执行和完成的实际工作（项目）联系起来。

>[!IMPORTANT]
>
>在项目的业务案例区域中创建的项目级别目标不与Workfront目标中创建的战略目标相关联。 有关业务案例项目目标的信息，请参阅[创建业务案例目标](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)。


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
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
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

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 当您删除附加到目标的项目时，该项目也会从目标中删除。

  >[!CAUTION]
  >
  >如果在删除项目之前目标处于活动状态，且目标上没有其他进度指示器，则该目标将变为非活动状态。


## 将项目添加到目标

1. 单击&#x200B;**主菜单** ![主菜单图标](assets/main-menu-icon.png)(为Shell绘制此菜单：或单击左上角的&#x200B;**主菜单** ![主菜单行](assets/three-line-main-menu-icon.png)（如果可用）。)，然后&#x200B;**目标**。
1. 从目标列表中，单击目标的名称以打开目标页面。
1. 单击左侧面板中的&#x200B;**进度指示器**。
1. 从&#x200B;**新建进度指示器**&#x200B;下拉菜单中，单击&#x200B;**添加现有项目**。

   此时会显示将项目添加到目标框。
1. （可选）通过单击列表右上角的相应图标来更新&#x200B;**视图**、**筛选器**&#x200B;或&#x200B;**分组**，以修改项目列表的显示方式。
1. （可选）单击&#x200B;**搜索**&#x200B;图标![搜索图标](assets/search-icon.png)并开始键入项目名称以在列表中快速找到该项目。
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
