---
navigation-topic: business-case-and-scorecards
title: 使用方案规划器的业务案例中的预算资源
description: 作为资源计划的一部分，您可以在构建业务案例时使用Adobe Workfront Scenario Planner来预算完成项目中的工作所需的工作角色。
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# 使用方案规划器的业务案例中的预算资源

作为资源计划的一部分，您可以在构建业务案例时使用Adobe Workfront Scenario Planner来预算完成项目中的工作所需的工作角色。

有关创建业务案例的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

>[!TIP]
>
>当您发布计划时，链接至您在系统层方案规划器中输入的项目的计划的工作角色信息将显示在项目业务案例的资源预算区域中。 Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。

您还可以使用资源规划程序在业务案例中预算资源。 有关更多信息，请参阅以下内容：

* 业务案例中的[预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>我们建议您在开始处理项目时决定使用资源规划者还是场景规划者。 在项目周期内经常在这两个资源之间切换可能会导致项目资源预算不一致。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront Scenario Planner购买附加许可证，才能访问本文中描述的功能。</p> <p>有关获取Workfront Scenario Planner的信息，请参阅<a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">使用Scenario Planner所需的访问权限</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对以下内容的访问权限： </p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>财务数据</p> </li> 
     <li> <p>场景计划器 </p> </li> 
    </ul> <p>有关预算资源所需的访问权限的信息，另请参阅<a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">在Adobe Workfront中预算资源所需的访问权限</a>。</p> <p>注意：如果您仍然没有访问权限，请咨询Adobe Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

在开始之前，必须执行以下操作：

* 使用Scenario Planner创建计划。

  有关信息，请参阅[在Scenario Planner](../../../scenario-planner/create-and-edit-plans.md)中创建和编辑计划。

* 在计划上创建计划并将其链接到项目。

  确保您指明计划所需的工作角色信息，并用此信息更新链接的项目。

  有关更多信息，请参阅以下文章：

   * [在Scenario Planner中创建和编辑计划](../../../scenario-planner/create-and-edit-initiatives.md)
   * [将项目导入方案规划程序中的计划](../../../scenario-planner/import-projects-to-plans.md)
   * [通过发布方案规划器](../../../scenario-planner/publish-scenarios-update-projects.md)中的计划来更新或创建项目。

* 虽然这些不是先决条件，但我们仍建议执行以下操作：

   * 将项目上的任务分配给Scenario Planner中预算的工作角色。
   * 指示项目上任务的计划小时数。

     这有助于您了解一项任务可能需要完成的工作量，这有助于您决定应该为资源预算多长时间来完成该任务。

     有关将任务与计划小时数关联的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 使用场景规划器为链接到计划的项目编制业务案例中的预算资源

>[!IMPORTANT]
>
>您可以按15年的周期预算您的资源。 如果您为工期超过15年的项目预算资源，预算信息可能不准确。
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. 转到要为其预算资源的项目。

   >[!TIP]
   >
   >这是一个链接到Scenario Planner中某个计划的项目，其链接的计划已发布至少一次。

1. 单击左侧面板中的&#x200B;**业务案例**。
1. （视情况而定）在&#x200B;**资源预算**&#x200B;部分中，执行以下操作之一：

   * 如果您刚刚从Scenario Planner发布信息，请在&#x200B;**中选择方案计划器。选择用于计算项目预算劳力成本的小时**&#x200B;字段（位于资源预算区域），然后单击&#x200B;**选择**。

     ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * 如果之前已为该项目的预算资源选择了资源规划者，请单击&#x200B;**更改** > **方案规划者** > **选择**。

     ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront使用链接计划中的所需工作角色小时数计算项目的预算劳力成本和预算小时数。 这是推荐的选项。 成本以项目的货币显示在业务案例中。

     在复制项目并选择将预算小时数复制到新项目时，使用方案规划器的预算小时数未复制到新项目。 仅复制资源规划者中预算的小时数。 有关详细信息，请参阅[复制项目](../manage-projects/copy-project.md)。

     >[!IMPORTANT]
     >
     >当您使用Scenario Planner为项目预算资源时，预算劳力成本显示在Workfront的以下区域中：
     >
     >   
     >   
     >   * 业务案例的资源预算区域
     >   * 系统层“方案计划器”作为链接至项目的方案的“人员成本”。 有关详细信息，请参阅[在Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。
     >   
     >

1. （可选）单击&#x200B;**在Scenario Planner中查看**&#x200B;以打开包含链接到项目的计划的计划。 这将在新的浏览器选项卡中打开Scenario Planner。
1. （可选）更新有关计划的信息。 有关详细信息，请参阅[在Scenario Planner](../../../scenario-planner/create-and-edit-initiatives.md)中创建和编辑计划。

   >[!NOTE]
   >
   >每次对项目上的资源预算区域进行更改后，您必须发布计划才能进行更新。
