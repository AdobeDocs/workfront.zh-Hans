---
content-type: reference
product-area: projects
navigation-topic: financials
title: 了解项目的预算人工成本和预算工时
description: 了解项目的预算人工成本和预算工时
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# 了解项目的预算人工成本和预算工时

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

您可以使用Adobe Workfront资源计划器对资源进行预算以用于工作。

在对资源进行项目预算时，Workfront会根据每小时成本值计算角色、项目和用户的预算人工成本。

项目的“资源计划员预算人工成本”是与分配用于完成项目工作的任务职责关联的成本与可能承担每个职责以完成工作的估计小时数（资源计划员预算小时数）之间的计算。

>[!IMPORTANT]
>
>用户的资源计划员预算人工成本不会影响项目的人工成本。 只有职务职责的人工成本会影响项目的成本。

## 职务职责预算人工成本及项目概述

Workfront使用项目中职务职责的预算人工成本来计算项目的预算人工成本。

>[!TIP]
>
>“业务案例”中项目的预算人工成本在报表和列表中显示为“资源计划员预算人工成本”。

的 **预算人工成本** （或资源计划员预算人工成本）按以下公式计算：

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上述计算中使用的字段涉及以下内容：

* 在项目或资源计划员的“资源预算”区域中为职务职责编入预算的小时数。

   有关资源计划员中预算资源的详细信息，请参阅文章中的“资源计划员中的预算资源”部分 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   有关“业务案例”的“资源预算”区域中预算资源的详细信息，请参阅 [业务案例中的预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* 的 **职务角色的每小时成本率** 在上述计算中，是指与项目上每个任务职责关联的成本。\
   有关创建和管理任务职责并将其与成本费率关联的详细信息，请参阅文章 [创建和管理作业角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront使用项目的货币计算所有成本信息。 如果在资源计划器中为资源指定预算小时数，则更改项目币种的选项将被禁用。\
>有关更改项目货币的更多信息，请参阅文章 [更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md).

## 用户预算人工成本概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>用户预算的人工成本不会影响项目的预算人工成本。 只有项目中任务职责的人工成本会影响项目的资源计划员预算人工成本。
> 
>所有用户的所有人工成本总数可能等于或不等于与用户关联的任务职责的资源计划员预算人工成本。
>
>如果您在资源计划员中估计用户的预算小时数，则与这些用户关联的成本是与用户关联的职务职责的成本。 它们不是与用户或其费率相关的成本。

如果用户与项目中的职务职责相关联，并且其工时在资源计划员中进行预算，则其预算的人工成本将按以下名称显示，具体取决于您在Workfront中查看它们的位置：

* [!UICONTROL **预算人工成本**]:业务案例的“资源预算”区域，按其各自的角色进行。

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]:在按成本查看“项目”和“职责”视图中的信息时，资源计划员。

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

用户在业务案例的“资源预算”区域中显示其各自职责，如果满足以下要求，则显示在资源计划员中：

* 它们与项目中的一个作业角色关联。
* 它们在资源计划员中指定了预算小时数。
* 他们具有与其用户档案关联的每小时成本率。

   有关向用户添加每小时成本费率的详细信息，请参阅文章 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 用户是与项目关联的一个资源池的一部分。

用户的预算人工成本按以下公式计算：

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 查找项目的预算人工成本

“业务案例”或“资源计划员”的“资源预算”区域中反映的预算人工成本将以下名称显示在Workfront的以下区域：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>预算人工成本显示名称</strong></td> 
     <td><strong>Workfront地区</strong></td> 
    </tr> 
    <tr> 
     <td>预算劳力成本</td> 
     <td>业务案例的资源预算区域</td> 
    </tr> 
    <tr> 
     <td>预算成本</td> 
     <td><p>利用率报表成本视图</p><p>有关更多信息，请参阅 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看利用率信息</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>按成本列出的资源计划员项目或职责视图</td> 
    </tr> 
    <tr> 
     <td>资源计划员项目预算人工成本</td> 
     <td> <p>项目报告</p> <p>项目（财务数据）报表</p> <p>任务报告</p> <p>问题报告</p> <p>预算小时报表</p> <p>有关创建报表的信息，请参阅文章 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>如果您使用Adobe Workfront方案计划员对项目资源进行预算，则“业务案例”的“资源预算”区域中的“预算人工成本”与与项目关联的方案的“人员成本”相同。 方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md). 有关使用方案计划员编制预算资源的信息，请参阅 [使用方案计划员在业务案例中预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 查找项目的预算小时数

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

预算小时数影响项目的预算人工成本（或资源计划员预算成本）的值。

项目的“预算人工成本”是指与分配给完成项目工作的职务职责相关的成本，以及每个职责完成工作的估计小时数（预算小时数）。

您可以在下表所列的字段中查看Workfront的预算小时数。

>[!NOTE]
>
>在Workfront中提及“已编入预算的小时数”的任何其他提及均指使用已从Workfront中删除的已弃用功能编入预算的小时数。 这些是仅查看字段，在使用当前资源预算工具时，不会使用当前信息进行更新。

在“业务案例”或“资源计划员”的“资源预算”区域预算的小时数显示在Workfront的以下区域，并且名称如下：

* **小时**:业务案例的资源预算区域
* **BDG**：按小时查看的资源计划员
* **预算小时数**:利用率报表小时视图有关信息，请参阅 [查看资源利用信息](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **巴德。 小时**:预算小时报表

   “已编入预算的小时”报表中的“已编入预算的小时”对象是指与已弃用的资源管理工具相关的信息。 只有&quot;巴德&quot; “小时”字段是指在“资源计划员”或项目业务案例的“资源预算”区域中预算的小时数。

   有关创建报表的更多信息，请参阅文章 **创建自定义报表**.
* **资源计划员预算小时数**:在以下报表中：

   * 项目报告
   * 项目（财务数据）报表
   * 任务报告
   * 问题报告
   * 预算小时报表
