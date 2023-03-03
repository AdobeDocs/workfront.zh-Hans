---
navigation-topic: business-case-and-scorecards
title: 使用资源规划程序在业务案例中预算资源
description: 作为资源计划的一部分，您可以在构建业务案例时，使用项目层资源规划者来预算完成项目中的工作所需的工作角色。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# 使用资源规划程序在业务案例中预算资源

作为资源计划的一部分，您可以在构建业务案例时，使用项目层资源规划者来预算完成项目中的工作所需的工作角色。

有关创建业务案例的更多信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>您在项目层资源计划员中输入的信息也可在系统层资源计划员中看到。 反之亦然。 有关资源规划者的信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

您还可以使用Adobe Workfront Scenario Planner在业务案例中预算资源。 有关更多信息，请参阅 [使用方案规划器的业务案例中的预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>专业或专业以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审核或更高</p> <p>重要信息：您必须拥有计划许可证才能修改资源预算信息。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对以下内容的访问权限： </p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>资源管理</p> </li> 
     <li> <p>财务数据</p> </li> 
    </ul> <p>有关预算资源所需访问权限的信息，另请参阅 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">在Adobe Workfront中预算资源所需的访问权限</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询Adobe Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须执行以下操作：

* 满足Adobe Workfront中资源规划的所有先决条件。 有关信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 将资源池与项目关联。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   您不能预算分配给业务案例中的问题的资源。 您可以在系统层资源规划程序中为其编制预算。 有关资源规划者的详细信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 虽然这并非先决条件，但我们仍建议您为项目中的任务指明已计划小时数。 这有助于您了解任务可能需要完成的工作量，这有助于您确定完成任务应该为资源预算多少时间。 有关将任务与计划小时数关联的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 在业务案例中将资源池应用于项目和预算资源

>[!IMPORTANT]
您可以将资源预算为15年。 如果您为工期超过15年的项目预算资源，预算信息可能不准确。

要在业务案例中为没有资源池的项目应用资源池和预算项目资源，请执行以下操作：

1. 转到要为其预算资源的项目。
1. 单击 **商业论证** （在左侧面板中）。
1. （视情况而定）如果您的公司没有Workfront Scenario Planner的许可证，请单击 **编辑资源预算** 在 **资源预算** 部分，然后继续执行步骤5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （可选且有条件）如果项目信息是从场景规划器上的某个计划发布的，请执行以下操作之一：

   * 选择资源规划者 **选择用于计算项目预算劳力成本的小时数** 字段，然后单击 **选择>编辑资源预算**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 如果已为项目的预算资源选择Scenario Planner，请单击 **更改** > **编辑资源预算**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   这会使用项目的预算小时数来计算项目的预算劳力成本。

   Scenario Planner仅在新的Adobe Workfront Experience中可用，并且需要额外的许可证。 有关Workfront Scenario Planner的信息，请参阅 [Scenario Planner概述](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   我们建议您在开始处理项目时决定使用资源规划者还是场景规划者。 在项目生命周期中经常在这两个之间切换可能会导致项目资源预算方式不一致。

1. 在 **选择资源池** 字段，指定一个或多个 **资源池**.

   您只能指定使用活动用户填充的资源池。

   >[!TIP]
   如果项目已与资源池关联，则默认情况下将显示资源规划者。 要向项目添加更多资源池，请编辑项目。 有关编辑项目的信息，请参见 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 单击 **应用**.

   此时将显示选定项目的资源规划者。

   默认情况下，与此项目关联的前20个工作角色在资源预算部分中按字母顺序列出。 

   有关资源规划者的详细信息，请参阅 [资源规划者概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （可选和条件）展开工作角色以查看与其关联的用户。

   >[!NOTE]
   仅当活动用户满足以下条件时，活动用户才会显示在与其关联的工作角色下：
   * 它们属于项目的某个资源池。
   * 他们已分配预算小时数。
   * 它们与项目的某个工作角色相关联。


    

1. 单击 **今天** 返回到今天的时间范围。
1. （可选）单击 **周**， **月** 或 **季度** 以在不同时间范围内显示项目的信息。
1. （可选）单击 **小时** 下拉菜单，然后选择 **小时**，**FTE**，或 **成本** 以更改信息在“资源规划者”中的显示方式。 默认情况下显示小时数。

1. （可选）单击 **导出** 将资源规划者导出到Excel文件。

   >[!NOTE]
   一次最多可导出12个时间段的数据。

1. （可选）单击 **全屏** 图标 ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) 以全屏模式显示资源规划者。

1. 更新 **BDG** （预算小时数）字段，其中显示用户、角色或项目的小时数、FTE值或成本值，方法是执行以下操作之一：

   * 手动估算角色、用户或项目的小时数、FTE或成本值。

      或

   * 单击 **选项** 图标，然后选择用于自动为角色、用户或项目预算小时数的选项。
   有关资源规划者的“项目视图”中预算编制的详细信息，请参阅 [使用“项目”和“角色”视图在资源规划者中预算资源](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   您可以为“资源预算”区域中显示的任何时间范围预算资源的小时、FTE或成本，而不依赖于项目的时间表。 例如，如果您要指示资源在项目时间线中可能不可用（这些资源与计划小时数相关联），但在其他时间可能可用，则可以通过为计划小时数为零的时间范围为这些资源编列预算来实现此目的，前提是这些资源在那时可以工作。

1. （可选）要了解是否可以将预算小时数、FTE或成本移动到另一个时间范围，请单击 **选项** 图标，然后 **调整预算日期**.

   有关调整预算日期的详细信息，请参阅 [在资源规划程序中调整预算日期](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. 单击&#x200B;**保存**。

   如果您拥有与工作角色关联的每小时成本费率，则对“资源预算”区域中的资源进行预算将计算 **预算劳力成本** 项目的URL。 预算劳力成本显示在业务案例的资源预算区域和业务案例摘要中。

   >[!TIP]
   成本以项目的币种显示在业务案例中。

   在业务案例中指定的预算信息也会显示在资源规划程序中。

   在复制项目时，您还可以选择将预算小时数复制到新项目。 仅复制资源规划者中预算的小时数。 有关更多信息，请参阅 [复制项目](../manage-projects/copy-project.md).
