---
navigation-topic: business-case-and-scorecards
title: 使用资源计划员在业务案例中预算资源
description: 在资源计划中，您可以使用项目层资源计划员来预算在构建业务案例时完成项目中的工作所需的任务职责。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# 使用资源计划员在业务案例中预算资源

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

在资源计划中，您可以使用项目层资源计划员来预算在构建业务案例时完成项目中的工作所需的任务职责。

有关创建业务案例的更多信息，请参阅 [为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>在项目层资源计划器中输入的信息也在系统层资源计划器中可见。 相反，情况也是如此。 有关资源计划员的信息，请参阅 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

您还可以使用Adobe Workfront方案计划员对业务案例中的资源进行预算。 有关更多信息，请参阅 [使用方案计划员在业务案例中预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审阅或更高版本</p> <p>重要信息：您必须拥有计划许可证才能修改资源预算信息。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对以下项的访问权限： </p> 
    <ul> 
     <li> <p>项目</p> </li> 
     <li> <p>资源管理</p> </li> 
     <li> <p>财务数据</p> </li> 
    </ul> <p>有关预算资源所需访问权限的信息，另请参阅 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">在Adobe Workfront获得预算资源所需的资源</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询Adobe Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须执行以下操作：

* 在Adobe Workfront中满足资源规划的所有先决条件。 有关信息，请参阅 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 将资源池与项目关联。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   您不能对分配给业务案例中的问题的资源进行预算。 您可以在系统层资源计划员中对它们进行预算。 有关资源计划员的详细信息，请参阅 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* 虽然这不是先决条件，但我们还建议您为项目中的任务指定计划小时数。 这有助于您了解任务可能需要完成的工作量，这有助于您决定为完成该任务而在预算中花费的资源时间。 有关将任务与计划小时数关联的信息，请参阅 [编辑任务](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## 在业务案例中将资源池应用于项目和预算资源

>[!IMPORTANT]
您可以将资源预算为15年。 如果您对持续时间超过15年的项目的资源进行预算，则预算信息可能不准确。

要在业务案例中为没有资源池的项目应用资源池和预算项目资源，请执行以下操作：

1. 转到要对资源进行预算的项目。
1. 单击 **商业案例** 中。
1. （视情况而定）如果您的公司没有Workfront方案计划员的许可证，请单击 **编辑资源预算** 在 **资源预算编制** ，然后继续执行步骤5。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （可选和视情况而定）如果项目信息是从方案计划员的方案发布的，请执行以下操作之一：

   * 在 **选择用于计算项目预算人工成本的小时数** 字段，然后单击 **选择>编辑资源预算**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * 如果为项目的预算资源选择了方案计划员，请单击 **更改** > **编辑资源预算**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   它使用项目的预算小时数来计算项目的预算人工成本。

   方案规划器仅在新的Adobe Workfront体验中可用，并且需要额外的许可证。 有关Workfront方案规划器的信息，请参阅 [方案计划员概述](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   我们建议您在开始处理项目时决定是使用资源计划员还是方案计划员。 在项目生命周期中经常在两个资源之间切换可能会导致项目资源预算方式不一致。

1. 在 **选择资源池** 字段，指定一个或多个 **资源池**.

   您只能指定使用活动用户填充的资源池。

   >[!TIP]
   如果项目已与资源池关联，则默认情况下会显示资源计划器。 要向项目添加更多资源池，请编辑项目。 有关编辑项目的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 单击 **应用**.

   此时将显示选定项目的资源计划员。

   默认情况下，与此项目关联的前20个作业角色按字母顺序列在“资源预算”部分中。 

   有关资源计划员的详细信息，请参阅 [资源计划员概述](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （可选和视情况而定）展开作业角色以查看与其关联的用户。

   >[!NOTE]
   活动用户只有在满足以下条件时才会显示在与其关联的作业角色下：
   * 它们属于项目的一个资源池。
   * 他们已分配预算小时数。
   * 它们与项目的一个作业角色相关联。


    

1. 单击 **今天** 回到今天的时间范围。
1. （可选）单击 **周**, **月** 或 **季度** 以显示不同时间范围内项目的信息。
1. （可选）单击 **小时** 下拉菜单，然后选择 **小时**,**FTE**&#x200B;或 **成本** 更改资源计划员中信息显示方式。 默认显示小时数。

1. （可选）单击 **导出** 将资源计划器导出为Excel文件。

   >[!NOTE]
   一次最多可导出12个时间段的数据。

1. （可选）单击 **全屏** 图标 ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) 以全屏模式显示资源计划员。

1. 更新 **BDG** （预算小时数）字段，其中包含用户、角色或项目的“小时”、“FTE”或“成本”值，方法是执行以下操作之一：

   * 手动估计角色、用户或项目的“小时”、“FTE”或“成本”值的金额。

      或

   * 单击 **选项** 图标，然后选择一个选项以自动为角色、用户或项目预算小时数。
   有关资源计划员的“项目视图”中预算的详细信息，请参阅 [使用“项目”和“职责”视图在资源计划员中预算资源](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   您可以为资源在“资源预算”区域中显示的任何时间范围预算小时数、FTE或成本，而与项目的时间表无关。 例如，如果您想要指明资源可能在项目时间轴期间不可用（在该时间轴中，资源与计划时间关联），但可能在另一时间可用，则可以通过将资源预算到计划时间为零的时间范围（如果计划时间为零，则当资源可用时）来执行此操作。

1. （可选）要了解是否可以将预算的工时、FTE或成本移到其他时间范围，请单击 **选项** 图标，然后 **调整预算日期**.

   有关调整预算日期的详细信息，请参阅 [在资源计划器中调整预算日期](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. 单击&#x200B;**保存**。

   如果您具有与任务职责关联的“每小时成本”费率，则对“资源预算”区域中的资源进行预算会计算 **预算人工成本** 的项目。 预算的人工成本显示在“业务案例”和“业务案例汇总”的“资源预算”区域中。

   >[!TIP]
   成本以项目的币种显示在业务案例中。

   在“业务案例”中指定的预算信息也会显示在资源计划器中。

   <!--drafted for Budgeted Hours: 
   <span class="preview">When you copy a project, you have the option to also copy the Budgeted Hours to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md)</span>
   -->
