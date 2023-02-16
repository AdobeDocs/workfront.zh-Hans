---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案计划员中创建和编辑计划
description: 在对公司的较高级别策略进行优先级排序时，您可以在使用Workfront方案计划器时创建计划。 有关计划的详细信息，请参阅方案计划员中的计划概览。
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2402'
ht-degree: 1%

---

# 在 [!DNL Scenario Planner]

您可以使用 [!DNL Workfront Scenario Planner]，以确定贵公司更高级别战略的优先级。 有关计划的更多信息，请参阅 [中的计划概述 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

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
   <td> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品</td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取[!UICONTROL Workfront Scenario Planner]的信息，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!UICONTROL Scenario Planner]所需的访问权限</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别配置* </td> 
   <td> <p>[!UICONTROL Edit]对 [!DNL Scenario Planner]</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限 </p> </td> 
   <td> <p>[!DNL Manage] 计划权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建或编辑计划

您可以从头开始创建计划，也可以编辑与您共享的现有计划。

>[!NOTE]
>
>创建计划后，您将被视为计划创建者和所有者。 停用某个用户后，该计划没有所有者，任何人都不可见，除非之前已与某个链接共享。

本文介绍了如何从头开始创建计划，或如何编辑现有计划。

有关计划的所有考虑事项（包括计划可用的信息），请参阅 [中的计划概述 [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

有关删除计划的信息，请参阅 [删除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

要创建或编辑计划，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

   您创建的现有计划列表将显示在 [!DNL Workfront Scenario Planner].

1. （可选）单击 **[!UICONTROL 过滤器]** 图标 ![](assets/filter-icon-34x37.png)在计划列表的右上角，从以下位置选择：

   | 筛选 | 描述 |
   |---|---|
   | [!UICONTROL 全部] | 显示您创建或与您共享的所有计划。 |
   | [!UICONTROL 我的计划] | 显示您创建的计划。 |
   | [!UICONTROL 已与我共享] | 显示与您共享的计划。 |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （可选）单击 **[!UICONTROL 搜索]** 图标 ![](assets/search-icon.png) 键入关键词并快速在列表中找到计划。

1. 单击现有计划的名称以对其进行编辑，并继续执行步骤7。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   或

   单击 **[!UICONTROL 新计划]** 创建计划并继续执行步骤5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   的 [!UICONTROL 新计划] 框中。

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. （视情况而定）创建新计划时，请指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td>键入计划的名称。 这是必填字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>重要信息： <span style="font-weight: normal;">在创建并保存计划后，您不能修改以下选择。</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE（[!UICONTROL相当于全时]）或[!UICONTROL小时数]</span> </td> 
      <td> <p><span>选择以下选项之一，以指示您要如何估计此计划的任务职责信息：</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. 这是默认设置 </span> </p> 
      <p><b>重要信息</b></p>  
      <p>对于 [!DNL Scenario Planner], [!DNL Workfront] 使用以下值：1个FTE = 8小时。 </p> </li> 
      <li> <p><strong>[!UICONTROL小时数]</strong> </p> </li> 
       </ul> <p><b>重要信息</b></p>

   您在此处选择的选项可确定如何显示计划、计划方案和方案的职务职责信息</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL开始日期]</td> 
      <td> <p>选择您希望计划开始的月份和年份。 在此字段中只能选择月。 [!DNL Workfront] 假定计划的开始日期是选定月份的第一天，结束日期是该月份持续时间内月末的最后一天。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL持续时间]</td> 
      <td> <p>从下拉菜单中，从以下持续时间中进行选择：</p> 
       <ul> 
        <li>1 年. 这是默认的持续时间。 </li> 
        <li>3年</li> 
        <li> <p>5年</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. （视情况而定）单击 **[!UICONTROL 下一个]**.

   计划的时间轴显示为 **[!UICONTROL 初始方案]**.

   有关创建其他方案的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. （可选）从时间轴下拉菜单中，选择下表中的一个选项，以更改您查看计划时间轴的方式。

   ![](assets/month-dropdown-with-all-options.png)

   | 下拉菜单选项 | 描述 |
   |---|---|
   | [!UICONTROL 月] | 按月显示时间轴。 这是一年计划的默认和唯一选项。 |
   | [!UICONTROL 季度] | 按季度显示时间轴。 此选项仅在 [!UICONTROL 持续时间] 计划是三五年。 这是3年计划的默认选项。 |
   | [!UICONTROL 年] | 按年显示时间轴。 此选项仅在 [!UICONTROL 持续时间] 计划是五年。 这是5年计划的默认选项。 |

1. （可选）从左到右滚动以查看计划的整个持续时间。
1. （可选）单击 **[!UICONTROL 今天]** 指示符行返回到当天。

   ![](assets/today-indicator-350x160.png)

1. 单击 **[!UICONTROL 作业角色]** 框，以添加可用于执行计划的作业角色。

   详细信息 [!UICONTROL 作业角色] 框中。

   >[!TIP]
   >
   >角色分配单位（FTE或小时） [!DNL Workfront] 此计划的用法显示在框标题的圆括号中。

   ![](assets/adding-people-to-plan-350x206.png)

1. 单击 **[!UICONTROL 开始键入作业角色]** 字段，从列表中选择角色或开始键入活动作业角色的名称。

   单击此字段时，系统中的所有活动作业角色都将列出。

   这会将作业角色添加到“作业角色”列。

1. 更新或查看作业角色的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL最大可用数]（对于FTE） </p> <p role="rowheader">或 </p> <p role="rowheader"><span>[!UICONTROL可用总数]（小时）</span> </p> </td> 
      <td> <p><span>根据您选择使用小时还是FTE来进行计划，键入</span> 职务角色FTE的数量 <span>或小时</span> 可用于在以下字段中执行计划工作： </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL可用总数]</strong> （表示小时）：指示在方案期间所有月份的总小时数。 默认情况下， [!DNL Workfront] 在方案持续期间的所有月份中平均分配可用总数。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>如果为设计人员输入1200小时，则表示在计划期间，当计划[!UICONTROL持续时间]为1年时，设计人员每月可使用100小时。 </p> </li> 
        <li> <p><b>[!UICONTROL最大可用数]</b> （对于FTE）：指示在计划期间每个月有工作角色可用的FTE数。 默认情况下， <strong>Workfront</strong> 在方案持续期间，为每月分配[!UICONTROL Max available]数字。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>如果为顾问输入1个FTE，则表示在计划期间，顾问每月可用1个FTE。 </p> <p>您可以输入一个小于1个FTE的数字。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>0.5顾问工作角色意味着顾问将其一半的FTE（通常为4小时，其中8小时是1个FTE）用于处理此计划。 对于方案计划器中的所有计算，Workfront会使用以下值：1个FTE = 8小时。 </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL最大必需值]（对于FTE）</p> <p role="rowheader">或 </p> <p role="rowheader"><span>[!UICONTROL所需总数]（小时）</span> </p> </td> 
      <td> <p><span>根据您选择使用小时还是FTE来进行计划，请查看</span> 职务角色FTE的数量 <span>或小时</span> 要在此情景中完成各项计划所必需的。 查看以下字段：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL总需要]</strong> （表示小时）：计划期间所有月份所需的总小时数。</p> </li> 
        <li> <p><strong>[!UICONTROL最大必需值]</strong> （对于FTE）：计划期间任何月份所需的最大FTE数。 </p> </li> 
       </ul> <p>提示：的 <span>最大值</span> FTE数量 <span>或总小时数</span> 在开始添加方案后，将显示该作业角色的必需参数。 有关向计划添加计划的信息，请参阅 <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">在 [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL每小时费率]</td> 
      <td> <p>这是作业角色的[!UICONTROL成本小时]费率。 每小时费率以系统的货币显示。 有关为系统设置汇率的信息，请参阅 <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">设置汇率</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）将鼠标悬停在作业角色的名称上，或在更新角色信息后单击选项卡，然后单击 **[!UICONTROL 垃圾桶图标]** ![](assets/delete.png) 把它从计划中移除。
1. 单击 **[!UICONTROL 职务角色分配]**.

   在方案持续期间，将针对所有月份显示作业角色分配面板。

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. 键入职务角色的名称，以将其添加到 **[!UICONTROL 开始键入作业角色字段]**，然后在列表中显示时单击Enter 。 这会将作业角色添加到 [!UICONTROL 作业角色] 列。
1. 更新或查看方案每个月的以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL作业角色]（FTE或小时）</td> 
      <td>方案可用的作业角色和方案中的方案所需的作业角色都显示在作业角色分配面板中。 在列标题中有一个指示是工作角色估计是在FTE中还是在小时中。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL可用](最大值 &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>或</p> 
        <p>[!UICONTROL可用](总计 &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>根据您选择使用小时数还是FTE进行计划、审核或更新</span> 每月FTE的职务角色数 <span>或小时</span> 适用于以下字段中的方案：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL可用](最大值 &lt;number of="" ftes=""&gt;)</strong>:括号中的数字显示方案中任一月份可用角色的最大数量。 查看或更新方案每月的FTE数量。 更改月度分配可能会更新括号中的FTE数量。 </p> </li> 
        <li> <p><span><strong>[!UICONTROL可用](总计 &lt;number of="" hours=""&gt;)</strong>:括号中的数字显示方案中所有月份的可用小时总数。 查看或更新方案每月的小时数。 更改月度分配会更新括号中的小时数。</span> </p> </li> 
       </ul> <p>手动更新每月职务角色分配是解决方案中各方案之间职务角色冲突的另一种方法。 </p> <p>提示：   <p><span>要更新几个月的每月角色可用性，请在任意月份的[!UICONTROL Available]字段中键入小时数或FTE，然后拖动字段的角在相邻月份上以复制每月的相同值。 将其删除以更新所有月份。</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL必需](最大值 &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">或</p> 
        <p role="rowheader">[!UICONTROL必需](总计 &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>根据您选择使用小时还是FTE来进行计划，请查看</span> 在以下字段中，此方案需要的工作角色FTE的月数或小时数： </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL必需](最大值 &lt;number of="" ftes=""&gt;)</strong>:括号中的数字显示方案中任何一个月份所需的最大角色数。 </p> </li> 
        <li> <p><span><strong>[!UICONTROL必需](总计 &lt;number of="" hours=""&gt;)</strong>:括号中的数字显示方案中所有月份所需的总小时数。</span> </p> </li> 
       </ul> <p>提示：您无法修改所需的FTE数 <span>或小时</span> 作业角色。 在您开始添加方案及其职务职责要求后，方案中会填充此数字。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>方案的必需作业角色和可用作业角色之间的月差。 [!DNL Workfront] 使用以下公式计算每个月每个作业角色的差异：</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> （在FTE或小时中） </p> 
        <p>提示：当差异显示负数时，方案需要的任务职责比计划可用的职责多。 您的资源已过度分配。 </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL利用率] %</td> 
      <td> 
       <div> 
        <p>利用率百分比显示方案中方案实际使用（或需要）多少个可用作业角色。 </p> 
        <p>[!DNL Workfront] 使用以下公式计算每月每个作业角色的利用率： </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>利用率百分比可能以下列颜色显示，具体取决于资源的分配：</p> 
        <ul> 
         <li> <p><b>绿色</b>:作业角色的可用数量与所需数量相匹配。 资源已完全分配，利用率为100%。 </p> </li> 
         <li> <p><b>红色</b>:所需的作业角色比计划可用的要多。 资源被过度分配，利用率高于100%。</p> </li> 
         <li> <p><b>蓝色</b>:可用的作业角色比所需的要多。 资源分配不足，利用率低于100%。 </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 应用]** 保存每月的工作角色分配

   或

   单击 **[!UICONTROL 取消]** 关闭作业角色分发列表并返回到方案。

1. 单击 **[!UICONTROL 金融]** 框，以添加此计划的预算。

   详细信息 [!UICONTROL 金融] 框中。

   >[!TIP]
   >
   >货币 [!DNL Workfront] 此计划的用法显示在框标题的圆括号中。

1. 指定 **[!UICONTROL 年度预算]**.

   >[!NOTE]
   >
   >如果您的计划跨多年，则必须为每年指定预算金额。

1. 按Enter键保存年度预算，然后 [!UICONTROL 选项卡] 转到第二年。

   对于选定年份的每个月，每年预算会自动平均分配。

1. 单击 **[!UICONTROL 高级]** 以查看每月预算分配。 年度预算和月度预算始终为四舍五入数字。 当预算金额由于小数而不能平均分配给一年内所有月份时 **[!UICONTROL 剩余]** 指标显示在年度预算分配下。

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. 人工调整月度预算以消除超出的金额。

   当所有月预算金额的合计大于年度预算时， **[!UICONTROL 超出]** 警告指示器显示在年度预算分配下。 人工调整月度预算金额，直到它们等于或低于计划的可用预算。

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. 禁用 **[!UICONTROL 包括人员成本]** 设置以排除与任务角色关联的成本，使其从计算到计划的整体成本。 固定成本始终计入计划的整体成本。 此设置默认启用，并影响计划上的所有方案。
1. 单击 [!UICONTROL 金融] 框来关闭它。 您输入的信息会自动保存。

   您现在可以开始创建计划中的计划并添加方案。

1. （推荐）单击 **[!UICONTROL 新举措]** 添加新计划。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   有关添加计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. （可选）复制现有方案以创建同一计划的新方案。 有关创建和使用多个方案的更多信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. 单击 **[!UICONTROL 保存计划]**.

   计划已创建或更新。

1. （可选）单击 **[!UICONTROL “收藏夹”图标]** ![](assets/favorites-icon-small.png) 在计划名称的右侧，将计划添加到收藏夹列表。

1. （可选）复制计划的URL，并将其发送给可能需要查看或更新该计划的任何其他用户。 他们至少 [!UICONTROL 查看] 访问其访问级别，以便能够查看计划。 他们肯定有 [!UICONTROL 编辑] 有权编辑。 如果他们必须审核计划的财务信息，如预算、成本和职务职责费率信息，则他们还必须有权访问 [!UICONTROL 财务数据] 访问级别。 有关 [!DNL Scenario Planner]，请参阅 [使用所需的访问权限 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
