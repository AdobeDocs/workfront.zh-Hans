---
navigation-topic: business-case-and-scorecards
title: 将记分卡应用于项目并生成一致性分数
description: 您可以使用记分卡衡量项目与项目组合中先前建立的标准的符合程度。 记分卡通常反映了组织的使命、价值观和战略目标。
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# 将记分卡应用于项目并生成一致性分数

您可以使用记分卡衡量项目与项目组合中先前建立的标准的符合程度。 记分卡通常反映了组织的使命、价值观和战略目标。

有关记分卡以及如何创建记分卡的更多信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>查看或更高权限的Portfolio</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>查看项目组合或更高权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 项目记分卡 {#project-scorecards}

* [记分卡概述](#scorecards-overview)
* [项目记分卡](#project-scorecards)

### 记分卡概述 {#scorecards-overview}

通常，项目经理会完成记分卡信息，以便为项目生成介于0和100之间的对齐值。 项目组合经理稍后在项目组合优化器中查看项目以比较它们时，将使用生成的值。

有关组合优化的更多信息，请参阅文章 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### 将记分卡应用于项目

作为拥有项目的“计划”许可证和“管理”权限的用户，您可以将记分卡附加到项目。

有关项目权限的更多信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

您可以在构建项目的业务案例过程中向项目添加记分卡。

有关构建业务案例的更多信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

您的Adobe Workfront管理员或组管理员必须在项目的业务案例区域中启用“记分卡”部分，然后才能从业务案例访问记分卡。 有关设置项目首选项和启用Business Case区域的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

要将记分卡应用于项目，请执行以下操作：

1. 转到要应用记分卡的项目。
1. 单击 **商业论证** （在左侧面板中）。
1. 查找 **记分卡** 商业论证部分。\
   您必须先创建记分卡，然后再创建 **记分卡** 部分显示在业务案例中。

   有关创建记分卡的信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. 从下拉菜单中选择一个记分卡。

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. 为记分卡中的所有问题指定一个答案。

   Workfront将分数应用于每个已回答的问题，并根据每个问题的单独分数计算项目整体分数。

   有关生成项目总体一致性分数的更多信息，请参阅 [为项目生成对齐分数](#generate-an-alignment-score-for-a-project).

1. 单击 **保存** 以保存记分卡并对项目评分。

   记分卡现在与项目关联，并对项目进行评分。

1. （视情况而定）当记分卡问题的值发生更改时，必须重新计算记分卡以反映项目得分的新值。 要重新计算记分卡，请执行以下操作：

   1. 转到项目列表，然后选择列表中的所有项目。
   1. 单击 **编辑** 图标。
   1. 单击 **设置** 然后，在左侧面板中 **重新计算记分卡** 选项。
   1. 单击保存。这会根据为所有选定项目附加的记分卡重新计算得分值。

      >[!NOTE]
      >
      >   <span class="preview">批量编辑项目时，已从“预览”环境中删除了重新计算记分卡的选项。 </span>


## 生成对齐分数

* [为项目生成对齐分数](#generate-an-alignment-score-for-a-project)
* [为项目组合生成对齐分数](#generate-an-alignment-score-for-a-portfolio)

### 为项目生成对齐分数 {#generate-an-alignment-score-for-a-project}

一致性分数是完成记分卡后生成的值。

记分卡包含问题，这些问题具有已分配数值的答案选择，称为对齐点。 这些要点用于确定项目与您的组织的协调程度。 每个问题的对齐点包含一个介于0和100之间的数字。

完成记分卡后，Workfront会使用以下公式以百分比计算项目的对齐分数：

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

有关更多信息，请参阅 [创建记分卡](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### 为项目组合生成对齐分数 {#generate-an-alignment-score-for-a-portfolio}

项目组合的一致性分数是项目组合中所有项目的平均一致性分数。

完成项目的记分卡后，Workfront会使用这些值通过下列公式以百分比形式计算项目组合的对齐分数：

Portfolio一致性分数=项目一致性分数的百分比总和/项目组合中的项目数

>[!NOTE]
>
>如果项目没有与其关联的记分卡，因此没有一致性分数，则它被视为项目组合中的一致性为0%。 在项目组合的项目数中考虑该项目。

## 查看一致性分数

您可以在项目级别或Portfolio优化器中查看项目的对齐分数。

* [查看项目中的一致性分数](#View%20the)
* [在Portfolio优化器中查看项目和项目组合的对齐分数](#View%20the2)

### 查看项目中的一致性分数

如果您拥有项目的“参与”权限，则可以在项目级别查看项目的对齐分数。

1. 转到要查看其一致性分数的项目。
1. 单击 **商业论证** （在左侧面板中）。
1. 转到 **商业论证摘要** 屏幕右侧。

   一致性得分位于业务案例摘要中，位于 **已对齐** 值。

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### 在Portfolio优化器中查看项目和项目组合的对齐分数

如果您拥有项目组合的管理访问权限，则可以在Portfolio优化器中查看项目或项目组合的对齐分数。

有关Portfolio优化器中显示信息的详细信息，请参阅 [Portfolio优化器概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [在Portfolio优化器中找到项目的对齐分数](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [在Portfolio优化器中找到项目组合的对齐分数](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### 在Portfolio优化器中找到项目的对齐分数 {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)，则 **Portfolio**.

1. 单击Portfolio的名称。
1. 单击 **Portfolio优化** （在左侧面板中）。

   此时将显示Portfolio优化器。

1. 项目的对齐分数以百分比形式显示在 **对齐方式** Portfolio优化程序的列。

   这是基于与项目关联的记分卡的项目的对齐分数。

#### 在Portfolio优化器中找到项目组合的对齐分数  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. 转到 **项目** 区域。
1. 选择 **Portfolio** 选项卡。
1. 单击Portfolio的名称。
1. 选择 **Portfolio优化** 选项卡。
1. 在Portfolio优化器的顶部，查找 **已对齐** 值，以及 **对齐方式** 指示组合对齐分数的量规。

   这是项目组合的对齐分数。

   有关如何生成项目组合的对齐分数的更多信息，请参阅 [为项目组合生成对齐分数](#generate-an-alignment-score-for-a-portfolio).

## Portfolio优化器得分概述

项目的对齐分数与项目组合优化器分数之间存在差异。

项目的对齐分数是根据完成记分卡后获得的积分来计算的。 然后，使用此得分确定项目组合对齐方式得分。 对齐分数以百分比显示。

项目的对齐分数显示在 **对齐方式** Portfolio优化程序的列。

项目组合优化器得分是在Portfolio优化器中自动计算的排名，通过它可以对项目进行优先排序。 项目组合优化器得分显示为指示器图标并附有一个数字，该数字显示在 **分数** Portfolio优化程序的列。 仅当完成业务案例的所有部分（目标除外）时，才会生成Portfolio优化程序得分。

有关为项目创建业务案例的更多信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

有关计算项目的项目组合优化器分数的更多信息，请参阅 [Portfolio优化器得分概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
