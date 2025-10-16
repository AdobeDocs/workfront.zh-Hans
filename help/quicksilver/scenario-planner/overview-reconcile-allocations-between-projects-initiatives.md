---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: 在项目和计划之间调节资源分配概览
description: 在项目和计划之间协调资源分配概述
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 在项目和计划之间协调资源分配概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

您可以将项目与计划连接起来，以确保您的战略计划与实际工作同步。 当您在[!DNL Scenario Planner]中概述您的战略计划和计划并计划项目中的实际工作时，您可以确保项目中的资源和计划相匹配，这样您就不会过度分配或充分利用它们。

## 先决条件

在开始之前，您必须具备以下条件：

* [!DNL Scenario Planner]中具有与项目连接的计划的计划。
* 计划所需的工作角色分配。
* 项目中具有计划小时数并分配到以下项之一的任务或问题：

   * 工作角色
   * 与工作角色关联的用户

## 连接项目和计划

>[!NOTE]
>
>只有贵组织已为[!DNL Workfront Scenario Planner]购买附加许可证，您才能创建计划并将它们连接到项目。

您可以通过执行以下操作之一来将项目与计划关联：

* 将项目作为新计划导入计划

  有关详细信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中将项目导入计划。

* 将计划发布到项目

  有关详细信息，请参阅[通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目。

这两个流程都会在项目及其相应的计划之间创建连接。 连接它们后，您可以通过比较它们并确保它们匹配来管理它们的资源分配。

## 关于协调链接项目和计划上的资源的注意事项

>[!NOTE]
>
>只有贵组织为[!DNL Workfront Scenario Planner]购买了额外的许可证，您才能查看计划、将其连接到项目以及查看其在项目上的资源分配。

* 您可以将用户、团队和工作角色分配给项目上的工作项，也可以将工作角色分配给计划。 因此，您只能协调项目和计划之间的工作角色。

  >[!TIP]
  >
  >要将用户在项目中的时间与计划中的角色分配相协调，您必须将用户与工作角色关联。

* 您可以在项目的以下区域查看链接项目上的计划工作角色分配：

   * 项目上[!DNL Scenario Planner]项目详细信息[!UICONTROL 区域的]部分。 有关更多信息，请参阅以下文章：

      * [通过在 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)中发布计划来更新或创建项目
      * [管理项目[!UICONTROL 概述]区域中的信息](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >在[!DNL Scenario Planner]项目详细信息[!UICONTROL 的]部分中，您无法并排查看项目和计划的工作角色信息。

   * [!UICONTROL 角色分配]面板位于以下区域：

      * 项目的[!UICONTROL 工作负载均衡器]

        有关如何查看和协调[!UICONTROL 工作负载均衡器]中计划和链接项目之间的角色分配的信息，请参阅[在[!UICONTROL 工作负载均衡器]](../scenario-planner/show-role-allocation-workload-balancer.md)中显示项目和计划的角色分配。

      * [!UICONTROL 任务]分区

        有关如何协调[!UICONTROL 任务]分区中计划和链接项目之间的角色分配的信息，请参阅[在任务列表中显示项目和计划的角色分配](../scenario-planner/show-role-allocation-task-list-nwe.md)。

     >[!TIP]
     >
     >您可以在[!UICONTROL 角色分配]面板中并排查看项目和计划的工作角色信息。

* 您无法查看链接计划上项目的工作角色分配。 有关详细信息，请参阅[在 [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)中将项目导入计划。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
