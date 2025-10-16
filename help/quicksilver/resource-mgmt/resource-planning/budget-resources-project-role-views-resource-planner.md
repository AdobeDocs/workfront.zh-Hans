---
product-area: resource-management
navigation-topic: resource-planning
title: 使用项目和角色视图的资源规划者中的预算资源
description: 您可以使用“项目”和“角色”视图在Adobe Workfront资源规划程序中预算资源。 您不能使用资源规划者中的用户视图预算资源。
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# 使用项目和角色视图的资源规划者中的预算资源

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

资源规划者的主要功能是为项目上必须完成的工作预算资源。

>[!IMPORTANT]
>
>只有在将&#x200B;**按项目查看**&#x200B;或&#x200B;**按角色查看**&#x200B;视图应用于资源规划者时，才能预算您的资源。

在资源规划者中开始预算信息之前，请参阅以下文章：

* [资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [资源规划者的“项目”和“角色”视图中的小时数、FTE和成本信息概览](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>编辑对资源管理的访问权限，包括访问资源规划者中的编辑优先级和预算小时数</p> <p>按成本编辑对预算资源的财务数据的访问权限</p> <p>编辑对项目和用户的访问权限</p></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td> <p>管理要为其编制预算信息的项目的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 资源规划者中的预算资源

* 项目视图中的[预算资源](#budget-resources-in-the-project-view)
* 角色视图中的[预算资源](#budget-resources-in-the-role-view)
* [批量预算资源](#budget-resources-in-bulk)

### 项目视图中的预算资源 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. 默认显示&#x200B;**规划者**。
1. （视情况而定）选择&#x200B;**按项目查看**&#x200B;视图。
1. 展开项目和工作角色以管理项目、工作角色或用户的分配。
1. 要为用户分配预算，请执行下列操作之一：

   * 在&#x200B;**BDG**&#x200B;列中，手动指定用户的预算小时数、FTE或成本。

   * 单击用户工作角色的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**将用户的计划小时数设置为预算**。\
     使用以下公式计算每个用户的预算小时数：

     `User Budgeted Hours = User Planned Hours`

1. 要分配工作角色的预算，请执行以下操作之一：

   * 在&#x200B;**BDG**&#x200B;列中，手动指定工作角色的预算小时数、FTE或成本。

     >[!NOTE]
     >
     >角色预算小时数已添加到项目预算小时数。

   * （视情况而定）如果您已为用户预算小时数，请单击工作角色的&#x200B;**更多**&#x200B;菜单，然后单击角色的&#x200B;**用户预算小时总数**。\
     使用以下公式计算每个角色的预算小时数：

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * 单击项目的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**将角色的计划小时数设置为预算**。\
     使用以下公式计算每个角色的预算小时数：\
     &#x200B;*

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* 角色预算小时数已添加到项目预算小时数。
     >* 可以为主角色和其他（或辅助）角色为用户预算。
     >* 用户角色的FTE可用性&#x200B;**百分比**&#x200B;必须为与0%不同的数字，以便可用小时数在资源规划者中显示工作角色的值。 如果用户与具有0% **FTE可用性百分比**&#x200B;的角色关联，则该工作角色的可用小时值为零。 在这种情况下，角色可能会显示负的&#x200B;**净值**。\
     >有关工作角色的FTE可用性&#x200B;**百分比**&#x200B;的详细信息，请参阅文章[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

   * 在&#x200B;**BDG**&#x200B;列中，手动指定项目的预算小时数、FTE或成本。 这会向项目下的每个角色分配项目预算小时数。 存在以下情况：

      * 如果您指定的项目预算小时数等于项目计划小时数，则角色预算小时数与角色计划小时数匹配。
      * 如果指定的项目预算小时数与项目计划小时数不相等，则根据每个角色所需的计划小时数百分比分配角色预算小时数。\
        例如，如果项目具有20个计划小时数，并且这些小时数分布在两个工作角色之间（顾问需要12个计划小时数，工程师需要8个计划小时数），而您为项目预算了30个小时数，则小时数分布如下：顾问角色接收18个预算小时数，工程师角色接收12个预算小时数。

1. 要为项目分配预算，请执行以下操作之一：

   * 对项目下的角色进行预算，如步骤7中所述。\
     项目预算小时数按以下公式计算：

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * 在&#x200B;**BDG**&#x200B;列中，手动指定项目的预算小时数、FTE或成本。\
     这将更新角色预算小时数，如步骤7中所述。\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. 单击&#x200B;**保存**。\
   在资源规划者中预算资源后，资源的预算小时数以及与资源相关的任何成本将列在每个项目的业务案例中。\
   有关了解Business Case的“资源预算”区域的更多信息，请参阅[Overview of the Area of the Business Case](../../manage-work/projects/define-a-business-case/areas-of-business-case.md)一文中的“Resource Budgeting”一节。

1. （可选）选择用户视图，以注意每个用户的可用小时数和计划小时数之间存在的任何用户过度分配或利用不足。 预算小时数在用户视图中不可见。

   有关Workfront如何计算用户可用性的信息，请参阅[配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

### 角色视图中的预算资源 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

您必须具有对资源管理和财务数据的编辑访问权限和管理项目的财务权限，才能在资源规划者中预算资源。 如果您对工作角色下列出的至少一个项目只有“查看”权限，则不能为“角色”视图中的角色分配预算。 您仍然可以为您具有管理权限的项目分配预算。

有关预算资源所需的访问权限的信息，请参阅文章[在Adobe Workfront中预算资源所需的访问权限](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。

要在&#x200B;**&#x200B;**&#x200B;角色视图的资源规划者中分配预算，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)。

1. 单击&#x200B;**资源**。
1. 默认显示&#x200B;**规划者**。
1. （视情况而定）选择&#x200B;**按角色查看**&#x200B;视图。
1. 展开工作角色和项目以管理项目、工作角色或用户的分配。
1. 要为用户分配预算，请执行下列操作之一：

   * 在&#x200B;**BDG**&#x200B;列中，手动指定用户的预算小时数、FTE或成本。
   * 单击项目的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**将用户的计划小时数设置为预算**。\
     使用以下公式计算每个用户的预算小时数：

     `User Budgeted Hours = User Planned Hours`

1. 要分配工作角色的预算，请执行以下操作之一：

   * 在&#x200B;**BDG**&#x200B;列中，手动指定工作角色的预算小时数、FTE或成本。\
     这会将角色预算小时数分配给您有权管理的项目的项目预算小时数。

   * 单击工作角色的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**将项目的计划小时数设置为已预算。**&#x200B;角色预算小时数使用以下公式计算：\
     &#x200B;*

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *项目预算小时数使用以下公式计算：

     `Project Budgeted Hours = Project Planned Hours`

   * 在&#x200B;**BDG**&#x200B;列中，为工作角色下列出的项目手动指定预算小时数、FTE或成本。\
     这会将项目预算小时数添加到角色。

   >[!NOTE]
   >
   >可以为主角色和其他（或辅助）角色为用户预算。 用户角色的FTE可用性&#x200B;**百分比**&#x200B;必须为与0%不同的数字，以便可用小时数在资源规划者中显示工作角色的值。 如果用户与具有0% **FTE可用性百分比**&#x200B;的角色关联，则该工作角色的可用小时值为零。 在这种情况下，角色可能会显示负的&#x200B;**净值**。\
   >有关工作角色的FTE可用性&#x200B;**百分比**&#x200B;的详细信息，请参阅文章[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

1. 要为项目分配预算，请执行以下操作之一：

   * 在&#x200B;**BDG**&#x200B;列中，手动指定项目的预算小时数、FTE或成本。\
     这也会更新列出项目的角色的预算小时数。

   * 单击工作角色的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**将项目的计划小时数设置为预算**。\
     项目预算小时数按以下公式计算：

     `Project Budgeted Hours = Project Planned Hours`

     项目预算小时数已添加到角色预算小时数。

   * （视情况而定）如果您已为用户预算小时数，请单击项目的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**项目的用户预算小时总数**。\
     项目预算小时数使用以下公式计算：

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. 单击&#x200B;**保存**。\
   在资源规划者中预算资源后，资源的预算小时数以及与资源相关的任何成本将列在每个项目的业务案例中。
有关了解业务案例的资源预算编制区域的详细信息，请参阅文章[业务案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

1. （可选）选择&#x200B;**按用户查看**&#x200B;视图可注意到每个用户的可用小时数和计划小时数之间存在的任何用户过度分配或利用不足的情况。 预算小时数在“按用户查看”视图中不可见。

### 批量预算资源 {#budget-resources-in-bulk}

使用快速链接时，您可以批量为资源分配预算。 快速链接仅可用于“项目”和“角色”视图。

![自动预算选项](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>使用资源预算分配的快速链接时，预算仅自动应用于屏幕上显示的时间段。 如果项目的时间表跨越的时间长于屏幕上显示的时间表，您必须从左向右滚动，然后使用快速链接自动为资源编列预算。

要批量预算您的资源，请执行以下操作：

1. 转到。\
   有关访问资源规划者的详细信息，请参阅文章[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的“访问资源规划者”部分。\
   列表中会显示您可以管理的项目列表。

1. （可选）展开每个项目可查看与其关联的工作角色列表。\
   或
1. （可选）选择&#x200B;**按角色查看**，然后展开每个角色以查看与其关联的项目列表。
1. 将鼠标悬停在项目或工作角色的名称上。
1. 单击项目或角色名称最右侧显示的&#x200B;**更多**&#x200B;图标![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)。

1. 单击其中一个可用选项可自动指定其他对象的预算小时数(BDG)。

   根据您是在项目还是角色上单击了更多图标，批量预算编制的选项会有所不同。 下表说明了可用于项目和角色的选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>项目视图</strong> </td> 
      <td><strong>角色视图</strong> </td> 
     </tr> 
     <tr> 
      <td>项目选项</td> 
      <td> 
       <ul> 
        <li><strong>将角色的计划小时数设置为预算</strong>：选择此选项可使角色的预算小时数与其计划小时数相同。 将为项目预算小时数显示角色的预算小时总数。 </li> 
        <li><strong>调整预算日期</strong> ：选择此选项以将预算小时数移动到不同的时间范围。<br>有关调整预算日期的详细信息，请参阅<a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">在资源规划者中调整预算日期</a>。</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>将用户的计划小时数设置为预算</strong>：选择此选项可使用户的预算小时数与其计划小时数相同。 </li> 
        <li><strong>项目的用户预算小时数总计</strong>：选择此选项可将所有用户预算小时数相加，并将总计显示为项目和角色的预算小时数。 我们建议您在手动为用户预算或首先使用上一个选项之后使用此选项。 </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>角色选项</td> 
      <td> 
       <ul> 
        <li><strong>将用户的计划小时数设置为预算</strong>：选择此选项可使用户的预算小时数与其计划小时数相同。 </li> 
        <li><strong>角色的用户预算小时数总计</strong>：选择此选项可将用户的所有预算小时数相加，并将总计显示为角色和项目的预算小时数。 我们建议您在手动为用户预算或首先使用上一个选项之后使用此选项。 </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>将项目的计划小时数设置为预算</strong>：选择此选项可使项目预算小时数变得与项目计划小时数相同。 </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果缺少在资源规划者中工作的一些先决条件，则某些选项可能未显示。
   >
   >
   >有关在资源规划者中实现准确预算必须满足的先决条件的更多信息，请参阅[资源规划者概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)文章中的“在资源规划者中工作的先决条件”部分。\
   >例如，以下场景中可能未显示某些选项：
   >
   >   
   >   
   >   * 当项目未与资源池关联时
   >   * 当与项目关联的资源池不包含用户时
   >   * 当与项目关联的资源池包含的用户没有与其关联的工作角色时。
   >   
   >
