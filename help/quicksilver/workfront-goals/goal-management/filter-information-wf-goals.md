---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中筛选信息
description: 您可以查看您或其他任何人在Adobe Workfront目标中添加的目标。 有关创建目标的信息，请参阅在Adobe Workfront目标中创建目标。 在查看目标时，您可以过滤Workfront目标中的信息，以仅查看对您重要的目标。
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# 在Adobe Workfront目标中筛选信息

您可以查看您或其他任何人在Adobe Workfront目标中添加的目标。 有关创建目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md). 在查看目标时，您可以过滤Workfront目标中的信息，以仅查看对您重要的目标。

## 访问要求

<!--drafted - replace the table below with this one when P&P releases: 

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

您必须具有以下访问权限才能执行本文中描述的操作：

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
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高权限访问目标</p> <p><b>注释</b>

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
     <p>查看或更高权限</p> 
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## Workfront目标中的过滤器概述

>[!NOTE]
>
>为了高效查找并重点关注正确的目标，我们建议您在Workfront目标中使用过滤器。 这样，在开始管理对您而言非常重要的目标之前，您就可以显示正确的信息。 默认情况下，Workfront目标会显示系统中的所有目标。

您可以在Workfront的“目标”区域的以下部分中查找和筛选目标：

* 目标列表
* 图表
* 目标对齐方式

有关“目标”区域各节的信息，请参阅 [Adobe Workfront目标部分概述](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>您可以为一个部分配置过滤器，在移动到Workfront目标的其他部分时，这些过滤器会一直保留。

在Workfront目标中使用过滤器时，请考虑以下事项：

* 您可以创建并应用过滤器，而无需保存它，也可以保存过滤器以备以后重复使用。

   存在以下情形：

   * 保存过滤器后，每次登录Workfront目标时，该过滤器都会成为您的默认过滤器。
   * 在不保存的情况下应用过滤器时，可以通过刷新页面还原到原始列表。

* 您只能查看和应用您创建的过滤器。 其他用户创建的过滤器仅显示给这些用户。
* 您无法与其他用户共享您创建的过滤器。

## 在Workfront目标中应用快速过滤器

您可以在目标列表中使用快速过滤器来帮助您仅查找对您很重要的项目。 您无法保存快速过滤器，并且它们不是永久性的。 Workfront会在您刷新页面时清除快速过滤器的结果。

有关更多信息，请参阅 [将快速过滤器应用到列表](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## 在Workfront目标中创建并应用过滤器

对于Workfront目标的任何部分，创建过滤器的过程都是相同的。

您可以从头开始创建过滤器，也可以编辑其中一个内置过滤器。

1. 转到Workfront目标。

   有关访问Workfront目标的信息，请参阅 [访问和打开Adobe Workfront目标中的目标](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   默认情况下，将显示目标列表部分。

1. 单击 **过滤器** 列表右上角。

   ![](assets/filter-icon-and-label.png)

   默认情况下，Workfront会 **全部** 过滤器，该过滤器显示系统中的所有目标。

   >[!TIP]
   >
   >您无法编辑或删除“全部”筛选器。

1. 执行下列操作之一：

   * 单击以下任一预定义过滤器，可仅显示以下所有者的目标：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>全部</td> 
        <td> <p>系统中的所有目标，无论是谁创建了这些目标，目标的时间段是多少，还是所有者是谁。 这是默认过滤器，您无法对其进行编辑。 </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>个人的</td> 
        <td>您所拥有的目标。</td> 
       </tr> 
       <tr> 
        <td>我的团队</td> 
        <td> <p>选择您的任何团队作为所有者的目标。 </p> <p><b>笔尖</b>

      未将您分配给任何团队时，不会显示目标。 </p> </td>
      </tr> 
       <tr> 
        <td>我的组</td> 
        <td>选择您的任何群组作为所有者的目标。 </td> 
       </tr> 
       <tr> 
        <td>公司</td> 
        <td> <p>与您的组织关联的目标。 </p> <p><b>笔尖</b>
        <p>在Adobe Workfront目标中，公司过滤器会显示选择贵组织作为其所有者的目标。 </p> <p>您无法使用此字段搜索公司。 默认情况下，只会选择拥有您的Workfront实例的组织。 </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 将鼠标悬停在过滤器的名称上，然后单击 **编辑** 图标 ![](assets/edit-icon.png) 在其名称旁边以自定义该组，并添加用户、团队、组的特定名称或您的组织名称，然后在列表中显示时选择该组。

   * 单击 **新建过滤器** 要创建新过滤器，请从以下选项中选择以自定义新过滤器：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">期间</td> 
        <td>在下拉菜单中选择时间段。 您可以选择多个时间段。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">状态</td> 
        <td> <p>从下拉菜单中从以下选项选择状态：</p> 
         <ul> 
          <li> <p>活动</p> </li> 
          <li> <p>草稿</p> </li> 
          <li> <p>非活动</p> </li> 
          <li> <p>已关闭</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">进度</td> 
        <td> <p>从下拉菜单中选择进度： </p> 
         <ul> 
          <li> <p>存在问题</p> </li> 
          <li> <p>处于风险中</p> </li> 
          <li> <p>准时</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">所有者</td> 
        <td> <p>开始键入所有者的名称，然后在列表中显示时选择该名称。 </p> <p>您可以键入用户、团队、组的名称或组织的名称，也可以从预定义的选项中进行选择。 </p> <p>以下预定义过滤器选项始终指当前已登录的用户： </p> 
         <ul> 
          <li> <p><strong>我</strong>:显示您是所有者的目标。</p> </li> 
          <li> <p><strong>我的家队</strong> 和 <strong>我的所有团队</strong>:显示将您的主团队或任何团队指定为所有者的目标。 </p> <p>提示：未将您分配给任何团队时，不会显示目标。 </p> </li> 
          <li> <p><strong>我的家庭组</strong> 和 <strong>我的所有组</strong>:显示将您的主页群组或任何群组指定为所有者的目标。</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. （可选）单击 **重置** ，以清除您选择的所有字段，然后从头开始构建过滤器。
1. （可选）单击 **应用** 来应用过滤器，而不进行保存。

   过滤器显示在 **未保存** 过滤器生成器的区域作为 **新建过滤器**.

   无法重命名未保存的过滤器。

   下次从Workfront注销并重新登录时，未保存的过滤器将从“目标”区域中删除。

   >[!TIP]
   >
   >一次只能有一个未保存的新过滤器。

1. 单击 **保存** 要保存过滤器以便稍后使用，请在 **添加过滤器名称** 字段，单击 **完成**.

   这会将过滤器保存在 **已保存** 的子区域。 您以后可以使用此过滤器。

   默认情况下，下次您重新登录Workfront时，将显示最后保存并应用的过滤器

1. （可选）单击 **向左箭头** 下一页 **新建过滤器** 退出过滤器生成器并返回过滤器列表。
1. （可选）将鼠标悬停在自定义过滤器的名称上，单击 **更多** 菜单，然后单击 **删除**，则 **删除**. 这会删除过滤器，您将无法恢复该过滤器。

   >[!TIP]
   >
   >您无法删除任何预定义过滤器。

1. 单击 **X图标** 过滤器生成器的右上角以关闭过滤器生成器。

   当前应用的过滤器名称将显示在目标列表右上角的过滤器图标右侧。

   目标列表会按您的筛选条件进行筛选。

1. （可选和视情况而定）在“目标对齐”部分中查看目标时，单击 **给他们看** 如果您要查看已过滤的目标，请执行以下操作：

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   筛选器名称以黄色列出，表示被忽略。

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. （可选和视情况而定）单击 **重新应用过滤器** 以应用过滤器并忽略上一步中显示的项目。


