---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 将项目导入方案规划器中的计划
description: 您可以将现有项目导入计划。 导入的项目将转换为计划，您可以在计划中管理它们，就像管理新计划一样。 原始项目仍与新计划关联。
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1710'
ht-degree: 0%

---

# 将项目导入[!DNL Scenario Planner]中的计划

您可以将现有项目导入计划。 导入的项目将转换为计划，您可以在计划中管理它们，就像管理新计划一样。 原始项目仍与新计划关联。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>计划*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b>许可证*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关获取[!DNL Workfront Scenario Planner]的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[！UICONTROL Edit]或更高版本对 [!DNL Scenario Planner]</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何更改访问级别的信息，请参阅<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[！UICONTROL Manage]对计划的权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在方案规划者中请求对计划的访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 将项目作为新计划导入计划中的注意事项

* 必须先创建项目，然后才能将项目作为新计划导入计划。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* 您必须对项目具有至少[!UICONTROL 查看]权限，才能将这些项目作为新计划导入计划。
* 您可以将同一项目导入多个计划中。
* 要导入的项目必须包含计划时间框架中的日期。 您无法导入[!UICONTROL 计划完成日期]早于计划开始日期或[!UICONTROL 计划开始日期]晚于计划结束日期的项目。
* 您无法一次导入100个以上的项目。
* 某些项目信息也会导入到计划中，并成为计划信息。 有关哪些项目信息已导入计划并成为计划信息的信息，请参阅本文中的[项目信息已导入计划](#project-information-imported-into-the-plan)部分。
* 链接项目上发生的更改不会影响计划上的计划。
* 对计划上的计划所做的更改不会自动影响链接的项目计划更改仅在您从计划发布计划时影响链接的项目。 有关发布计划如何影响链接项目的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。
* 删除通过导入项目创建的计划不会删除项目。
* 删除链接到计划的项目不会删除计划。

## 导入到计划中的项目信息 {#project-information-imported-into-the-plan}

将项目导入到计划时，某些项目信息也会导入到计划中，并成为计划信息。 下表显示了将项目导入计划时，哪些项目信息将成为计划信息：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>项目信息</td> 
   <td>计划信息 </td> 
  </tr> 
  <tr> 
   <td>项目名称</td> 
   <td>计划名称</td> 
  </tr> 
  <tr> 
   <td>项目计划日期</td> 
   <td> <p>计划开始和结束月份。</p> <p>如果项目在月中开始或结束，则导入日期会延长到计划中的一整月。 例如，如果项目计划日期为2020年3月20日至5月5日，则导入计划的日期为2020年3月至5月。</p> <p>如果计划的开始日期或完成日期超过计划的持续时间，则会出现导入的方案在计划之前或之后开始的可视指示。 </p> </td> 
  </tr> 
  <tr> 
   <td>分配给任务和问题的工作角色</td> 
   <td> <p>计划工作角色。 </p> <p>注意：   <p>如果用户在项目生命周期内更改角色，则导入的角色取决于导入项目时的分配状态。 存在以下情况：</p> 
     <ul> 
      <li> <p>如果分配给任务或问题的用户在将其分配标记为[！UICONTROL完成]之后更改了角色，则[!DNL Workfront]会将用户在将分配标记为[！UICONTROL完成]之前履行的角色导入计划。</p> </li> 
      <li> <p>如果分配给任务或问题的用户在项目生命周期内更改了角色，但在导入项目时，他们在任务或问题上的分配未标记为[！UICONTROL完成]，则[!DNL Workfront]将仅导入分配用户的当前角色。 </p> </li> 
     </ul> <p>有关任务状态的信息，请参阅Adobe[!DNL Workfront]术语的<a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">词汇表</a>中的“任务状态”。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>与分配给任务或问题的工作角色关联的项目[！UICONTROL计划小时数]</td> 
   <td> <p><span>根据计划是设置为使用FTE还是使用小时数，项目任务中的[！UICONTROL计划小时数]在计划</span>上变为</span> [！UICONTROL必需FTE数] <span>或[！UICONTROL必需要小时数]。 </p> <p>有关设置计划以使用FTE或小时数的信息，请参阅<a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中创建和编辑计划。 </p> <p>请考虑以下事项：</p> 
    <ul> 
     <li> <p>[!DNL Workfront] 使用分配给任务和问题的工作角色或分配给任务或问题的用户与项目相关联的工作角色，并将它们作为所需工作角色转移到新计划中。 </p> </li> 
     <li> <p>当计划设置为使用FTE时，与项目任务和问题中的工作角色关联的已计划小时数首先转换为FTE。 然后，此FTE将分配给计划的工作角色。 <span>计划小时数在[!DNL Workfront]中平均分配。 如果任务或问题跨越多个月，则计划持续时间中每个月的计划小时数将在每月FTE中转换为并转移到计划的每个月。</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><span>例如，如果一项任务在9月份被分配给工作角色80个计划小时数，那么在9月份，导入的工作角色为计划显示0.5 FTE。</span> </p> </li> 
     <li> <p>[!DNL Workfront] 使用以下公式计算与方案关联的所需工作角色的FTE：</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>提示： [!DNL Scenario Planner]假设一个月有160个工作小时。</p> <p>例如，如果某个项目的持续时间为1200分钟，并且该项目上的一个工作角色与计划小时数的600分钟关联，则其FTE为0.5。在导入项目时，新创建的计划上的所需工作角色FTE为每月计划0.5。 </p> </li> 
     <li>当工作角色分配给项目上的任务且计划小时数为零时，计划工作角色的所需FTE在默认情况下为零。 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>当工作角色被分配给具有零[！UICONTROL持续时间]的项目中的任务时，计划的工作角色所需的FTE <span>或小时数</span>默认为零，即使任务具有计划的小时数。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## 将项目导入计划

>[!IMPORTANT]
>
>将项目导入计划后，它们就会成为计划中的计划。 尽管这两个项目是链接的，但它们作为独立图元存在，并且更新它们时不会自动相互影响。
>
>出现以下情况：
>
>* 在将项目导入计划后，对项目所做的更改不会影响计划。这些更改包括对工作角色分配的更改。
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* 只有在您将计划发布到相应项目时，对计划所做的更改才会影响项目上[!DNL Scenario Planner]区域中的信息。 否则，它们不会影响项目任务和问题的[!UICONTROL 计划小时数]信息。
>
>  有关发布计划如何影响链接项目的信息，请参阅[通过在Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。
>

1. 单击[!DNL Workfront]右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击[!DNL Scenarios]以访问[!DNL Scenario Planner]。

1. 单击要导入项目的计划的名称。
1. 单击&#x200B;**[!UICONTROL 新建计划]**，然后单击&#x200B;**[!UICONTROL 导入项目]**。

   此时会显示[!UICONTROL 导入项目]框。 日期包含在计划时间框架中的项目会显示在列表中。

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >处于任何状态的项目都会显示在列表中。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. （可选）单击&#x200B;**[!UICONTROL 筛选器图标]** ![](assets/filter-nwepng.png)并从列表中选择一个可用的筛选器以减少列表上的项目数。 默认情况下，项目列表按用户当前在项目列表中选定的项目过滤器进行过滤。

1. （可选）单击&#x200B;**[!UICONTROL 搜索图标]** ![](assets/search-icon.png)并添加屏幕上任何字段显示的关键字。 包含搜索词的项目会自动显示在列表中，并且所有项目都处于隐藏状态。

1. （视情况而定）单击&#x200B;**[!UICONTROL X图标]**&#x200B;可删除搜索并显示所有项目。
1. 选择最多100个项目并单击&#x200B;**[!UICONTROL 导入]**。

   项目将作为新计划导入。

   请注意以下事项：

   * 项目图标![](assets/project-icon-sp.png)显示在计划名称的右侧。
   * 如果项目时间线超出计划的持续时间，则计划栏将以左侧（当开始日期早于计划日期时）或右侧（当结束日期晚于计划日期时）的尖角边距结束。

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 月数和工作角色已更新以匹配项目的月数和工作角色。

   >[!TIP]
   >
   >与工作角色关联的成本在计划级别更新，且不会从项目导入。

1. 单击表示新计划的栏以打开右侧的计划详细信息面板。

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   在&#x200B;**[!UICONTROL 计划持续时间]**&#x200B;区域查看以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划持续时间]</td> 
      <td>这是计划的持续时间（以月为单位）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划]</td> 
      <td>计划的开始日期和结束日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL项目]</td> 
      <td> <p>链接项目的[！UICONTROL计划开始日期]和[！UICONTROL完成日期]。</p> <p>提示：如果[！UICONTROL项目]信息缺失，则该项目已被删除。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 编辑计划的名称。 默认情况下，它与项目的名称匹配。
1. （可选）执行以下操作之一：

   * 更新&#x200B;**[!UICONTROL 所需工作角色]**&#x200B;部分中的工作角色
   * 更新&#x200B;**[!UICONTROL 成本]**&#x200B;部分中的&#x200B;**[!UICONTROL 固定成本]**

   * 单击&#x200B;**[!UICONTROL 更新可用工作角色]**&#x200B;或&#x200B;**[!UICONTROL 更新可用预算]**&#x200B;以解决新计划与计划上的其他计划之间的冲突。

1. （视情况而定）单击&#x200B;**[!UICONTROL 应用]**&#x200B;以将更改保存到您的计划。
1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存对计划的更改。
1. （可选）要将您对计划所做的更改更新回从中导入计划的项目，请从计划发布该项目。 有关发布计划的信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。
1. （可选）单击项目图标以访问链接的项目。

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
