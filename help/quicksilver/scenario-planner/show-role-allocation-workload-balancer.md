---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在负载平衡器中显示项目和方案的角色分配
description: 在连接项目和方案后，您可以并排管理其资源分配，以确保它们
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 显示 [!DNL Workload Balancer]

>[!IMPORTANT]
>
>贵组织必须为 [!DNL Adobe Workfront Scenario Planner] 以便您查看项目的计划信息。 有关获取 [!DNL Workfront Scenario Planner]，请参阅 [使用所需的访问权限 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

在连接项目和方案后，您可以并排管理其资源分配，以确保它们匹配。 这可避免过度分配或利用这些资源。

本文介绍了如何使用 [!UICONTROL 角色分配] 面板 [!UICONTROL 工作负载平衡器] 项目。

有关在项目和计划之间协调资源（包括先决条件）的一般信息，请参阅 [协调项目和举措之间的资源分配的概述](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 访问要求

您需要遵循以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 计划*</b> </p> </td> 
   <td>[!UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 许可证*</b> </p> </td> 
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为 [!DNL Adobe Workfront Scenario Planner] ，以访问本文中描述的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参阅 <a href="../scenario-planner/access-needed-to-use-sp.md">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[!UICONTROL视图]或更高版本对项目的访问权限 </p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>[!UICONTROL视图]或对项目拥有更高权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Request]对 [!DNL Workfront Scenario Planner]</a>.</p> <p>有关请求对项目进行额外访问的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 显示 [!DNL Workload Balancer]

如果贵公司已购买 [!DNL Workfront Scenario Planner] 许可证，您可以在项目级别协调方案与与其链接的项目之间的资源分配 [!DNL Workload Balancer].

1. （视情况而定）使用以下文章中描述的方法之一，将项目与方案连接起来：

   * [将项目导入 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [通过在 [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >如果对方案上的资源进行更改，则必须重新发布方案所属的方案，以便获取方案中的最新资源信息以更新项目。

1. 转到要复查项目以及关联方案的作业角色分配的项目。
1. 单击 [!DNL Workload Balancer] 中。

   您可能需要单击 **[!UICONTROL 计划]**，则 **[!UICONTROL 切换到工作负载平衡器]**.

1. 执行下列操作之一：

   * 单击 **[!UICONTROL 月]** 要按月查看工作负载平衡器，请单击时间轴中一个月旁边的下拉菜单 ![](assets/drop-down-next-to-month-month-view-wb.png)，然后单击 **[!UICONTROL 更多]**.
   * 单击 **[!UICONTROL 显示角色分配]** 图标 ![](assets/show-role-allocation-icon.png) 的双曲余切值。

   的 [!UICONTROL 角色分配] 面板。

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >尽管您可以查看 [!UICONTROL 角色分配] 面板，即使贵组织未购买 [!DNL Workfront Scenario Planner] 许可证，则您无法查看有关计划作业角色的信息。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 在 **[!UICONTROL 项目总计]** “角色分配”面板的区域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL作业角色]</td> 
      <td> <p>与以下任一项关联的作业角色的名称：</p> 
       <ul> 
        <li> <p>项目任务</p> </li> 
        <li> <p>项目问题</p> </li> 
        <li> <p>与项目链接的计划</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL计划时数]</td> 
      <td>在计划的总持续时间内与计划上每个工作角色关联的所需小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL计划时数]</td> 
      <td>在项目总持续时间内，与项目任务或问题中每个任务角色关联的计划小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>计划所需小时数与与项目工作相关的计划小时数之差。 [!DNL Workfront] 使用以下公式计算[!UICONTROL Variance]:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>如果资源的计划时间超过方案要求的时间，则[!UICONTROL Variance]为负，以红色显示。 这表示您的资源被过度分配。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在以下情况下，不会显示项目的计划小时数：
   >
   >   
   >   
   >   * 未将任务或问题分配给作业角色，或具有与其关联的作业角色的用户时。
   >   * 任务或问题具有 [!UICONTROL 持续时间] 零。




1. （可选）如果 [!UICONTROL 差异] 列显示您的资源被过度分配，请调整以下选项之一：

   * 降低显示已过度分配或向任务添加更多资源的一个作业角色的计划小时数，并将更多计划小时数分配给新资源。 您可以在编辑任务或问题时更新分配或计划小时数。 有关更多信息，请参阅以下文章：

      * [编辑任务](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [编辑问题](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >您必须拥有其他访问权限和权限才能编辑任务和问题。

   * 增加显示方案中超额分配的角色所需小时数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >您必须具有其他访问权限和权限才能编辑计划。


1. （可选）单击下拉图标，以展开 [!UICONTROL 角色分配] 面板或 [!UICONTROL 工作负载平衡器].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   在 [!UICONTROL 项目总计] 区域。

   >[!TIP]
   >
   >在 [!UICONTROL 角色分配] 面板是时间轴中显示在 [!UICONTROL 工作负载平衡器]. 在时间轴上向后滚动以查看其他月份。

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


