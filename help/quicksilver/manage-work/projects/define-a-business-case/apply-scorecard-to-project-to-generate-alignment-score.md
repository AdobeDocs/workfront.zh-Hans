---
navigation-topic: business-case-and-scorecards
title: 将记分卡应用于项目并生成对齐分数
description: 您可以使用评分卡衡量项目与之前已建立的项目组合标准的一致程度。 评分卡通常反映组织的使命、价值和战略目标。
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '1420'
ht-degree: 0%

---

# 将记分卡应用于项目并生成对齐分数

<span class="preview">此页面上突出显示的信息是指目前尚不普遍可用的功能。 它仅在“预览”环境中可用。</span>

您可以使用评分卡衡量项目与之前已建立的项目组合标准的一致程度。 评分卡通常反映组织的使命、价值和战略目标。

有关记分卡以及如何创建记分卡的更多信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>业务或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>查看或更高权限访问Portfolio</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>查看或更高对组合的权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 项目记分卡 {#project-scorecards}

* [记分卡概述](#scorecards-overview)
* [项目记分卡](#project-scorecards)

### 记分卡概述 {#scorecards-overview}

通常，项目管理器会完成记分卡信息，以便为项目生成一个介于0到100之间的对齐值。 产生的值稍后在组合经理审核组合优化器中的项目以比较时使用。

有关组合优化的更多信息，请参阅文章 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### 将记分卡应用于项目

作为具有计划许可证和管理项目权限的用户，您可以将记分卡附加到项目。

有关项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

您可以在项目中添加记分卡，作为构建项目业务案例的一部分。

有关构建业务案例的更多信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您的Adobe Workfront管理员或组管理员必须先在项目的“业务案例”区域中启用记分卡部分，然后才能从“业务案例”中访问记分卡。 有关设置项目首选项和启用业务案例区域的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

要将记分卡应用到项目，请执行以下操作：

1. 转到要应用记分卡的项目。
1. 单击 **商业案例** 中。
1. 查找 **记分卡** 部分。\
   您必须在 **记分卡** 部分。

   有关创建记分卡的信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. 从下拉菜单中选择记分卡。

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. 在评分卡中为所有问题指定答案。

   Workfront对每个已回答的问题都应用一个分数，并根据每个问题的单个分数计算总体项目分数。

   有关生成项目整体对齐分数的更多信息，请参阅 [为项目生成对齐分数](#generate-an-alignment-score-for-a-project).

1. 单击 **保存** 以保存记分卡并对项目进行评分。

   记分卡现在与项目关联，并且项目已进行评分。

1. （视情况而定）当记分卡问题的值发生更改时，必须重新计算记分卡以反映项目得分的新值。 要重定记分卡，请执行以下操作：

   1. 转到项目列表，然后选择列表中的所有项目。
   1. 单击 **编辑** 图标。
   1. 单击 **设置** 在左侧面板中，然后检查 **重新计算记分卡** 选项。
   1. 单击保存。这会根据为所有选定项目附加的记分卡来重新计算得分值。

      >[!NOTE]
      >
      >   <span class="preview">批量编辑项目时，用于重新计算记分卡的选项已从预览环境中删除。 </span>


## 生成对齐分数

* [为项目生成对齐分数](#generate-an-alignment-score-for-a-project)
* [为组合生成对齐分数](#generate-an-alignment-score-for-a-portfolio)

### 为项目生成对齐分数 {#generate-an-alignment-score-for-a-project}

对齐分数是完成记分卡后生成的值。

记分卡包含带有已分配数值（称为对齐点）的答案选项的问题。 这些要点用于确定项目与贵组织的一致程度。 每个问题的对齐点都包含一个介于0和100之间的数字。

完成记分卡后，Workfront使用以下公式计算项目的对齐分数（以百分比表示）：

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

有关更多信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### 为组合生成对齐分数 {#generate-an-alignment-score-for-a-portfolio}

组合的对齐分数是组合中所有项目的对齐分数的平均值。

项目的记分卡完成后，Workfront会使用这些值通过以下公式计算组合的对齐分数（以百分比表示）：

Portfolio对齐分数=项目对齐分数的百分比总和/项目组合中的项目数

>[!NOTE]
>
>如果某个项目没有与其关联的记分卡，因此没有对齐分数，则在项目组合中将其视为具有0%的对齐分数。 项目在项目组合中的项目数量中予以考虑。

## 查看对齐分数

您可以在项目级别或Portfolio优化器中查看项目的对齐分数。

* [查看项目的对齐分数](#View%20the)
* [在Portfolio优化器中查看项目和项目组合的对齐分数](#View%20the2)

### 查看项目的对齐分数

如果您对项目具有“参与”权限，则可以在项目级别查看项目的协调得分。

1. 转到要查看其对齐分数的项目。
1. 单击 **商业案例** 中。
1. 转到 **业务案例摘要** 屏幕右侧。

   协调得分位于“业务案例摘要”中，位于 **对齐** 值。

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### 在Portfolio优化器中查看项目和项目组合的对齐分数

如果您有权管理Portfolio组合，则可以在Analytics Optimizer中查看项目或组合的对齐分数。

有关Portfolio优化器中显示的信息的更多信息，请参阅 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [在Portfolio优化器中找到项目的对齐分数](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [在Portfolio优化器中找到组合的对齐分数](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### 在Portfolio优化器中找到项目的对齐分数 {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，则 **Portfolio**.

1. 单击Portfolio的名称。
1. 单击 **Portfolio优化** 中。

   此时将显示Portfolio优化程序。

1. 项目的对齐分数以百分比的形式显示在 **对齐方式** 列的Portfolio优化程序。

   这是基于与项目关联的记分卡的项目对齐分数。

#### 在Portfolio优化器中找到组合的对齐分数  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. 转到 **项目** 的双曲正切值。
1. 选择 **Portfolio** 选项卡。
1. 单击Portfolio的名称。
1. 选择 **Portfolio优化** 选项卡。
1. 在Portfolio优化程序顶部，找到 **对齐** 值，以及 **对齐方式** 指示组合对齐分数的量规。

   这是组合的对齐分数。

   有关如何生成组合的对齐分数的更多信息，请参阅 [为组合生成对齐分数](#generate-an-alignment-score-for-a-portfolio).

## Portfolio优化程序得分概述

项目的对齐分数与项目组合优化程序分数之间存在差异。

项目的对齐分数是根据完成记分卡后获得的点数计算的。 然后，使用此分数确定组合对齐分数。 对齐分数以百分比显示。

项目的对齐分数显示在 **对齐方式** 列的Portfolio优化程序。

组合优化程序得分是在Portfolio优化程序中自动计算的排名，项目可以按其优先级排列。 组合优化程序得分显示为一个指示器图标，并附有一个数字，它显示在 **得分** 列的Portfolio优化程序。 只有在“业务案例”的所有部分（“目标”除外）都完成后，才会生成Portfolio优化程序分数。

有关为项目创建业务案例的详细信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

有关计算项目的组合优化程序分数的更多信息，请参阅 [Portfolio优化程序得分概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
