---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在Scenario Planner中创建和比较计划方案
description: 在规划公司的长期战略时，您一开始可能没有或想到的信息非常多。 要得出利益相关者可以接受的最终策略，需要时间和试验。 进行“假设”分析为您的计划创建多个场景，可以帮助您准确预测和评估潜在环境，并最终制定最佳可能计划。
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 1%

---

# 在[!DNL Scenario Planner]中创建并比较计划方案

<!--Audited: 07/2024-->

在规划公司的长期战略时，您一开始可能没有或想到的信息非常多。 要得出利益相关者可以接受的最终策略，需要时间和试验。 进行“假设”分析为您的计划创建多个场景，可以帮助您准确预测和评估潜在环境，并最终制定最佳可能计划。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 计划*</p> </td> 
   <td> <p>当前： [！UICONTROL Business]或更高版本</p>
   <p>新增：Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 许可证*</p> </td> 
   <td> <p>新增：浅色或更高</p> 
   <p>当前： [！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td>产品* </td> 
   <td> 
   <p>对于当前Workfront计划： </p>
   <p>您必须为[!DNL Adobe Workfront Scenario Planner]购买额外的许可证才能访问本文中介绍的功能。</p> <p>有关[!DNL Workfront Scenario Planner]的访问权限的信息，请参阅<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用[!DNL Scenario Planner]</a>所需的访问权限。 </p> </td> 
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

## 创建方案

方案是计划的副本。 您可以根据需要创建任意数量的方案。 但是，我们建议您尽量减少场景的数量，以便能够轻松进行比较。

{{step1-to-scenario-planner}}

1. 创建计划或单击现有计划的名称。

   有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

   您创建的第一个计划会自动保存为&quot;[!UICONTROL 初始方案]&quot;。

1. 单击现有方案旁边的向下箭头，然后单击&#x200B;**[!UICONTROL 复制]**&#x200B;图标。

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   这将创建一个与复制的方案具有相同信息的新方案。 如果它是计划的第二个方案，则自动命名为“[!UICONTROL 方案2]”；如果它是第三个方案，则自动命名为“[!UICONTROL 方案3]”，依此类推。 无法重命名方案。 您可以创建的副本数量没有限制。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. 通过以下任一方式更新新方案：

   * 创建、更新或删除计划

     >[!TIP]
     >
     >当您删除方案中的某个方案时，它仅会从选定方案中删除，而不会从所有方案中删除。

     有关创建计划的信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

   * 更新计划的优先级
   * 调整人员或预算信息
   * 查看和调整场景中的计划冲突

     有关解决冲突的信息，请参阅[解决 [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)中的计划冲突。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存更改。

## 比较方案

创建方案后，您可以对其进行比较，以找到最适合您组织的方案。

1. 转到要比较方案的计划。
1. 单击&#x200B;**[!UICONTROL 比较方案]**。 此时将显示方案比较页面。

   计划的所有现有方案都以并排卡片格式显示。 初始方案始终列在首位，并且是静态的。

   ![](assets/scenario-cards-overlapping-350x166.png)

1. （可选）向右滚动查看所有方案卡片。

   以下信息显示在方案卡片上：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>方案的名称</td> 
      <td> <p>由Workfront自动生成的名称，无法编辑。 例如，“[！UICONTROL初始场景]”、“[！UICONTROL场景2]”等。 </p> </td> 
     </tr> 
     <tr> 
      <td>方案描述</td> 
      <td>一个手动条目，您可以在该条目中描述方案的详细信息。 </td> 
     </tr> 
     <tr> 
      <td>可用的职位角色</td> 
      <td>在计划持续时间内，计划预算中可用的工作角色的数量。 </td> 
     </tr> 
     <tr> 
      <td>所需的工作角色</td> 
      <td>所需工作角色的数量，基于您的计划。 </td> 
     </tr> 
     <tr> 
      <td>预算</td> 
      <td>为此方案中的计划定义的总预算。 有关计划的预算信息，请参阅[!DNL Scenario Planner]</a>中的<a href="../scenario-planner/plans-overview.md" class="MCXref xref">计划概览。 </td> 
     </tr> 
     <tr> 
      <td>成本</td> 
      <td>与方案中的计划关联的成本。 有关成本的信息，请参阅[!DNL Scenario Planner]</a>中的<a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">计划概述。 </td> 
     </tr> 
     <tr> 
      <td>利用情况</td> 
      <td>此方案中的计划的[！UICONTROL预算利用率]百分比。 有关[！UICONTROL预算利用率]百分比的信息，请参阅[!DNL Scenario Planner]</a>中的<a href="../scenario-planner/plans-overview.md" class="MCXref xref">计划概览。 </td> 
     </tr> 
     <tr> 
      <td>净值</td> 
      <td>此方案中的计划的[！UICONTROL净值]。 有关计划的[！UICONTROL净值]的信息，请参阅[!DNL Scenario Planner]</a>中的<a href="../scenario-planner/plans-overview.md" class="MCXref xref">计划概述。 </td> 
     </tr> 
     <tr> 
      <td>计划</td> 
      <td>此方案中的计划的计划数。</td> 
     </tr> 
     <tr> 
      <td>冲突</td> 
      <td>在此方案的计划中显示任何类型冲突的计划数。 有关计划冲突的信息，请参阅<a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">解决[!DNL Scenario Planner]</a>中的计划冲突。 </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >当初始方案与其他方案之间的信息不同时，更改的值旁边会显示一个向上或向下箭头，以指示与初始方案相比，该值会增加或减少。
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >例如，预算、工作角色数量、计划数量可能会从一个方案更改为另一个方案。

1. 单击方案的名称以访问方案并进行更改。

   有关详细信息，请参阅本文中的[创建方案](#create-scenarios)部分。

1. 单击&#x200B;**[!UICONTROL 添加描述]**&#x200B;以添加方案的描述

   或

   单击说明字段进行更新，然后单击屏幕上的任意位置保存更改。

1. （可选）单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![](assets/more-icon.png)以&#x200B;**[!UICONTROL 复制]**&#x200B;或&#x200B;**[!UICONTROL 删除]**&#x200B;方案。

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   当您复制方案时，它会自动显示在信息卡页面上，并根据此模式重命名：“[!UICONTROL 方案] `<next number in order>`”。

1. （视情况而定）如果您单击&#x200B;**[!UICONTROL 删除]**，请单击&#x200B;**[!UICONTROL 是，删除它]**&#x200B;以进行确认。

   无法恢复已删除的方案。

   有关删除方案的信息，请参阅[删除 [!DNL Scenario Planner]](../scenario-planner/delete-plans.md)中的计划。

1. 单击&#x200B;**[!UICONTROL 保存计划]**&#x200B;以保存您的方案和计划。
