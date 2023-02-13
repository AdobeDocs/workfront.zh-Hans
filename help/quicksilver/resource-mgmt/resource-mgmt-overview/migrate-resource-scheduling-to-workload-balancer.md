---
filename: migrate-resource-scheduling-to-workload-balancer
product-area: resource-management
navigation-topic: resource-management-overview
title: 从资源计划迁移到 [!UICONTROL 工作负载平衡器]
description: 我们希望您通过帮助您设计迁移计划，尽可能少地体验到工作中断。 以下步骤将帮助您培训团队并确定切换到工作负载平衡器的最佳时间。
author: Alina
exl-id: 4bc08d5f-99c7-40e2-85d6-1de0b585aef8
source-git-commit: d2a8380e3383b97b8245bd2b6d3cb9ff75306e4f
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 0%

---

# 从资源迁移 [!UICONTROL 计划] 到 [!UICONTROL 工作负载平衡器]

<span class="preview">此页面上突出显示的信息是指目前尚不普遍可用的功能。 它仅在“预览”环境中可用。</span>

<!-- drafted for res scheduling deprecation blurb for PREVIEW release - Oct 2022 - CHANGE THIS BLURB TO SOMETHING ELSE AT PRODUCTION:-->

>[!CAUTION]
>  
>  
> <span class="preview">计划区域已从预览环境中删除，并将从 **2023年1月**. </span>\
> <span class="preview"> 在2023年1月之后，您必须在负载平衡器中计划您的资源。 </span>
>  
><span class="preview"> 有关使用工作负载平衡器计划资源的信息，请参阅一节 [工作负载平衡器](../../resource-mgmt/workload-balancer/workload-balancer.md).</span>

本文中的信息仅在您管理了资源中的资源计划时才适用于您 [!UICONTROL 计划] Adobe Workfront地区。 Workfront开始弃用 [!UICONTROL 计划] 2020年11月推出的工具，已使用 [!UICONTROL 工作负载平衡器].

有关的弃用计划信息，请参阅 [!UICONTROL 资源计划] 工具和时间表替换为 [!UICONTROL 工作负载平衡器]，请参阅 [弃用Adobe Workfront中的资源计划工具](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

我们希望您通过帮助您设计迁移计划，尽可能少地体验到工作中断。 以下步骤将帮助您培训团队并确定切换到 [!UICONTROL 工作负载平衡器].

## 找到资源计划工具

您和您的团队可能正在使用某些资源 [!UICONTROL 计划] 工具在Workfront的以下区域：

* 的 [!UICONTROL 计划] 部分 [!UICONTROL 资源化] 面积
* 的 [!UICONTROL 计划] 项目部分
* 的 [!UICONTROL 计划] 小组部分

在此弃用后， [!UICONTROL 工作负载平衡器] 替换所有  [!UICONTROL 资源计划] 工具。

## 步骤1:让您的团队接受培训

参加培训 [新Adobe Workfront经验的资源管理方案](https://one.workfront.com/s/resource-management-program-nwe) （75分钟）Workfront一号。

如果您在登录或访问课程时遇到困难，请联系客户支持。 有关信息，请参阅 [联系客户支持](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## 步骤2:确定迁移的最佳时间 {#step-2-determine-the-best-time-to-migrate}

请按照以下步骤确定迁移的最佳时间是何时：

1. 确定资源中的哪些功能 [!UICONTROL 计划] 您的团队最常使用的工具，并确保在 [!UICONTROL 工作负载平衡器]. 有关 [!UICONTROL 工作负载平衡器]，请参阅文章中的“功能可用性”部分 [弃用Adobe Workfront中的资源计划工具](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

   >[!IMPORTANT]
   >
   >计划工具的几乎所有功能现在都在负载平衡器中。

1. 确定您的团队是否管理分配中的用户分配。 调整或修改用户分配是指在工作项目的整个期间修改每个用户的每日计划小时数。

   在计划工具中编辑的分配不会传输到负载平衡器。 默认情况下，系统会在项目的整个持续时间内平均分配工作项的总计划小时数。

   您必须在负载平衡器中手动管理分配，以确保分配与您在计划工具中的分配相匹配。 有关信息，请参阅 [在工作负载平衡器中管理用户分配](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. “计划”区域中任何保存的过滤器都不会自动传输到工作负载平衡器。 在工作负载平衡器中，请留出时间来创建可能需要的任何过滤器。 有关在工作负载平衡器中创建过滤器的信息，请参阅 [在工作负载平衡器中筛选信息](../workload-balancer/filter-information-workload-balancer.md).

<!--
1. Using the information gathered from Steps 1 and Step 2, decide which version of Step 3 you should continue with based on the needs of your organization.
-->

## 步骤3:迁移到 [!UICONTROL 工作负载平衡器]{#step-3-migrate-to-the-workload-balancer}

我们已根据您在步骤2中的发现结果，确定了此步骤的以下版本：

* [步骤3a:您或您的团队使用 [!UICONTROL 计划] 工具，但不修改用户分配](#step-3a-you-or-your-teams-use-the-scheudling-tools-but-do-not-modify-user-allocation)
* [步骤3b:您或您的团队可在 [!UICONTROL 计划] 工具](#step-3b-you-or-your-teams-manage-user-allocations-in-the-scheduling-tools)

### 步骤3a:您或您的团队使用 [!UICONTROL 计划] 工具，但不修改用户分配

如果您或您的团队没有修改工作分配中的每日小时分配，则可以将计划资源切换到 [!UICONTROL 工作负载平衡器].

![](assets/nwe-workload-balancer-global-350x125.png)

执行以下操作：

* 选择过渡日期。

   >[!TIP]
   >
   >在过渡日期之前，请给您的团队一些时间来完成有关使用负载平衡器的培训。 有关培训的信息，请参阅 [从资源计划迁移到负载平衡器](#migrate-from-resource-uicontrol-scheduling-to-the-uicontrol-workload-balancer) 在本文中。

* 遵循以下准则来协助您的团队：

   * 鼓励您的团队访问 [概述 [!UICONTROL 工作负载平衡器]](../../resource-mgmt/workload-balancer/overview-workload-balancer.md) 页面和所有链接的页面，以深入了解 [!UICONTROL 工作负载平衡器] 工作。
   * 在过渡的一周前为您的团队主办常见问题解答会议，以回答问题，进行切换，然后再举行其他常见问题解答会议以回答后续问题。
   * 使用顶部工具栏中的反馈按钮向Workfront提交反馈。 我们的产品开发人员始终希望了解您的用例，以了解如何 [!UICONTROL 工作负载平衡器] 提供更多价值。

### 步骤3b:您或您的团队可在 [!UICONTROL 计划] 工具

如果您的工作流与此方案匹配，则您在过渡计划中应更具战略性。 显示在 [!UICONTROL 计划] 工具存储在与显示在 [!UICONTROL 工作负载平衡器]. 这表示您在资源中执行的每日分配的调整 [!UICONTROL 计划] 工具不会转移到 [!UICONTROL 工作负载平衡器].

>[!CAUTION]
>
>您必须 **2023年1月** 以确保从“计划”区域分配的用户与生产环境中的负载平衡器中的用户匹配。 此时，我们将从生产环境中删除计划工具。 您必须手动调整工作负载平衡器中的分配，以匹配计划工具中的分配。 <span class="preview">计划工具已从预览环境中删除。</span>


在向 [!UICONTROL 工作负载平衡器] 当您使用 [!UICONTROL 计划] 功能：

* 暂停管理 [!UICONTROL 计划] 工具。 要执行此操作，请执行以下操作：

   * 了解当前项目中任务的平均持续时间，并在确定管理用户分配需要多长时间时考虑这一点。

      >[!TIP]
      >
      >您只需查看当前或规划项目即可，这些项目是您的团队积极进行分配和管理每日分配的项目。

   * 创建任务报告，并在视图中添加任务持续时间字段，并按项目名称对其进行分组。 按平均值在视图中汇总持续时间列，然后保存您的报表。

      有关创建报表的信息，请参阅 [创建自定义报表](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) .

   * 分析任务报告。 例如，如果任务平均持续时间为3天，则最好选择一周的过渡。 让团队停止管理一周的用户分配。 接下来的一周，将团队转换到 [!UICONTROL 工作负载平衡器] 并在下周开始管理用户分配。
   >[!NOTE]
   >
   >如果平均任务持续时间超过在删除计划工具之前剩余的时间，则此建议可能不起作用。


   ![](assets/timeline-stop-using-resource-scheduler-callouts-350x178.png)

   >[!TIP]
   >
   >您可以在过渡期间继续执行任务和发放分配。 所做的分配将反映在资源计划程序和 [!UICONTROL 工作负载平衡器].

* 如果您是一家规模较大的组织，其团队为数百个项目管理资源，则可以考虑从 [!UICONTROL 计划] 工具 [!UICONTROL 工作负载平衡器] 一个组合。 通过在 [!UICONTROL 工作负载平衡器] 一次查看一个特定的组合。

* 允许您的资源经理进行协作：在  [!UICONTROL 资源计划] 工具，并对 [!UICONTROL 工作负载平衡器]. 当由两个协调工具组成的团队使用这两个工具时，请他们将工作流转到 [!UICONTROL 工作负载平衡器].

## 需要更多帮助

如果您需要此迁移的其他信息，请联系自定义支持。 有关联系支持团队的信息，请参阅 [联系客户支持](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
