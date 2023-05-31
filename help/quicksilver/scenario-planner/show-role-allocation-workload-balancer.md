---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在工作负载均衡器中显示项目和计划的角色分配
description: 连接项目和计划后，您可以并排管理其资源分配以确保它们
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# 在中显示项目和计划的角色分配 [!UICONTROL 工作负载均衡器]

>[!IMPORTANT]
>
>贵组织必须购买额外的许可证 [!DNL Adobe Workfront Scenario Planner] 以便查看有关项目的计划信息。 有关获取 [!DNL Workfront Scenario Planner]，请参见 [使用所需的访问权限 [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

连接项目和计划后，您可以并排管理其资源分配以确保它们相匹配。 这样可以避免过度分配或利用不足。

本文介绍如何使用协调资源 [!UICONTROL 角色分配] 面板位于 [!UICONTROL 工作负载均衡器] 项目的URL。

有关在项目和计划之间协调资源的一般信息（包括先决条件），请参阅 [协调项目和计划之间的资源分配概览](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## 访问要求

您需要执行以下操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 计划*</b> </p> </td> 
   <td>[！UICONTROL Business]或更高版本</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> 许可证*</b> </p> </td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td><b>产品</b> </td> 
   <td> <p>您必须为购买附加许可证 [!DNL Adobe Workfront Scenario Planner] 以访问本文中介绍的功能。</p> <p>有关获取 [!DNL Workfront Scenario Planner]，请参见 <a href="../scenario-planner/access-needed-to-use-sp.md">使用所需的访问权限 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>[！UICONTROL视图]或更高的项目访问权限 </p> <p>注意：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参见 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>项目的[！UICONTROL视图]或更高权限</p> <p>有关请求对计划的附加访问权限的信息，请参阅 <a href="../scenario-planner/request-access-to-plan.md">[！UICONTROL Request]访问 [!DNL Workfront Scenario Planner]</a>.</p> <p>有关请求对项目的附加访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 在中显示项目和计划的角色分配 [!UICONTROL 工作负载均衡器]

如果您的公司购买了 [!DNL Workfront Scenario Planner] 许可证，您可以在项目级别协调计划和与其链接的项目之间的资源分配 [!UICONTROL 工作负载均衡器].

1. （视情况而定）使用以下文章中描述的方法之一将项目与计划关联：

   * [将项目导入中的计划 [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [通过在以下位置发布计划来更新或创建项目： [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >如果您更改了计划中的资源，则必须重新发布计划所属的方案，以便计划中的最新资源信息能够更新项目。

1. 转到要查看项目和相关计划的工作角色分配情况的项目。
1. 单击 [!UICONTROL 工作负载均衡器] （在左侧面板中）。

   您可能需要单击 **[!UICONTROL 计划]**，则 **[!UICONTROL 切换到工作负载均衡器]**.

1. 执行下列操作之一：

   * 单击 **[!UICONTROL 月]** 要按月查看工作负载均衡器，请单击时间线中一个月旁边的下拉菜单 ![](assets/drop-down-next-to-month-month-view-wb.png)，然后单击 **[!UICONTROL 更多]**.
   * 单击 **[!UICONTROL 显示角色分配]** 图标 ![](assets/show-role-allocation-icon.png) 工具栏的右上角。

   此 [!UICONTROL 角色分配] 面板显示。

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >虽然您可以查看 [!UICONTROL 角色分配] 面板，即使贵组织未购买 [!DNL Workfront Scenario Planner] 许可证，则无法查看有关计划工作角色的信息。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. 请查看 **[!UICONTROL 项目总计]** “角色分配”面板的区域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL工作角色]</td> 
      <td> <p>与以下任意项关联的工作角色的名称：</p> 
       <ul> 
        <li> <p>项目中的任务</p> </li> 
        <li> <p>项目问题</p> </li> 
        <li> <p>链接到项目的计划</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划小时数]</td> 
      <td>计划总持续时间内与计划上每个工作角色关联的所需小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL计划小时数]</td> 
      <td>在项目总持续时间内，与项目任务或问题中的每个工作角色关联的已计划小时数。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL变量]</td> 
      <td> <p>计划上所需的小时数与项目上工作相关的计划小时数之间的差额。 [!DNL Workfront] 使用以下公式计算[！UICONTROL方差]：</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>当计划资源的时间超过计划所需的小时数时，[！UICONTROL方差]为负数，并以红色显示。 这意味着您的资源被过度分配。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >项目中的计划小时数未显示在以下方案中：
   >
   >   
   >   
   >   * 未将任务或问题分配给工作角色或与其关联的工作角色的用户时。
   >   * 当任务或问题具有 [!UICONTROL 持续时间] 零。




1. （可选）如果 [!UICONTROL 变量] 列显示您的资源分配过量，请调整以下选项之一：

   * 降低显示过度分配的一个工作角色的已计划小时数，或向任务添加更多资源，并向新资源分配更多已计划小时数。 编辑任务或问题时，您可以更新分配或任务或问题的已计划小时数。 有关更多信息，请参阅以下文章：

      * [编辑任务](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [编辑问题](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >您必须具有其他访问权限才能编辑任务和问题。

   * 增加显示计划过度分配的角色所需小时数。 有关更多信息，请参阅 [在中创建和编辑计划 [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >您必须具有其他访问权限才能编辑计划。


1. （可选）单击下拉图标以展开 [!UICONTROL 角色分配] 面板中或时间轴中的 [!UICONTROL 工作负载均衡器].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   中显示的相同类型的信息 [!UICONTROL 项目总计] 区域也会每月显示。

   >[!TIP]
   >
   >中列出的月份 [!UICONTROL 角色分配] 面板是时间轴中的月份，显示在的屏幕上 [!UICONTROL 工作负载均衡器]. 在时间轴上前后滚动以查看其他月份。

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


