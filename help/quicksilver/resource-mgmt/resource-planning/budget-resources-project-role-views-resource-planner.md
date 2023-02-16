---
product-area: resource-management
navigation-topic: resource-planning
title: 使用“项目”和“职责”视图在资源计划员中预算资源
description: 您可以使用“项目”和“职责”视图对Adobe Workfront资源计划员中的资源进行预算。 您不能使用“资源计划员”中的“用户”视图来预算资源预算。
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# 使用“项目”和“职责”视图在资源计划员中预算资源

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

资源计划员的主要功能是对资源进行预算，以用于必须在项目中完成的工作。

>[!IMPORTANT]
>
>您只能在应用 **按项目查看** 或 **按角色查看** 查看资源计划员。

在资源计划器中开始预算信息之前，请参阅以下文章：

* [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [在Adobe Workfront获得预算资源所需的资源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [资源计划员的“项目”和“职责”视图中的工时、FTE和成本信息概览](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，包括对资源计划员中“编辑优先级”和“预算小时数”的访问权限</p> <p>按成本编辑对预算资源的财务数据访问权限</p> <p>编辑对项目和用户的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要预算的项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 资源计划员中的预算资源

* [项目视图中的预算资源](#budget-resources-in-the-project-view)
* [“职责”视图中的预算资源](#budget-resources-in-the-role-view)
* [批量预算资源](#budget-resources-in-bulk)

### 项目视图中的预算资源 {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **资源化**.
1. 的 **计划员** 默认显示。
1. （视情况而定）选择 **按项目查看** 中。
1. 展开项目和作业角色以管理项目、作业角色或用户的分配。
1. 要为用户分配预算，请执行以下操作之一：

   * 在 **BDG** 列中，为用户手动指定预算小时数、FTE或成本。

   * 单击 **更多** 菜单，然后单击 **将用户的计划小时数设置为预算**.\
      每个用户的预算小时数使用以下公式计算：

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. 要为职务角色分配预算，请执行以下操作之一：

   * 在 **BDG** 列中，为职务角色手动指定预算小时数、FTE或成本。

      >[!NOTE]
      >
      >“已编入预算的工时”角色将添加到“项目已编入预算的工时”中。

   * （视情况而定）如果您已为用户编入了小时数预算，请单击 **更多** 菜单，然后单击 **角色的用户预算总时数**.\
      每个角色的预算小时数使用以下公式计算：

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * 单击 **更多** 菜单，然后单击 **将角色的计划小时数设置为预算值**.\
      每个角色的预算小时数使用以下公式计算：\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* “已编入预算的工时”角色将添加到“项目已编入预算的工时”中。
      >* 可以为“主角色”和“其他（或辅助）角色”预算用户。
      >* 的 **FTE可用性百分比** 对于用户的角色，“可用小时数”的值必须不同于0%，才能在“资源计划员”中显示任务角色的值。 如果用户与具有0% **FTE可用性百分比**，则该作业角色的“可用小时数”值为0。 在这种情况下，角色可能显示为负面 **净值**.\
         >有关 **FTE可用性百分比** 有关作业角色，请参阅文章 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * 在 **BDG** 列中，手动指定项目的预算小时数、FTE或成本。 这会将项目预算小时数分配给项目下的每个角色。 存在以下情形：

      * 如果您指定的项目预算小时数等于项目计划小时数，则角色预算小时数与角色计划小时数匹配。
      * 如果您指定的项目预算小时数不等于项目计划小时数，则根据每个职责所需的计划小时数百分比分配职责预算小时数。\
         例如，如果一个项目有20个计划时间，并且这些时间分配在两个工作角色（顾问需要12个计划时间，工程师需要8个计划时间）之间，而您为该项目预算了30个小时，则这些时间分配如下：顾问角色获得18个预算小时数，而工程师角色获得12个预算小时数。

1. 要为项目分配预算，请执行以下操作之一：

   * 按照步骤7中所述，对项目下的角色进行预算。\
      项目预算小时数按以下公式计算：

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * 在 **BDG** 列中，手动指定项目的预算小时数、FTE或成本。\
      这将更新角色预算小时数，如步骤7中所述。\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. 单击&#x200B;**保存**。\
   在资源计划员中预算资源后，资源的预算小时数以及与这些资源关联的任何成本都会列在每个项目的业务案例中。\
   有关了解“业务案例”的“资源预算”区域的详细信息，请参阅文章中的“资源预算”部分 [业务案例领域概述](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. （可选）选择“用户”视图，以注意每个用户在“可用”和“计划小时数”之间的任何用户过度分配或利用率过低。 预算小时数在“用户”视图中不可见。

   有关Workfront如何计算用户可用性的信息，请参阅 [配置资源管理首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### “职责”视图中的预算资源 {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

您必须拥有对项目的“资源管理和财务数据”和“管理财务”权限的编辑访问权限，才能在资源计划器中对资源进行预算。 如果您只对职务角色下列出的至少一个项目具有“查看”权限，则无法在“职责”视图中为该职责分配预算。 您仍可以为具有“管理”权限的项目分配预算。

有关预算资源所需访问权限的信息，请参阅文章 [在Adobe Workfront获得预算资源所需的资源](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

要在“职责”视图的“资源计划员”中分配预算，****请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **资源化**.
1. 的 **计划员** 默认显示。
1. （视情况而定）选择 **按角色查看** 中。
1. 展开作业角色和项目以管理项目、作业角色或用户的分配。
1. 要为用户分配预算，请执行以下操作之一：

   * 在 **BDG** 列中，为用户手动指定预算小时数、FTE或成本。
   * 单击 **更多** 菜单，然后单击 **将用户的计划小时数设置为预算**.\
      每个用户的预算小时数使用以下公式计算：

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. 要为职务角色分配预算，请执行以下操作之一：

   * 在 **BDG** 列中，手动指定职务角色的预算小时数、FTE或成本。\
      这会将角色预算小时数分配给您有权管理的项目的预算小时数。

   * 单击 **更多** 菜单，然后单击**将项目的计划小时数设置为预算。**使用以下公式计算“职责预算小时数”：\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *项目预算小时数使用以下公式计算：

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * 在 **BDG** 列中，为在职务角色下列出的项目手动指定预算小时数、FTE或成本。\
      这会将项目预算小时数添加到角色。
   >[!NOTE]
   >
   >可以为“主角色”和“其他（或辅助）角色”预算用户。 的 **FTE可用性百分比** 对于用户的角色，“可用小时数”的值必须不同于0%，才能在“资源计划员”中显示任务角色的值。 如果用户与具有0% **FTE可用性百分比**，则该作业角色的“可用小时数”值为0。 在这种情况下，角色可能显示为负面 **净值**.\
   >有关 **FTE可用性百分比** 有关作业角色，请参阅文章 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. 要为项目分配预算，请执行以下操作之一：

   * 在 **BDG** 列中，手动指定项目的预算小时数、FTE或成本。\
      此外，还会更新项目所在角色的预算小时数。

   * 单击 **更多** 菜单，然后单击 **将项目的计划小时数设置为预算**.\
      项目预算小时数按以下公式计算：

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      项目预算小时数将添加到角色预算小时数中。

   * （视情况而定）如果您已为用户预算了小时数，请单击 **更多** 菜单，然后单击 **项目的用户预算总时数**.\
      项目预算小时数使用以下公式计算：

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. 单击&#x200B;**保存**。\
   在资源计划员中预算资源后，资源的预算小时数以及与这些资源关联的任何成本都会列在每个项目的业务案例中。\
   有关了解“业务案例”的“资源预算”区域的详细信息，请参阅文章 [业务案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. （可选）选择 **按用户查看** 查看，以注意每个用户的“可用”和“计划小时数”之间的任何用户过度分配或利用率不足。 “按用户查看”视图中不显示预算小时数。

### 批量预算资源 {#budget-resources-in-bulk}

使用快速链接时，您可以批量预算资源分配。 快速链接仅可用于项目视图和角色视图。

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>使用资源预算分配的快速链接时，预算会自动仅应用于屏幕上显示的时间段。 如果项目的时间轴跨度超过屏幕上显示的时间轴，则必须从左到右滚动，然后使用快速链接自动对资源进行预算。

要批量预算资源，请执行以下操作：

1. 转到。\
   有关访问资源计划员的详细信息，请参阅文章中的“访问资源计划员”部分 [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   列表中会显示您可以管理的项目列表。

1. （可选）展开每个项目以查看与其关联的作业角色列表。\
   或
1. （可选）选择 **按角色查看**，然后展开每个角色以查看与其关联的项目列表。
1. 将鼠标悬停在项目或作业角色的名称上。
1. 单击 **更多** 图标 ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)显示在项目或角色名称的最右侧。

1. 单击其中一个可用选项，可自动为其他对象指定预算小时数(BDG)。

   根据您是单击项目还是角色上的更多图标，批量预算选项会有所不同。 下表说明了可用于项目和角色的选项：

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
        <li><strong>将角色的计划小时数设置为预算值</strong>:选择此选项可使角色的预算小时数与其计划小时数相同。 角色的预算小时数总计将显示项目预算小时数。 </li> 
        <li><strong>调整预算日期</strong> :选择此选项可将预算小时数移到其他时间范围。<br>有关调整预算日期的详细信息，请参阅 <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">在资源计划器中调整预算日期</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>将用户的计划小时数设置为预算</strong>:选择此选项可使用户的预算小时数与其计划小时数相同。 </li> 
        <li><strong>项目的用户预算总时数</strong>:选择此选项可将所有用户的预算小时数一起添加，并将总计显示为项目和角色的预算小时数。 我们建议您在手动预算用户或先使用前一个选项后使用此选项。 </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>角色选项</td> 
      <td> 
       <ul> 
        <li><strong>将用户的计划小时数设置为预算</strong>:选择此选项可使用户的预算小时数与其计划小时数相同。 </li> 
        <li><strong>角色的用户预算总时数</strong>:选择此选项可将用户的所有预算小时数一起添加，并将合计显示为角色和项目的预算小时数。 我们建议您在手动预算用户或先使用前一个选项后使用此选项。 </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>将项目的计划小时数设置为预算</strong>:选择此选项可使项目预算小时数与项目计划小时数相同。 </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果缺少在资源计划器中工作的某些先决条件，则可能无法显示某些选项。
   >
   >
   >有关在资源计划器中准确编制预算必须满足的先决条件的详细信息，请参阅 [资源计划员概述](../../resource-mgmt/resource-planning/get-started-resource-planner.md) 文章。\
   >例如，某些选项可能不会在以下情况下显示：
   >
   >   
   >   
   >   * 项目未与资源池关联时
   >   * 与项目关联的资源池不包含用户时
   >   * 当与项目关联的资源池包含没有与项目关联作业角色的用户时。

