---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案规划器中创建和编辑方案
description: 使用Adobe Workfront方案计划员时，您可以在您创建的计划或与您共享的计划中创建方案。 通过创建计划，您可以显示较小的组织单位对计划完成的贡献。 例如，如果贵组织有未来三年的计划以扩展到新市场，则您可以在此计划内为每个部门创建计划，以估计每个部门完成此计划所需的人员和预算。
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# 在 [!DNL Scenario Planner]

使用 [!UICONTROL Adobe Workfront方案规划器]，您可以在您创建或与您共享的计划中创建方案。 通过创建计划，您可以显示较小的组织单位对计划完成的贡献。 例如，如果贵组织有未来三年的计划以扩展到新市场，则您可以在此计划内为每个部门创建计划，以估计每个部门完成此计划所需的人员和预算。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证* </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品 </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。 </p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别配置* </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

您必须创建计划，或者其他用户必须与您共享计划，然后才能在该计划内创建方案。 有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

有关什么是计划的更多信息，请参阅 [中的计划概述 [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## 创建计划

您可以通过以下方式创建计划：

* 白手起家。
* 通过将项目导入计划

   有关将项目作为计划中的方案导入的信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 复制现有计划。

   有关复制方案的信息，请参阅 [复制 [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

要从头开始创建计划：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

1. 单击要为其创建方案的计划的名称。
1. 单击 **+图标** 左侧 **[!UICONTROL 新举措]**

   或

   单击 **[!UICONTROL 新举措]** 下拉菜单，然后选择 **[!UICONTROL 新举措]** 或 **[!UICONTROL 导入项目].**

1. 在 **[!UICONTROL 无标题倡议]** ，然后按Enter键或单击页面上的其他位置。

   方案将以蓝色条形显示在计划的时间线上。 默认情况下，方案的持续时间为一个月，并且始终从计划的第一个月开始。

1. （可选）拖动左侧面板和时间轴之间的分隔栏以调整左侧面板的大小。

1. （可选）拖动计划栏的结尾，将持续时间延长到一个多月，并将计划的结束月份发布到您希望的位置。
1. （可选和视情况而定）如果方案的持续时间比计划的持续时间短，请将方案栏拖放到计划时间轴上的其他位置，以将其移动到其他时间范围。

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >您只能选择以月为单位的持续时间。 您从头开始创建的方案的持续时间不能超过计划的持续时间。

1. （可选）从 **[!UICONTROL 月]** 下拉菜单中，选择以下选项之一以更改计划的时间轴：

   | 下拉菜单选项 | 描述 |
   |---|---|
   | [!UICONTROL 月] | 按月显示时间轴。 这是一年计划的默认选项。 |
   | [!UICONTROL 季度] | 按季度显示时间轴。 此选项仅在 [!UICONTROL 持续时间] 计划是三五年。 这是3年计划的默认选项。 |
   | [!UICONTROL 年] | 按年显示时间轴。 此选项仅在 [!UICONTROL 持续时间] 计划是五年。 这是5年计划的默认选项。 |


1. （可选）从左向右滚动以查看计划的整个持续时间。
1. （可选）单击 **[!UICONTROL 今天]** 指示符行返回到当前日期。

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >如果您的计划是在将来或过去，并且不包含当前日期，则不会显示“今天”指示器。

1. 单击方案的栏。 将在右侧打开方案详细信息面板。

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   指定或查看以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">计划持续时间</td> 
      <td>倡议的持续时间（以月为单位）。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">开始和结束日期</td> 
      <td>计划的开始和结束日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所需的作业角色部分 </td> 
      <td> <p>单击 <strong>[!UICONTROL开始键入作业角色]</strong> 字段，然后从列表中选择角色，或开始键入<span>n个活动</span> 作业角色。 </p> <p><span>根据计划是设置为使用FTE还是小时，</span> 在FTE中添加此方案所需的工作角色数 <span><span>或小时</span></span><span> 每月</span>. <span>默认情况下，将显示方案的前三个月。</span></p> <p><span>更新方案的职务职责信息还会更新计划的必需职务职责信息。</span> </p> <p>有关设置计划以使用FTE或小时的信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> <p>提示：  
        <ul> 
         <li> <p><span>使用[!UICONTROL Tab]键移至下个月。</span> </p> </li> 
         <li> <p> 全部 <span>活动</span> 单击此字段时，系统中会列出作业角色。 </p> </li> 
         <li> <p>首先显示已添加到计划的“可用”作业角色中的作业角色。 有关向计划添加可用作业角色的信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案计划员中创建和编辑计划</a>. </p> </li> 
         <li> <p>[!DNL Workfront] 认为全职等效为一个月160小时。 </p> </li> 
        </ul> </p> <p>您可以为FTE输入一个小于1个FTE的数字或小数 <span>或</span> <span data-mc-edit-date="2021-04-22T16:51:21.5923499-04:00" data-mc-editor="alinawilson" data-mc-comment=" yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:00.3159349-04:00">小时</span>. 例如，0.5顾问工作角色意味着顾问将将其一半的FTE（通常为4小时，其中8小时为1个FTE）用于此计划。 </p> <p>对于方案计划器中的所有计算，Workfront会使用以下值：1个FTE = 8小时。 </p> </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">费用科</td> 
      <td> <p>在[!UICONTROL成本]部分的右侧，将显示方案的总成本。 [!DNL Workfront] 使用以下公式计算方案成本：</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>在 <strong>[!UICONTROL固定成本]</strong> 字段中，手动输入您认为完成此方案将花费的粗略估计金额。 这不应包括与该倡议估计的工作角色相关的费用。</p> <p><span>在使用Tab键时，通过从一个月移动到下一个月，输入方案每月的金额。</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>根据计划是设置为使用FTE还是小时，[!UICONTROL Workfront]使用以下公式计算[!UICONTROL人员成本]:</p> 
        <ul> 
         <li> <p>使用FTE时： </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>，其中160是一个月内的总工作小时数。 </p> </li> 
         <li> <p style="font-weight: normal;">使用小时： </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">有关设置计划以使用小时或FTE的信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案计划员中创建和编辑计划</a>.</p> </li> 
        </ul> 
        <p>人员成本以在“汇率”首选项中选择的基本货币计算。 有关汇率的信息，请参阅 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> 
        <p>更新方案的成本信息还会更新计划的[!UICONTROL成本]区域。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">在您定义了方案所需的任务职责和成本值并修改方案的持续时间后，可能会出现以下情况之一：</p> 
       <ul> 
        <li> <p style="font-weight: normal;">如果缩短计划， [!DNL Workfront] 删除所需资源金额和与从计划中删除的时间关联的成本。 工作角色仍保留在计划中，但它们没有必需的FTE或 <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">小时</span>. 计划和预算的可用资源保持不变。<br>有关计划的信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">如果您延长方案时间，则必须指定方案中新添加月份的职务职责和成本金额。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] 部分</td> 
      <td>在 <strong>[!DNL Net Value]</strong> 部分，在 <strong>[!UICONTROL计划收益]</strong> 字段。 这就是你所相信的实现这一倡议的好处。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果您已经为计划定义了职务职责数和预算、所编辑的职务职责数和方案及其上所有方案的成本，并且这些任务和预算都超过了您为计划指定的金额， [!DNL Workfront] 可能会发现您没有足够的资源来完成该计划。 [!DNL Workfront] 在尝试实现此方案时，会将其标记为冲突，并将其显示为红色条。 所有遵循矛盾倡议的倡议都以红色背景显示。 您可能需要从资源不足的第一个计划开始调整一些计划的需求。 有关调整冲突方案的信息，请参阅 [解决 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. （可选）将鼠标悬停在作业角色的名称上，然后单击 **[!UICONTROL 垃圾桶图标]** ![](assets/delete.png) 将其从计划中删除。

1. （视情况而定）如果您对方案进行了更改，请单击 **[!UICONTROL 应用]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. （视情况而定）如果您未进行任何更改，请单击 **X** 图标来关闭它。
1. （可选）更新您的计划的优先级。

   有关优先排定各项倡议的信息，请参阅 [更新方案计划员中的方案优先级](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >列在清单第一的倡议具有更高的优先权，在列在清单下方的倡议之前获得资源。

1. 单击 **[!UICONTROL 保存计划]**.

   该计划现已纳入您的计划。

   有关从计划中删除方案的信息，请参阅 [删除 [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
