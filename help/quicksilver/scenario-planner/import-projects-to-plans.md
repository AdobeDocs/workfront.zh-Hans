---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案计划器中将项目导入计划
description: 您可以将现有项目导入计划。 导入的项目将转换为方案，您可以在计划中管理它们，就像您管理新方案一样。 原始项目仍与新倡议挂钩。
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# 将项目导入 [!DNL Scenario Planner]

您可以将现有项目导入计划。 导入的项目将转换为方案，您可以在计划中管理它们，就像您管理新方案一样。 原始项目仍与新倡议挂钩。

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
   <td> <p>[!DNL Adobe Workfront]<b> 计划*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 许可证*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对方案计划员中计划的访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 关于将项目作为新计划导入计划的考虑

* 必须先创建项目，然后才能将项目作为新方案导入计划。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* 你至少 [!UICONTROL 查看] 权限，以便能够将项目导入计划作为新计划。
* 您可以将同一项目导入多个计划。
* 要导入的项目必须在计划的时间范围内包含日期。 您无法导入具有 [!UICONTROL 计划完成日期] 早于计划开始或 [!UICONTROL 计划开始日期] 比计划结束还晚。
* 一次不能导入100个以上的项目。
* 有些项目信息也被导入计划中，成为主动信息。 有关将哪些项目信息导入计划并成为主动信息的信息，请参阅 [将项目信息导入计划](#project-information-imported-into-the-plan) 章节。
* 在链接项目上发生的更改不会影响计划上的各项倡议。
* 对计划中的方案所做的更改不会自动影响链接的项目方案更改仅在从计划中发布方案时影响链接的项目。 有关发布活动如何影响链接项目的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* 删除通过导入项目创建的方案不会删除该项目。
* 删除链接到方案的项目不会删除方案。

## 将项目信息导入计划 {#project-information-imported-into-the-plan}

在将项目导入计划时，某些项目信息也会导入计划中，并成为主动信息。 下表显示了在将项目导入计划时，哪些项目信息会成为方案信息：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>项目信息</td> 
   <td>主动信息 </td> 
  </tr> 
  <tr> 
   <td>项目名称</td> 
   <td>方案名称</td> 
  </tr> 
  <tr> 
   <td>项目计划日期</td> 
   <td> <p>计划开始和结束月份。</p> <p>如果项目在一个月中旬开始或结束，则导入日期会延长到计划中的整个月。 例如，如果项目计划日期为2020年3月20日至5月5日，则导入方案的日期为2020年3月至5月。</p> <p>如果计划起始日期或完成日期超出计划持续时间，则会显示一个可视指示，表示导入的方案在计划之前或之后开始或结束。 </p> </td> 
  </tr> 
  <tr> 
   <td>分配给任务和问题的作业角色</td> 
   <td> <p>计划工作角色. </p> <p>注释:   <p>如果用户在项目生命周期中更改了角色，则导入的角色取决于您在导入项目时分配的状态。 存在以下情形：</p> 
     <ul> 
      <li> <p>如果分配给任务的用户或问题在将其分配标记为[!UICONTROL Done]后更改了其角色， [!DNL Workfront] 将用户在将分配标记为[!UICONTROL Done]之前履行的角色导入方案。</p> </li> 
      <li> <p>如果分配给任务或问题的用户在项目生命周期中更改了角色，但在导入项目时，他们在任务或问题上的分配未标记为[!UICONTROL Done], [!DNL Workfront] 仅导入分配用户的当前角色。 </p> </li> 
     </ul> <p>有关分配状态的信息，请参阅 <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe [!DNL Workfront] 术语</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>与分配给任务或问题的作业角色关联的项目[!UICONTROL计划时数]</td> 
   <td> <p><span>根据计划是设置为使用FTE还是小时，项目任务中的[!UICONTROL计划小时数]将变为</span> [!UICONTROL必需FTE] <span>或计划中的[!UICONTROL必需时数]</span>. </p> <p>有关设置计划以使用FTE或小时的信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> <p>请考虑以下事项：</p> 
    <ul> 
     <li> <p>[!DNL Workfront] 使用分配给任务和问题的作业角色，或分配给任务或问题的用户在项目中与之关联的作业角色，并将它们作为“必需的作业角色”转移到新方案。 </p> </li> 
     <li> <p>当计划设置为使用FTE时，与项目任务和问题中的作业角色关联的计划小时数将首先转换为FTE。 然后，将此FTE分配给方案的工作角色。 <span>计划时数在 [!DNL Workfront]. 如果任务或问题跨越多个月，则计划期间内每月的计划小时数将以每月FTE转换并转移到计划的每个月。</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span><span>例如，如果在9月份将任务分配给80个计划小时的职务职责，则导入的职务职责在9月份将为方案显示0.5个FTE。</span> </p> </li> 
     <li> <p>[!DNL Workfront] 使用以下公式计算与方案关联的必需作业角色的FTE:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>提示：的 [!DNL Scenario Planner] 假定一个月有160个工作小时。</p> <p>例如，如果项目的持续时间为1200分钟，并且项目上的工作角色与600分钟计划小时关联，则其FTE为0.5。在导入项目时，新创建方案上的必需工作角色FTE对于方案的每个月为0.5。 </p> </li> 
     <li>如果将职务角色分配给项目上计划时数为零的任务，则方案职务角色的必需FTE默认为零。 <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>将作业角色分配给项目上的任务（持续时间为零[!UICONTROL）时，为必需的FTE <span>或小时</span> 对于方案的任务角色，默认为零，即使任务具有“计划时数”。 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## 将项目导入计划

>[!IMPORTANT]
>
>在将项目导入计划后，这些项目就成为计划的倡议。 尽管这两个项目是链接的，但它们作为独立实体存在，并且在更新它们时不会自动相互影响。
>
>发生以下情况：
>
>* 在将项目导入计划后，对项目所做的更改永远不会影响方案。这些更改包括对职务职责分配所做的更改。
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* 对计划所做的更改会影响 [!DNL Scenario Planner] 区域。 否则，它们不会影响 [!UICONTROL 计划小时数] 项目任务和问题的信息。
>
>  有关发布活动如何影响链接项目的信息，请参阅  [通过在方案规划器中发布方案来更新或创建项目](../scenario-planner/publish-scenarios-update-projects.md).

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) 的右上角 [!DNL Workfront]，然后单击 [!DNL Scenarios] 访问 [!DNL Scenario Planner].

1. 单击要导入项目的计划名称。
1. 单击 **[!UICONTROL 新计划]**，然后单击 **[!UICONTROL 导入项目]**.

   的 [!UICONTROL 导入项目] 框中。 计划时间范围内包含日期的项目会显示在列表中。

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >处于任何状态的项目都会显示在列表中。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. （可选）单击 **[!UICONTROL “过滤器”图标]** ![](assets/filter-nwepng.png)并从列表中选择一个可用的过滤器，以减少列表上的项目数量。 默认情况下，项目列表会按照用户当前选定的项目筛选器在项目列表中进行筛选。

1. （可选）单击 **[!UICONTROL “搜索”图标]** ![](assets/search-icon.png) 并添加屏幕上任何字段上显示的关键词。 包含搜索词的项目会自动显示在列表中，并且所有项目都会隐藏。

1. （视情况而定）单击 **[!UICONTROL X图标]** 删除搜索并显示所有项目。
1. 选择最多100个项目并单击 **[!UICONTROL 导入]**.

   这些项目作为新举措引进。

   请注意以下事项：

   * 项目图标 ![](assets/project-icon-sp.png) 显示在方案名称的右侧。
   * 如果项目时间轴超过计划的持续时间，则方案栏以左侧（当开始日期早于计划日期时）或右侧（当结束日期晚于计划日期时）的指向边距结束。

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * 已更新月数和作业角色，以匹配项目的角色。
   >[!TIP]
   >
   >与职务角色关联的成本在方案层更新，不会从项目中导入。

1. 单击表示新方案的栏以打开右侧的方案详细信息面板。

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   在 **[!UICONTROL 计划持续时间]** 区域查看以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL计划持续时间]</td> 
      <td>这是倡议的持续时间（以月为单位）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>计划的开始和结束日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL项目]</td> 
      <td> <p>链接项目的[!UICONTROL计划开始日期]和[!UICONTROL完成日期]。</p> <p>提示：如果[!UICONTROL项目]信息缺失，则项目会被删除。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 编辑方案的名称。 默认情况下，它与项目名称匹配。
1. （可选）执行以下操作之一：

   * 在 **[!UICONTROL 所需的作业角色]** 部分
   * 更新 **[!UICONTROL 固定成本]** 在 **[!UICONTROL 成本]** 部分

   * 单击 **[!UICONTROL 更新可用的作业角色]** 或 **[!UICONTROL 更新可用预算]** 解决新倡议与计划其他倡议之间的冲突。

1. （视情况而定）单击 **[!UICONTROL 应用]** 以保存对您的计划所做的更改。
1. 单击 **[!UICONTROL 保存计划]** 以保存对计划所做的更改。
1. （可选）要将您对方案所做的更改更新回其从中导入的项目，请从计划中发布该项目。 有关发布计划的信息，请参阅 [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. （可选）单击项目图标以访问链接的项目。

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
