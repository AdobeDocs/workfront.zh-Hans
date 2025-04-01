---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中过滤信息
description: 您可以查看自己或其他人在Adobe Workfront目标中添加的目标。 有关创建目标的信息，请参阅在Adobe Workfront目标中创建目标。 在查看目标时，您可以过滤Workfront目标中的信息以仅查看对您很重要的目标。
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '1358'
ht-degree: 2%

---

# 在Adobe Workfront目标中过滤信息

<!--Audited for P&P only: 4/2025-->

您可以查看自己或其他人在Adobe Workfront目标中添加的目标。 有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。 在查看目标时，您可以过滤Workfront目标中的信息以仅查看对您很重要的目标。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <p> 新产品要求：Workfront</p>
  <p>或</p>
   <p>当前产品要求：除了Workfront许可证之外，您必须为Adobe Workfront Goals购买许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
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
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Workfront目标中的过滤器概述

>[!NOTE]
>
>要高效地查找并关注正确的目标，我们建议您在Workfront目标中使用过滤器。 这允许您在开始管理对您而言重要的目标之前显示正确的信息。 默认情况下，Workfront目标显示系统中的所有目标。

您可以在Workfront的“目标”区域的以下部分中查找并过滤目标：

* 目标列表
* 图表
* 目标对齐方式

有关“目标”区域的各个部分的信息，请参阅[Adobe Workfront目标部分的概述](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)。

>[!IMPORTANT]
>
>您可以为一个区域配置过滤器，在迁移到Workfront目标的另一个区域时，这些过滤器将保持持久性。

在Workfront目标中使用过滤器时，请考虑以下事项：

* 您可以创建和应用筛选器而不保存它，也可以保存筛选器以供以后重复使用。

  存在以下情况：

   * 保存过滤器后，它会在您每次登录Workfront目标时成为您的默认过滤器。
   * 应用筛选器而不保存它时，可以通过刷新页面还原为原始列表。

* 您只能查看和应用已创建的过滤器。 其他用户创建的过滤器仅对这些用户显示。
* 您无法与其他用户共享您创建的过滤器。

## 在Workfront目标中应用快速过滤器

您可以在目标列表中使用快速过滤器，以帮助您仅查找对您很重要的项目。 无法保存快速过滤器，因此它们不是永久性的。 在刷新页面时，Workfront会清除快速过滤器的结果。

有关详细信息，请参阅[将快速筛选器应用到列表](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

## 在Workfront目标中创建并应用过滤器

对于Workfront目标的任何部分，创建过滤器的过程都是相同的。

您可以从头开始创建过滤器，也可以编辑其中一个内置过滤器。

1. 转到Workfront目标。

   有关访问Workfront目标的信息，请参阅[在Adobe Workfront目标中访问和打开目标](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   默认情况下，将显示目标列表部分。

1. 单击列表右上角的&#x200B;**筛选器**。

   ![筛选器图标](assets/filter-icon-and-label.png)

   默认情况下，Workfront应用&#x200B;**全部**&#x200B;筛选器，该筛选器显示您的系统中的所有目标。

   >[!TIP]
   >
   >您无法编辑或删除“全部”筛选器。

1. 执行下列操作之一：

   * 单击以下任何预定义过滤器，以仅显示以下所有者的目标：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>全部</td> 
        <td> <p>您系统中的所有目标，无论这些目标的创建者、创建时间期限或所有者是谁。 这是默认筛选器，您无法对其进行编辑。 </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>个人的</td> 
        <td>您拥有的目标。</td> 
       </tr> 
       <tr> 
        <td>我的团队</td> 
        <td> <p>选择您的任何团队作为负责人的目标。 </p> <p><b>提示</b>

     如果您未分配到任何团队，则不会显示任何目标。 </p> </td>
     </tr> 
       <tr> 
        <td>我的组</td> 
        <td>选择您的任何组作为所有者的目标。 </td> 
       </tr> 
       <tr> 
        <td>公司</td> 
        <td> <p>与您的组织关联的目标。 </p> <p><b>提示</b>
        <p>在Adobe Workfront目标中，公司过滤器显示您的组织被选为所有者的目标。 </p> <p>您无法使用此字段搜索公司。 默认情况下，仅选择您拥有Workfront实例的组织。 </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * 将鼠标悬停在筛选器名称上，然后单击筛选器名称旁边的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)以自定义筛选器并添加特定用户、团队、组名称或您的组织名称，然后在用户出现在列表时选择它。

   * 单击&#x200B;**新建筛选器**&#x200B;以创建新筛选器，然后从以下选项中进行选择以自定义新筛选器：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">期间</td> 
        <td>在下拉菜单中选择一个时间段。 您可以选择多个时间段。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">状态</td> 
        <td> <p>从以下选项中选择下拉菜单中的状态：</p> 
         <ul> 
          <li> <p>活动</p> </li> 
          <li> <p>草稿</p> </li> 
          <li> <p>非活动</p> </li> 
          <li> <p>已关闭</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">进度</td> 
        <td> <p>从以下选项中选择下拉菜单中的进度： </p> 
         <ul> 
          <li> <p>存在问题</p> </li> 
          <li> <p>处于风险中</p> </li> 
          <li> <p>准时</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">所有者</td> 
        <td> <p>开始键入拥有者的名称，然后当该名称出现在列表中时将其选定。 </p> <p>您可以键入用户、团队、组的名称或组织的名称，也可以从预定义选项中进行选择。 </p> <p>以下预定义过滤器选项始终指当前登录的用户： </p> 
         <ul> 
          <li> <p><strong>我</strong>：显示您作为所有者的目标。</p> </li> 
          <li> <p><strong>我的主团队</strong>和<strong>我的所有团队</strong>：显示您的主团队或任何团队被指定为所有者的目标。 </p> <p>提示：当您未分配到任何团队时，不会显示任何目标。 </p> </li> 
          <li> <p><strong>我的主组</strong>和<strong>我的所有组</strong>：显示将主组或任何组指定为所有者的目标。</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. （可选）单击筛选器框右下角的&#x200B;**重置**&#x200B;以清除所有已选字段并从头开始构建筛选器。
1. （可选）单击&#x200B;**应用**&#x200B;以应用筛选器而不保存。

   筛选器在筛选器生成器的&#x200B;**未保存**&#x200B;区域显示为&#x200B;**新筛选器**。

   无法重命名未保存的筛选器。

   当您下次注销Workfront并重新登录时，未保存的过滤器将从“目标”区域中删除。

   >[!TIP]
   >
   >您一次只能有一个未保存的新筛选器。

1. 单击&#x200B;**保存**&#x200B;保存筛选器以稍后使用，然后在&#x200B;**添加筛选器名称**&#x200B;字段中添加筛选器的名称，然后单击&#x200B;**完成**。

   这会将筛选器保存在筛选器生成器的&#x200B;**已保存**&#x200B;部分中。 您以后可以使用此过滤器。

   默认情况下，在您下次重新登录Workfront时会显示上次保存并应用的过滤器

1. （可选）单击&#x200B;**新筛选器**&#x200B;旁边的&#x200B;**左指箭头**&#x200B;以退出筛选器生成器并返回筛选器列表。
1. （可选）将鼠标悬停在自定义筛选器的名称上，单击&#x200B;**更多**&#x200B;菜单，单击&#x200B;**删除**，然后单击&#x200B;**删除**。 这将删除筛选器，您无法恢复它。

   >[!TIP]
   >
   >您无法删除任何预定义过滤器。

1. 单击筛选器生成器右上角的&#x200B;**X图标**&#x200B;以关闭筛选器生成器。

   当前应用的筛选器的名称将显示在目标列表右上角的筛选器图标的右侧。

   目标列表按您的过滤条件过滤。

1. （可选且有条件）在“目标对齐方式”部分中查看目标时，如果要查看过滤掉的目标，请单击&#x200B;**显示它们**。

   ![显示过滤项上的链接](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   过滤器名称以黄色列出，表示它被忽略。

   ![过滤黄色轮廓](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. （可选且有条件）单击&#x200B;**重新应用筛选器**&#x200B;以应用筛选器并忽略您在上一步中显示的项。


