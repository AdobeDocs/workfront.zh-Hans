---
navigation-topic: business-case-and-scorecards
title: 使用资源规划程序在业务案例中预算资源
description: 作为资源计划的一部分，您可以在构建业务案例时，使用项目层资源规划者来预算完成项目中的工作所需的职位角色。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1240'
ht-degree: 0%

---

# 使用资源规划程序在业务案例中预算资源

<!--Audited: 06/2025-->

作为资源计划的一部分，您可以在构建业务案例时，使用项目层资源规划者来预算完成项目中的工作所需的职位角色。

有关创建业务案例的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

>[!TIP]
>
>您在项目层资源计划员中输入的信息也可在系统层资源计划员中看到。 反之亦然。 有关资源规划者的信息，请参阅[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

您还可以使用Adobe Workfront Scenario Planner在业务案例中预算资源。 有关详细信息，请参阅使用场景规划器](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)的业务案例中的[预算资源。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> <p>当前：Prime或更高版本</p>
   <p>旧版：专业版或更高版本</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> <p>当前：浅色或更高</p>
   <p>旧版：审阅或更高版本</p>

<p><b>重要信息：</b></p> 
   <p>当前：您必须拥有标准许可证才能修改资源预算信息。 </p> 
   <p>旧版：您必须拥有计划许可证才能修改资源预算信息。 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>编辑对以下内容的访问权限： </p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>资源管理</p> </li> 
     <li> <p>财务数据</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，必须执行以下操作：

* 满足Adobe Workfront中资源规划的所有先决条件。 有关信息，请参阅[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 将资源池与项目关联。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

  >[!NOTE]
  >
  >您不能预算分配给业务案例中的问题的资源。 您可以在系统级资源规划程序中为其编制预算。 有关资源规划者的详细信息，请参阅[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

* 虽然这并非先决条件，但我们仍建议您为项目中的任务指明已计划小时数。 这有助于您了解一项任务可能需要完成的工作量，这有助于您决定资源应该为完成该任务投入多少时间。 有关将任务与计划小时数关联的信息，请参阅[编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md)。

## 在业务案例中将资源池应用到项目和预算资源

>[!IMPORTANT]
>
>您可以按15年的周期预算您的资源。 如果您为工期超过15年的项目预算资源，预算信息可能不准确。

要在业务案例中为没有资源池的项目应用资源池和预算项目资源，请执行以下操作：

1. 转到要为其预算资源的项目。
1. 单击左侧面板中的&#x200B;**业务案例**。
1. （视情况而定）如果您的公司没有Workfront Scenario Planner的许可证，请单击&#x200B;**资源预算**&#x200B;部分中的&#x200B;**编辑资源预算**，然后继续执行步骤5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （可选且视情况而定）如果项目信息是通过Scenario Planner上的计划发布的，请执行以下操作之一：

   * 在&#x200B;**中选择资源规划者选择要用于计算项目预算劳力成本的小时数**&#x200B;字段，然后单击&#x200B;**选择>编辑资源预算**。

     资源规划者中的![业务案例](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 如果为项目选择了方案规划者来预算资源，请单击&#x200B;**更改** > **编辑资源预算**。

     Scenario Planner中的![业务案例](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)

   它使用项目的预算小时数来计算项目的预算劳力成本。

   Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅[Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md)。

   >[!NOTE]
   >
   >我们建议您在开始处理项目时决定使用资源规划者还是场景规划者。 在项目周期内经常在这两个资源之间切换可能会导致项目资源预算不一致。

1. 在&#x200B;**选择资源池**&#x200B;字段中，指定一个或多个&#x200B;**资源池**。

   您必须仅指定使用活动用户填充的资源池。

   >[!TIP]
   >
   >如果项目已与资源池关联，则默认情况下将显示资源规划者。 要向项目添加更多资源池，请编辑项目。 有关编辑项目的信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. 单击&#x200B;**应用**。

   此时将显示选定项目的资源规划者。

   默认情况下，与此项目关联的前20个工作角色按字母顺序列在“资源预算编制”部分。 

   有关资源规划者的详细信息，请参阅[资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （可选和条件）展开工作角色以查看与其关联的用户。

   >[!NOTE]
   >
   >仅当活动用户满足以下条件时，活动用户才会显示在与其关联的工作角色下：
   >
   >   
   >   
   >   * 它们属于项目的某个资源池。
   >   * 他们已分配预算小时数。
   >   * 它们与项目的某个工作角色关联。
   >   
   >

    

1. 单击&#x200B;**今天**&#x200B;返回今天的时间范围。
1. （可选）单击&#x200B;**周**、**月**&#x200B;或&#x200B;**季度**&#x200B;以显示不同时间范围内的项目信息。
1. （可选）单击&#x200B;**小时**&#x200B;下拉菜单，然后选择&#x200B;**小时**、**FTE**&#x200B;或&#x200B;**成本**&#x200B;以更改信息在资源规划者中的显示方式。 默认情况下显示小时数。

1. （可选）单击&#x200B;**导出**&#x200B;以将资源规划者导出到Excel文件。

   >[!NOTE]
   >
   >一次最多可以导出12个时间段的数据。

1. （可选）单击&#x200B;**全屏**&#x200B;图标![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png)以全屏模式显示“资源规划者”。

1. 通过执行以下操作之一，使用用户、角色或项目的小时、FTE或成本值更新&#x200B;**BDG**（预算小时数）字段：

   * 手动估算角色、用户或项目的小时数、FTE或成本值。

     或

   * 单击项目或工作角色的&#x200B;**选项**&#x200B;图标，然后选择用于自动为角色、用户或项目预算小时数的选项。

   有关资源规划者的“项目”视图中的预算的更多信息，请参阅“使用项目和角色”视图的资源规划者中的[预算资源](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)。

   >[!NOTE]
   >
   >您可以在“资源预算”区域中显示的任何时间范围内为资源预算小时数、FTE或成本，这与项目的时间表无关。 例如，如果您想指出您的资源在项目时间线中可能不可用（这些资源与计划小时数关联），但在其他时间可能可用，则可以通过为计划小时数为零的时间范围编列预算来实现此目的，前提是这些资源在计划小时数变为可用时可用。

1. （可选）要了解您是否可以将预算小时数、FTE或成本移动到另一个时间范围，请单击&#x200B;**选项**&#x200B;图标，然后单击&#x200B;**调整预算日期**。

   有关调整预算日期的详细信息，请参阅[在资源规划者中调整预算日期](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md)。

1. 单击&#x200B;**保存**。

   如果您有与工作角色关联的每小时成本费率，则对资源预算区域中的资源进行预算可计算项目的&#x200B;**预算劳力成本**。 预算劳力成本显示在业务案例的资源预算区域和业务案例摘要中。

   >[!TIP]
   >
   >成本以项目的货币显示在业务案例中。

   在业务案例中指定的预算信息也会显示在资源规划者中。

   在复制项目时，您还可以选择将预算小时数复制到新项目。 仅复制资源规划者中预算的小时数。 有关详细信息，请参阅[复制项目](../manage-projects/copy-project.md)。
