---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在方案计划员中创建和比较计划方案
description: 在规划公司的长期战略时，您可能会在开始时没有或想过许多信息。 制定利益相关方可以接受的最终策略需要时间和实验。 进行“假设”分析以为计划创建多个方案，可以帮助您准确预测和评估潜在情况，并最终制定最佳的可能计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# 在 [!DNL Scenario Planner]

在规划公司的长期战略时，您可能会在开始时没有或想过许多信息。 制定利益相关方可以接受的最终策略需要时间和实验。 进行“假设”分析以为计划创建多个方案，可以帮助您准确预测和评估潜在情况，并最终制定最佳的可能计划。

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
   <td> <p>编辑对 [!DNL Scenario Planner]</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL管理]计划的权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">请求对 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 创建方案

方案是计划的副本。 您可以根据需要创建任意数量的方案。 但是，我们建议您尽量减少方案数量，以便轻松进行比较。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png)，然后单击 [!UICONTROL 方案].

1. 创建计划。

   有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   您创建的第一个计划会自动另存为“[!UICONTROL 初始方案].&quot;

1. 单击现有方案旁边的向下箭头，然后单击 **[!UICONTROL 复制]** 图标。

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   这会创建一个新方案，其中包含与复制的方案相同的信息。 它自动命名为“[!UICONTROL 场景2]“如果这是您计划的第二种情况，”[!UICONTROL 场景3]“如果是第三个，依此类推。 无法重命名方案。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 通过以下任一方式更新新方案：

   * 创建、更新或删除方案

      >[!TIP]
      >
      >在方案中删除方案时，它仅会从选定方案中删除，而不会从所有方案中删除。

      有关创建计划的信息，请参阅 [在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * 更新贵机构计划的优先事项
   * 调整人员或预算信息
   * 在您的方案中查看并调整方案冲突

      有关解决冲突的信息，请参阅 [解决 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. 单击 **[!UICONTROL 保存计划]** 以保存更改。

## 比较方案

创建方案后，您可以比较它们以找到适合贵组织的最佳方案。

1. 转到要比较方案的计划。
1. 单击 **[!UICONTROL 比较方案]**. 此时将显示方案比较页。

   计划的所有现有方案都以并排卡片格式显示。 初始方案始终最先列出，且是静态的。

   ![](assets/scenario-cards-overlapping-350x166.png)

1. （可选）滚动到右侧以查看所有方案卡片。

   方案卡片上会显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>方案的名称</td> 
      <td> <p>由Workfront自动生成的名称，无法编辑。 例如，“[!UICONTROL Initial scenario]”、“[!UICONTROL Scenario 2]”等。 </p> </td> 
     </tr> 
     <tr> 
      <td>方案描述</td> 
      <td>手动输入，您可以在其中描述方案的具体信息。 </td> 
     </tr> 
     <tr> 
      <td>可用的作业角色</td> 
      <td>在计划期间计划预算中可用的职务角色数。 </td> 
     </tr> 
     <tr> 
      <td>所需的工作角色</td> 
      <td>根据您的计划，需要的工作角色数量。 </td> 
     </tr> 
     <tr> 
      <td>预算</td> 
      <td>在此方案中为计划定义的总预算。 有关计划的预算信息，请参阅 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的计划概述 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>成本</td> 
      <td>与方案中的计划相关的成本。 有关成本的信息，请参阅 <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">中的计划概述 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>利用</td> 
      <td>此方案中计划的[!UICONTROL预算利用率]百分比。 有关[!UICONTROL预算利用率]百分比的信息，请参阅 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的计划概述 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>净值</td> 
      <td>此方案中计划的[!UICONTROL净值]。 有关计划的[!UICONTROL净值]的信息，请参阅 <a href="../scenario-planner/plans-overview.md" class="MCXref xref">中的计划概述 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>计划</td> 
      <td>此情景中计划的计划数。</td> 
     </tr> 
     <tr> 
      <td>冲突</td> 
      <td>在此方案的计划中显示任何类型冲突的方案数量。 有关计划冲突的信息，请参阅 <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">解决 [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >如果初始方案和其他方案中的信息不同，则在值旁边会显示向上或向下箭头，指示与初始方案相比该值有增加或减少。
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >例如，预算、工作角色数、倡议数量可能会从一种情况更改为另一种情况。

1. 单击方案的名称以访问该方案并对其进行更改。

   有关更多信息，请参阅 [创建方案](#create-scenarios) 章节。

1. 单击 **[!UICONTROL 添加描述]** 为方案添加描述

   或

   单击描述字段以更新该字段，然后单击屏幕上的任意位置以保存更改。

1. （可选）单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-icon.png) to **[!UICONTROL 复制]** 或 **[!UICONTROL 删除]** 方案。

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   复制方案时，该方案会自动显示在卡片页面上，并会根据以下模式重命名：&quot;[!UICONTROL 方案] `<next number in order>`.&quot;

1. （视情况而定）如果您单击 **[!UICONTROL 删除]**，单击 **[!UICONTROL 是，删除它]** 确认。

   无法恢复已删除的方案。

   有关删除方案的信息，请参阅 [删除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. 单击 **[!UICONTROL 保存计划]** 以保存您的方案和计划。
