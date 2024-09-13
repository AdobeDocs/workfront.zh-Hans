---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在场景规划程序中解决方案冲突
description: 当计划相互冲突时，它们会争夺相同的资源。 您可用于方案的资源不足以涵盖方案中所有计划所需的所有资源。
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '2172'
ht-degree: 0%

---

# 解决[!DNL Scenario Planner]中的计划冲突

当计划相互冲突时，它们会争夺相同的资源。 您可用于方案的资源不足以涵盖方案中所有计划所需的所有资源。

这可以在以下任何情况下发生：

* 计划所需的工作角色数量大于为计划预算的角色数量。
* 该计划的费用大于计划可用的预算金额。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td> <ul></li>
   <li><p>新增：Ultimate </p></li>
   <p>场景规划程序不可用于新的Workfront Select或Workfront Prime计划。 </p>
   <li><p>当前： [！UICONTROL Business]或更高版本</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td> <p>新增：浅色或更高</p> 
   <p>当前： [！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品* </td> 
   <td> <ul><li><p>对于新的Workfront计划：</p><p> Adobe Workfront</li></p>
   <li><p>对于当前Workfront计划： </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>有关详细信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别 </td> 
   <td> <p>[！UICONTROL Edit]访问 [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[！UICONTROL Manage]对计划的权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">在[!DNL Scenario Planner]</a>中请求对计划的访问权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅[Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决冲突概述

* 冲突还被理解为工作角色或方案预算的过度分配。
* 当[!DNL Workfront]检测到冲突时，计划持续时间中与冲突月份对应的栏以红色显示。 这可以在以下任何情况下发生：

   * 在所有以前的计划都使用了为计划预算的资源后，计划每月所需的工作角色数量大于为计划预算的角色数量。
   * 在所有以前的倡议都使用计划的预算来支付其费用之后，该倡议的每月费用比计划的可用预算要多。

>[!TIP]
>
>默认情况下，[!DNL Scenario Planner]假定您为0个工作角色预算了$0或等效于系统货币的$0方案，除非您另外指定。 工作角色的数量表示为该工作角色预算的FTE（全职等效人数）或小时数。
>
>对于Scenario Planner中的所有计算，Workfront使用以下值： 1 FTE = 8小时。
>
>有关更新计划和预算的可用角色的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

* 您可以通过执行以下操作之一来解决冲突：

   * 自动从方案上的计划添加缺少的所需资源。 本文介绍如何使用此选项解决冲突。
   * 通过编辑计划，调整方案的工作角色和预算资源。 有关详细信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

## 解决计划之间的冲突

1. 转到要解决冲突的计划。

   有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

   有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

1. （可选）从&#x200B;**[!DNL Initial scenario]**&#x200B;下拉菜单中，选择要查看的方案。

   >[!TIP]
   >
   >一个计划可能具有多种方案。 查看计划的冲突时，[!DNL Workfront]是指选定方案上当前可用的资源以及该方案的计划上所需的资源。 有关方案的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md)中创建和比较计划方案。

1. 确保已启用&#x200B;**[!UICONTROL 显示冲突]**。 默认情况下处于启用状态。

   ![](assets/show-scenarios-toggle-on.png)

   第一个冲突方案以红色显示存在冲突的月份，方案名称旁边会显示一个警告图标。

   从第一个冲突计划开始的所有计划的背景以红色显示在计划图表上。

   当计划显示冲突时，这意味着至少一个特定角色的工作角色数量和/或发生的成本超过为特定月份的计划定义的工作角色数量或预算。

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. 执行以下操作之一，了解有关可能存在的冲突的更多信息：

   * 将鼠标悬停在计划名称旁边的警告图标上，以了解您是拥有工作角色还是预算冲突。

     ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     根据您是过度分配了工作角色还是高估了计划的成本，当鼠标悬停在警告图标上时，您可能会看到以下选项之一：

      * 显示工作角色冲突详细信息
      * 显示预算冲突详细信息
      * 显示工作角色和预算详细信息

   * 在按月查看计划时，将鼠标悬停在计划时间线中的某个月上可查看该月所需的资源以及该月的冲突是与人员还是与成本相关。

     ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     在计划层查看以下每月信息：

      * 当月计划的所有计划的可用、必需和过度分配工作角色的数量
      * 当月所有计划计划的可用成本、所需成本和过度分配成本

        >[!TIP]
        >
        >[!UICONTROL 可用]成本是该月方案的预算。

   * 将鼠标悬停在计划的红色栏上一个月会显示有关当月发生的冲突的其他信息框。

     ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     在方案级别的附加信息框中查看以下字段：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">发生冲突的月份</td> 
        <td>显示在附加信息框的标题中。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">计划名称</td> 
        <td>显示在附加信息框的标题中。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[！UICONTROL Job Roles]</td> 
        <td> <p>与所选月份过度分配的此计划关联的工作角色。 以下列显示所选月份所需的每个工作角色的信息，这些信息与该月份可用的工作角色数量冲突：</p> 
         <ul> 
          <li> <p><strong>[！UICONTROL可用]</strong>：在选定月份中，方案中的每个可用工作角色的数量。</p> </li> 
          <li> <p><strong>[！UICONTROL必需]</strong>：计划在选定月份所需的每个工作角色的数量。</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[！UICONTROL过度分配]：</strong>计划所需的数量与方案中的可用数量之间的差值。 </p> </li> 
         </ul> <p>提示：有时，[！UICONTROL Available]角色的数量与[！UICONTROL Required]角色的数量匹配或更高，但[!DNL Scenario Planner]仍显示过度分配。 这意味着存在更高级别的计划，这些计划已使用同一月计划中可用的工作角色。 </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">成本</td> 
        <td> <p>所选月份的计划成本。 以下列显示所选月份所需成本和可用预算的信息：</p> 
         <ul> 
          <li> <p><strong>[！UICONTROL可用]</strong>：计划中所选月份的可用预算。</p> </li> 
          <li> <p><strong>[！UICONTROL必需]</strong>：选定月份与此计划相关的成本。</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[！UICONTROL过度分配]：</strong>计划成本与计划可用预算之间的差额。 </p> </li> 
         </ul> <p>提示：有时，[！UICONTROL可用]成本与所选月份的计划[！UICONTROL必需]成本匹配或更高，并且[!DNL Scenario Planner]仍显示成本过度分配。 这意味着已有更高层的计划使用了同一月的可用预算。 </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. 执行以下操作之一，打开计划详细信息面板，查看有关冲突发生位置和解决冲突的更多信息：

   * 单击计划名称旁边的警告图标。
   * 单击方案栏。
   * 单击计划名称右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;图标![](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 编辑]**。

     计划详细信息面板将显示在右侧。

     当您的计划没有足够的可用人员或预算时，以下部分旁边会显示一个红色警告图标：

   * [!UICONTROL 必需的工作角色]
   * [!UICONTROL 成本]

1. （视情况而定）对于存在工作角色冲突的计划，请转至&#x200B;**[!UICONTROL 所需的工作角色]**&#x200B;部分以查看计划所需的所有工作角色。 确定可能过度分配的工作角色。 查看计划每个月每个工作角色所需的FTE数或小时数。 对于具有过度分配的月份，包含FTE或小时数的框将以红色大纲显示。

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. （可选）单击计划时间线中月份旁边的右箭头，以查看哪些其他月份显示工作角色冲突。

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. （可选）单击显示冲突的工作角色下的&#x200B;**[!UICONTROL 显示详细信息]**，以查看冲突出现的位置并突出显示计划图表区域中的冲突月份。 将显示每个工作角色的附加信息。

   为每个工作角色显示以下字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL可用]</td> 
      <td> <p>计划中每个月的可用工作角色数。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL以前已分配]</td> 
      <td>在特定月份已从计划预算分配给更高层计划的工作角色数量。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL过度分配]</td> 
      <td> <p>计划上所需工作角色的数量与更高层计划后计划可用数量之间的差异也使用了某些角色。 Workfront使用以下公式计算[！UICONTROL过度分配的]职位角色数：</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在计划图表上，分配工作角色的月份显示每个计划所需的角色名称和数量。 必须选择[!UICONTROL 月]视图才能查看工作角色的名称

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. 执行以下操作之一以解决工作角色冲突：

   * 手动将计划每月的工作角色数量调整为较低数量。
   * 将鼠标悬停在工作角色的名称上，然后单击&#x200B;**[!UICONTROL 删除]图标** ![](assets/delete.png)以从计划中删除工作角色。
   * 选择&#x200B;**[!UICONTROL 将角色添加到方案的可用资源]**，然后单击&#x200B;**[!UICONTROL 应用]**。

     这会将缺少的工作角色FTE数或小时数添加到方案的[!UICONTROL 可用]字段。

     >[!NOTE]
     >
     >您添加的用于解决冲突的角色会修改选定方案的[!UICONTROL 可用]工作角色，而非计划中的所有方案。

     计划时间线中针对该月显示一个向上绿色箭头![](assets/upward-green-arrow.png)，表示该月向计划添加了更多资源。 必须选择[!UICONTROL 月]视图才能查看此指示器。

   * （有条件）关闭详细信息面板，如果可能，请为计划提供更高的优先级以首先从计划接收预算资源。 有关更新计划优先级的信息，请参阅Scenario Planner ](../scenario-planner/prioritize-initiatives.md)中的[更新计划优先级。

1. （可选）单击&#x200B;**[!UICONTROL 隐藏详细信息]**&#x200B;以关闭其他详细信息框，然后单击&#x200B;**[!UICONTROL 应用]**&#x200B;以保存您对工作角色所做的更改。

1. （有条件）对于存在成本冲突的计划，请转到计划详细信息面板中的&#x200B;**[!UICONTROL 成本]**&#x200B;部分，以查看计划持续时间的每月成本。 确定计划的预算中哪些月份可能没有足够的资金来支付所选计划的成本。 可用预算不足的框以红色大纲显示。
1. （可选）单击计划时间线中月份旁边的右箭头，以查看预算不足以支付成本的其他月份。

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. （可选）单击成本信息下面的&#x200B;**[!UICONTROL 显示详细信息]**，以查看冲突在哪里出现，并在计划图表上突出显示冲突的月份。 系统会为每种成本类型显示以下附加字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL可用]</td> 
      <td> <p>计划预算中每个月的可用成本。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL以前已分配]</td> 
      <td>该计划预算中已分配给更高层计划的资金量。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL过度分配]</td> 
      <td> <p>计划所需费用与更高层计划之后计划预算中可用资金数额之间的每月差额也使用了一些可用预算。 [!DNL Workfront]使用以下公式计算过度分配的成本数：</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] 使用以下公式计算当前计划每个月的所需成本：</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在计划的图表上，成本不足的月份显示计划仍需要的角色名称和数量。 您必须选择“月份”视图以查看成本额。

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >如果您在创建计划时禁用了计划[!UICONTROL 预算]框的[!UICONTROL 包括人员成本]设置，则任何方案中的任何计划都不会显示[!UICONTROL 人员成本]行。 在这种情况下，Workfront不会计算人员成本以确定成本冲突。 有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

1. 执行以下操作之一来解决成本冲突：

   * 手动将计划每个月的[!UICONTROL 固定成本]的数目调整为一个较低的数字。
   * 在&#x200B;**[!UICONTROL 所需工作角色]**&#x200B;部分中，使用人员成本预算手动调整当月的工作角色数量（如果可能）。 这减少了人员成本。

     >[!TIP]
     >
     >您不能手动调整人员成本。

   * 选择&#x200B;**[!UICONTROL 将金额添加到方案的预算]**，然后单击&#x200B;**[!UICONTROL 应用]**。

     这会将不足的金额添加到缺少该金额的月份的方案预算中，这样也会更新整个方案预算。

     >[!NOTE]
     >
     >为解决成本冲突而添加的金额会修改所选方案的预算，而不是计划中的所有方案的预算。

   * （有条件）关闭详细信息面板，如果可能，请为计划提供更高的优先级以首先从计划接收预算资源。 有关更新计划优先级的信息，请参阅 [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md)中的[更新计划优先级。

1. 对“成本”部分进行任何更改时，单击&#x200B;**[!UICONTROL 应用]**。
1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。


