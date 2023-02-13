---
product-area: enterprise-scenario-planner-product-area
keywords: 发布，计划，项目，方案，方案
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 通过在方案规划器中发布方案来更新或创建项目
description: 您可以通过在Adobe Workfront方案规划器中发布方案，从现有方案创建项目，并更新以前与方案关联的项目。
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '1694'
ht-degree: 0%

---

# 通过在 [!DNL Scenario Planner]

从 [!DNL Adobe Workfront Scenario Planner] 完成以下操作：

* 根据方案中的方案创建项目，并将它们链接在一起。
* 使用链接的倡议提供的信息更新已与情景中的倡议关联的项目。 在将项目导入计划时，也可以将其链接到项目。 有关信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

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
   <td>产品 </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>访问级别*</p> </td> 
   <td> 
    <ul> 
    <li>对的[!UICONTROL Edit]访问权限 [!DNL Scenario Planner] 和项目</li></ul>

<p><b>注释</b>

如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限</p> </td> 
   <td> 
    <ul> 
     <li>计划的[!UICONTROL管理]权限 </li> 
     <li>已发布项目的[!UICONTROL管理]权限</li> 
    </ul> <p>有关请求对项目进行额外访问的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关访问 [!DNL Workfront Scenario Planner]，请参阅 [使用所需的访问权限 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## 先决条件

开始之前：

* 您必须先创建并保存计划，然后才能从中发布方案。

## 有关将计划发布到项目的注意事项

* 您只能发布计划中的一个方案。
* 一个方案只能链接到一个项目。
* 当一个项目属于不同计划时，可以将其链接到多个计划。

   >[!TIP]
   >
   >当一个项目存在于多个计划上，并且您从所有计划将信息发布到该项目时，最新发布会覆盖现有的 [!DNL Scenario Planner] 项目信息。

* 如果通过将项目导入计划来在计划上制定倡议，则发布倡议也会更新链接的项目以提供倡议信息。

   >[!TIP]
   >
   >您可以将同一项目导入多个计划。 发布内容可能会覆盖与多个方案链接的项目中的方案信息。

   有关通过导入项目创建方案的信息，请参阅 [将项目导入 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* 对项目所做的任何更改都不会转移到链接的方案。



## 发布计划

>[!IMPORTANT]
>
>如果对计划中的方案进行了任何更改（包括解决冲突），则必须重新发布方案，以便在项目中显示新信息。 仅当您发布相应的方案时，才会在链接到方案的项目上显示此信息。 有关解决计划之间冲突的信息，请参阅 [解决 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **[!UICONTROL 方案]**
1. （可选并视情况而定）如果要从现有计划中发布，请单击 **[!UICONTROL 过滤器]** 图标 ![](assets/filter-nwepng.png) 在计划的右上角，选择以下选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>显示您拥有或与您共享的所有计划。 这是默认设置。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL我的计划]</td> 
      <td>显示您创建的计划。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL与我共享]</td> 
      <td> <p>显示您未创建但已与您共享的计划。</p> <p>重要信息：您必须拥有与您共享的计划的[!UICONTROL管理]权限，才能发布这些计划。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. （可选）单击 **[!UICONTROL 搜索]** 图标 ![](assets/search-icon.png) 然后开始键入计划的名称，以便快速在列表中找到计划。
1. （视情况而定）要从新计划发布，请创建计划。

   有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. （可选）单击现有计划的名称并为计划创建新方案。

   有关创建计划方案的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. （可选）更新现有或新计划的计划或创建新计划的计划。

   有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. 单击 **[!UICONTROL 保存计划]**.
1. 选择要从 **[!UICONTROL 初始方案]** 下拉菜单，然后单击 **[!UICONTROL 转到发布]** ![](assets/go-to-publish-button-icon.png) 中。

   或

   单击 **[!UICONTROL 比较方案]**，将鼠标悬停在要从中发布的方案卡片上，然后单击 **[!UICONTROL 转到发布]** ![](assets/go-to-publish-button-icon.png).

   的 [!UICONTROL 发布计划] 页面，其中显示了方案中所有方案的列表。 如果之前发布了任何计划，则会显示项目图标 ![](assets/project-icon-sp.png) 显示在其名称和 **[!UICONTROL 上次发布时间]** 日期会填充在列表中。

   >[!TIP]
   >
   >通过导入项目创建的方案也会显示项目图标 ![](assets/project-icon-sp.png) 他们的名字权

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. （可选并视情况而定）如果要从现有计划中发布，请单击 **[!UICONTROL 过滤器]** 图标 ![](assets/filter-nwepng.png) 在计划的右上角，选择以下选项之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>显示选定方案的所有方案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL已发布]</td> 
      <td>显示您或其他用户之前发布的方案。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL已取消发布]</td> 
      <td> <p>显示未发布的方案。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. （可选）单击 **[!UICONTROL 搜索]** 图标 ![](assets/search-icon.png) 然后开始键入计划的名称，以便快速在列表中找到该计划。
1. 选择一个或多个方案以发布和创建或更新项目，然后单击 **[!UICONTROL 发布计划]**.

   这样，如果已发布的方案已链接到项目，则会根据每个选定的方案创建一个新项目，或更新现有的连接项目。

   >[!TIP]
   >
   >新项目与已发布的计划具有相同的名称。

1. （视情况而定）执行下列操作之一：

   * 如果您发布了一个方案，请单击 **[!UICONTROL 请参阅关联项目]** 打开从方案创建或更新的项目。
   * 如果您发布了多个方案，请单击 **[!UICONTROL 查看关联项目]** 以打开从各项举措发布的项目列表。 [!DNL Workfront] 应用 [!DNL Scenario Planner] 默认情况下，项目会过滤到项目列表。 最近发布的项目将显示在列表顶部。

      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. 转到以下区域以查看项目的主动信息：

   * **的 [!UICONTROL 更新] 部分**:会发布一个更新，以指示该项目是通过方案创建或更新的。 更新包含创建或更新项目的方案的名称以及包含方案的计划的链接名称。 您可以单击更新中计划的名称，以在 [!DNL Scenario Planner].

      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **的 [!UICONTROL 概述] 区域 [!UICONTROL 项目详细信息] 部分**:新 [!DNL Scenario Planner] 此区域中会创建包含链接方案信息的部分。

      ![](assets/scenario-planner-on-project-details-350x135.png)

      以下计划信息发布在 [!DNL Scenario Planner] 区域 [!UICONTROL 项目详细信息] 部分：

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL计划持续时间]</span> </td> 
        <td><span>将项目链接到方案时相应方案的持续时间。 此字段不可编辑。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL上次发布日期]</span> </td> 
        <td><span>上次根据相应方案发布项目的日期。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL计划开始日期]</span> </td> 
        <td><span>在计划开始月份的第一天，即项目与计划链接。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL计划结束日期]</span> </td> 
        <td><span>该项目与某个项目链接的计划结束月份的最后一天。 </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL计划FTE和小时中的作业角色]</span> </td> 
        <td> <p>有关相关职务角色及其为计划分配的时间的信息。 这包括：</p> 
         <ul> 
          <li>作业角色名称</li> 
          <li>FTE数</li> 
          <li> <p>所有FTE的小时数</p> <p>您可以使用小时数或FTE估算计划或方案所需的工作角色数量。</p> <p>有关更多信息，请参阅 <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案计划员中创建和编辑计划</a>. </p> </li> 
         </ul> 
      <p><b>笔尖</b>

      如果方案中每个月的职务角色数量不同，则此字段显示方案所需的最大角色数量。 例如，如果您需要1名顾问（1月）和2月（2月），列将显示2FTE以及所有月份2个FTE的相应小时数。</p> </td>
      </tr> 
      </tbody> 
     </table>

      >[!NOTE]
      >
      >具有 [!UICONTROL 查看] 对项目的访问权限可以查看 [!DNL Scenario Planner] 部分 [!UICONTROL 概述] 的上界。 您可以控制此区域是否显示在 [!UICONTROL 详细信息] 区域。 如果用户没有与其关联的布局模板，则默认情况下会显示此区域。
      >
      >   
      >   
      >   * 有关在 [!UICONTROL 详细信息] 部分，请参阅 [自定义 [!UICONTROL 详细信息] 使用布局模板查看](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
      >   * 有关查看 [!UICONTROL 概述] 区域 [!UICONTROL 项目详细信息]，请参阅 [[!UICONTROL 管理] 项目中的信息 [!UICONTROL 概述] 面积](../manage-work/projects/manage-projects/understand-project-overview-area.md).


   * **的 [!UICONTROL 角色分配] 面板 [!UICONTROL 工作负载平衡器] 或项目任务列表**:除了项目中的角色分配之外，该领域还填充了关于方案中角色分配的信息。

      有关更多信息，请参阅 [协调项目和举措之间的资源分配的概述](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

      ![](assets/role-allocation-panel-350x174.png)

      对项目日期或资源的任何更改都不会影响相应的方案或项目中包含方案信息的任何区域。

   * **的 [!UICONTROL 资源预算编制] 区域 [!UICONTROL 商业案例] 项目**:用于使用 [!DNL Scenario Planner] 信息会添加到 [!UICONTROL 资源预算编制] 区域 [!UICONTROL 商业案例] 的项目。

      有关更多信息，请参阅 [预算资源 [!UICONTROL 商业案例] 使用 [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      ![](assets/sp-in-business-case-selected-350x110.png)

1. （可选）在 [!DNL Scenario Planner] 在您发布方案后：

   * 发布的方案将成为您从中发布方案后的第一个方案。
   * 在至少发布了一次方案后，您无法从任何其他方案发布该方案。
   * 的 [!UICONTROL 转到发布] 在从某个方案中至少发布了一个方案后，会从所有其他方案中删除该选项。
   * 计划中已发布计划的项目图标旁边会显示一个绿色指示器。

      ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * 在方案顶部和方案卡上会显示绿色的“已发布”指示器，并在方案卡上填充已发布字段，以指示已发布的方案中的方案数量。

      ![](assets/published-scenario-highlighted-350x632.png)

      >[!TIP]
      >
      >如果删除了从方案的倡议中发布的所有项目，则会删除已发布方案的指示。 有关信息，请参阅 [删除项目](../manage-work/projects/manage-projects/delete-projects.md).

1. （可选）更新有关方案的信息，并重复上述过程，以重新发布方案和更新有关链接项目的方案信息。

   有关编辑方案的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


