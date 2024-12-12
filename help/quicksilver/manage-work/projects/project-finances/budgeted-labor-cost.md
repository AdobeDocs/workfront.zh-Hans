---
content-type: reference
product-area: projects
navigation-topic: financials
title: 了解项目的预算劳力成本和预算小时数
description: 了解项目的预算劳力成本和预算小时数
author: Lisa
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# 了解项目的预算劳力成本和预算小时数

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

您可以使用Adobe Workfront资源规划者为工作预算资源。

在为项目工作预算资源时，Workfront会根据每小时成本值计算角色、项目和用户的预算劳力成本。

项目的资源规划者预算劳力成本是与分配用于完成项目工作的工作角色关联的成本，与完成工作可能需要每个角色的估计小时数（资源规划者预算小时数）之间的计算。

>[!IMPORTANT]
>
>用户的资源规划者预算劳力成本不会影响项目的成本。 只有工作角色的劳力成本会影响项目成本。

## 工作角色和项目的预算劳力成本概览

Workfront使用项目上工作角色的预算劳力成本计算项目的预算劳力成本。

>[!TIP]
>
>业务案例中项目的预算劳力成本在报告和列表中显示为资源规划者预算劳力成本。

按照以下公式计算项目的&#x200B;**预算劳力成本**（或资源规划者预算劳力成本）：

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上述计算中使用的字段参考以下内容：

* 项目或资源规划者资源预算区域中工作角色的预算小时数。

  有关资源规划者中预算资源的详细信息，请参阅文章[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的“资源规划者中的预算资源”部分。

  有关业务案例的资源预算编制区域中的预算资源的详细信息，请参阅业务案例中的[预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

* 在上述计算中，工作角色&#x200B;**的**&#x200B;每小时成本费率是指与项目中的每个工作角色关联的成本。\
  有关创建和管理工作角色并将其与成本费率关联的更多信息，请参阅文章[创建和管理工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

>[!NOTE]
>
>Workfront使用项目的货币计算所有成本信息。 如果您在资源规划者中为资源指定预算小时数，则将禁用更改项目币种的选项。\
>有关更改项目货币的详细信息，请参阅文章[更改项目货币](../../../manage-work/projects/project-finances/change-project-currency.md)。

## 用户的预算劳力成本概览

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>用户预算劳力成本不会影响项目的预算劳力成本。 只有项目上工作角色的劳力成本会影响项目的资源规划者预算劳力成本。
> 
>所有用户的所有劳力成本的总和可能等于或不等于与用户关联的工作角色的资源规划者预算劳力成本。
>
>如果您估计资源规划者中用户的预算小时数，则与这些用户关联的成本是与用户关联的工作角色的成本。 它们不是与用户或其费率相关的成本。

如果用户与项目中的工作角色相关联，并且其小时数在资源规划者中进行了预算，则其预算劳力成本按以下名称显示，具体取决于您在Workfront中查看它们的位置：

* [!UICONTROL **预算劳力成本**]：业务案例的资源预算区域，位于其各自的角色下。

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]：资源规划者，在按成本查看“项目”和“角色”视图中的信息时。

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

如果用户满足以下要求，则显示在业务案例的“资源预算”区域中其各自的角色下，或者显示在资源规划者中：

* 它们与项目中的某个工作角色关联。
* 他们在资源规划者中指定了预算小时数。
* 他们有与其配置文件关联的每小时成本费率。

  有关向用户添加每小时成本费率的详细信息，请参阅文章[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

* 用户属于与项目关联的某个资源池。

用户的预算劳力成本按以下公式计算：

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## 查找项目的预算劳力成本

业务案例或资源规划者的资源预算区域中反映的预算劳力成本显示在Workfront的以下区域中，名称如下：

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>预算劳力成本显示名称</strong></td> 
     <td><strong>Workfront区域</strong></td> 
    </tr> 
    <tr> 
     <td>预算劳动力成本</td> 
     <td>业务案例的资源预算区域</td> 
    </tr> 
    <tr> 
     <td>预算成本</td> 
     <td><p>利用率报表成本视图</p><p>有关详细信息，请参阅<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">查看利用率信息</a> 。</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>资源规划者项目或角色视图，按成本</td> 
    </tr> 
    <tr> 
     <td>资源规划者项目预算劳力成本</td> 
     <td> <p>项目报告</p> <p>项目（财务数据）报表</p> <p>任务报告</p> <p>问题报告</p> <p>预算小时数报告</p> <p>有关创建报告的信息，请参阅文章<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报告</a>。</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>如果您使用Adobe Workfront方案规划程序来预算项目资源，则业务案例的资源预算区域中的预算人工成本与链接至项目的方案的人员成本相同。 Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。 有关使用Scenario Planner预算资源的信息，请参阅[使用Scenario Planner的业务案例中的预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)。

## 查找项目的预算小时数

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

预算小时数影响项目的预算劳力成本（或资源规划者预算成本）的值。

项目的预算劳力成本是与分配给完成项目工作的工作角色关联的成本，以及每个角色完成工作所需的估计小时数（预算小时数）。

您可以在下表列出的字段中查看Workfront中的预算小时数。

>[!NOTE]
>
>Workfront中对“预算小时数”的任何其他提及均指使用已从Workfront中删除的已弃用功能进行预算的小时数。 这些是仅供查看的字段，在使用当前资源预算编制工具时，不会更新为最新信息。

在业务案例或资源规划者的资源预算区域中进行预算的小时数显示在Workfront的以下区域和以下名称下：

* **小时**：业务案例的资源预算区域
* **BDG**：按小时查看的资源规划者
* **预算小时数**：使用情况报告小时数视图
有关信息，请参阅[查看资源利用率信息](../../../resource-mgmt/resource-utilization/view-utilization-information.md)。
* **预算。 小时数**：预算小时数报告

  预算小时数报表中的预算小时数对象引用与已弃用资源管理工具相关的信息。 只有“巴德” “小时”字段是指在资源规划者或项目业务案例的资源预算区域中进行预算的小时。

  有关创建报告的详细信息，请参阅文章&#x200B;**创建自定义报告**。
* **资源规划者预算小时数**：在以下报表中：

   * 项目报告
   * 项目（财务数据）报表
   * 任务报告
   * 问题报告
   * 预算小时数报告
