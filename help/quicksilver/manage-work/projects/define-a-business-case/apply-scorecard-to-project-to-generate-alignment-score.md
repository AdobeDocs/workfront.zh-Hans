---
navigation-topic: business-case-and-scorecards
title: 将记分卡应用于项目并生成一致性分数
description: 您可以使用记分卡衡量项目与项目组合中先前建立的标准的匹配程度。 记分卡通常反映了组织的使命、价值观和战略目标。
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 14b6b9c4a184131cfdc33b6156c578218ed9119a
workflow-type: tm+mt
source-wordcount: '1208'
ht-degree: 0%

---

# 将记分卡应用于项目并生成一致性分数

<!-- Audited: 06/2025 -->

您可以使用记分卡衡量项目与项目组合中先前建立的标准的匹配程度。 记分卡通常反映了组织的使命、价值观和战略目标。

有关记分卡以及如何创建记分卡的更多信息，请参阅[创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td>
   <p>当前：Prime或更高版本</p>
   <p>或</p>
   <p>旧版：商业版或更高版本</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>
   <p>当前：标准</p>
   <p>或</p>
   <p>旧版：计划</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> <p>查看或更高的项目组合访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>管理项目的权限</p> <p>查看项目组合或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 项目记分卡 {#project-scorecards}

* [记分卡概述](#scorecards-overview)
* [将记分卡应用到项目](#apply-a-scorecard-to-a-project)

### 记分卡概述 {#scorecards-overview}

通常，项目经理会完成记分卡信息，以便为项目生成介于0和100之间的对齐值。 项目组合经理稍后在项目组合优化器中查看项目以比较它们时，将使用生成的值。

有关项目组合优化的更多信息，请参阅[Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

### 将记分卡应用到项目

作为具有Standard或Plan许可证以及项目的“管理”权限的用户，您可以为项目附加记分卡。

有关项目权限的详细信息，请参阅[在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

您可以在构建项目的业务案例时向项目添加记分卡。

有关构建业务案例的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您的Adobe Workfront管理员或组管理员必须在项目的业务案例区域中启用“记分卡”部分，然后才能从业务案例访问记分卡。 有关设置项目首选项和启用Business Case区域的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

要将记分卡应用到项目，请执行以下操作：

1. 转到要应用记分卡的项目。
1. 单击左侧面板中的&#x200B;**业务案例**。
1. 查找业务案例的&#x200B;**记分卡**&#x200B;部分。\
   您必须先创建记分卡，然后才能在业务案例中显示&#x200B;**记分卡**&#x200B;部分。

   有关创建记分卡的信息，请参阅[创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

1. 从下拉菜单中选择一个记分卡。

   <!--![New scorecard](assets/new-scorecard.png)-->

1. 为记分卡中的所有问题输入答案。

   Workfront将分数应用于每个已回答的问题，并根据每个问题的单独分数计算项目整体分数。

   有关生成项目整体一致性分数的详细信息，请参阅[生成项目的一致性分数](#generate-an-alignment-score-for-a-project)。

1. 单击&#x200B;**保存**&#x200B;以保存记分卡并对项目评分。

   记分卡现在与项目关联，并对项目进行评分。

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## 生成对齐分数

* [生成项目的对齐分数](#generate-an-alignment-score-for-a-project)
* [生成项目组合的对齐分数](#generate-an-alignment-score-for-a-portfolio)

### 生成项目的对齐分数 {#generate-an-alignment-score-for-a-project}

一致性分数是完成记分卡后生成的值。

记分卡包含带有已分配数值（称为对齐点）的答案选项的问题。 这些要点用于确定项目与您的组织的匹配程度。 每个问题的对齐点都包含一个介于0和100之间的数字。

评分卡完成后，Workfront会使用以下公式以百分比计算项目的对齐分数：

`Project Alignment Score = The sum of the question points from the scorecard met at a given time / The sum of the possible points on the scorecard`

有关详细信息，请参阅[创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

### 生成项目组合的对齐分数 {#generate-an-alignment-score-for-a-portfolio}

项目组合的一致性分数是项目组合中所有项目的平均一致性分数。

当项目的记分卡完成时，Workfront使用这些值通过下列公式以百分比形式计算项目组合的对齐分数：

`Portfolio Alignment Score = The sum of the percentages of the project alignment scores / Number of projects in the portfolio`

>[!NOTE]
>
>如果项目没有与其关联的记分卡，因此没有一致性分数，则项目组合中的一致性被认为为0%。 在项目组合的项目数中考虑项目。

## 查看一致性分数

您可以在项目级别或Portfolio Optimizer中查看项目的对齐分数。

* [查看项目的对齐分数](#view-the-alignment-score-on-a-project)
* [在Portfolio Optimizer中查看项目与项目组合的对齐分数](#view-the-alignment-scores-of-the-project-and-of-the-portfolio-in-the-portfolio-optimizer)

### 查看项目中的一致性分数

如果您拥有项目的“参与”权限，则可以在项目级别查看项目的对齐分数。

1. 转到要查看其一致性分数的项目。
1. 单击左侧面板中的&#x200B;**业务案例**。
1. 转到屏幕右侧的&#x200B;**业务案例摘要**。

   一致性分数位于业务案例摘要中，位于&#x200B;**一致性**&#x200B;值中。

   <!--![Alignment score on a project](assets/alignment-score-on-a-project.png)-->

### 在Portfolio Optimizer中查看项目与项目组合的对齐分数

如果您拥有项目组合的管理访问权限，则可以在Portfolio Optimizer中查看项目或项目组合的对齐分数。

有关Portfolio Optimizer中显示信息的更多信息，请参阅[Portfolio Optimizer概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

* [在Portfolio Optimizer中找到项目的对齐分数](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [在Portfolio Optimizer中找到项目组合的对齐分数](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  <!--![Alignment score in Portfolio Optimizer](assets/alignment-score-in-portfolio-optimizer.png)-->

#### 在Portfolio Optimizer中找到项目的对齐分数 {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. 单击项目组合的名称。
1. 单击左侧面板中的&#x200B;**Portfolio优化**。

   此时将显示Portfolio Optimizer。

   项目的对齐分数在Portfolio优化器的&#x200B;**对齐**&#x200B;列中以百分比显示。

   这是基于与项目关联的记分卡的项目的对齐分数。

#### 在Portfolio Optimizer中找到项目组合的对齐分数  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

{{step1-to-portfolios}}

1. 单击项目组合的名称。
1. 单击左侧面板中的&#x200B;**Portfolio优化**。
1. 在Portfolio优化器的顶部找到&#x200B;**Aligned**&#x200B;值以及&#x200B;**Alignment**&#x200B;量规，它们表示项目组合的对齐分数。

   这是项目组合的对齐分数。

   有关如何生成项目组合的对齐分数的详细信息，请参阅[生成项目组合的对齐分数](#generate-an-alignment-score-for-a-portfolio)。

## Portfolio Optimizer得分概述

项目一致性分数与项目组合优化器分数之间存在差异。

根据完成记分卡后获得的点数计算项目的对齐分数。 然后，将使用该得分确定项目组合匹配度分数。 一致性分数以百分比显示。

项目的对齐分数显示在Portfolio优化器的&#x200B;**对齐**&#x200B;列中。

项目组合优化器得分是在Portfolio优化器中自动计算的排名，通过它可以对项目进行优先排序。 项目组合优化器得分显示为指示符图标，旁边带有一个数字，并显示在Portfolio优化器的&#x200B;**得分**&#x200B;列中。 仅当完成业务案例的所有部分（目标除外）时，才会生成Portfolio Optimizer分数。

有关为项目创建业务案例的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

有关计算项目的项目组合优化器得分的详细信息，请参阅[Portfolio优化器得分概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md)。
