---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 2020.2资源管理增强功能：工作负载均衡器
description: 本页介绍了2020.2版本中对生产环境的所有资源管理增强功能。 这些增强功能在2020年5月11日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# 2020.2资源管理增强功能：工作负载均衡器

本页介绍了2020.2版本中对生产环境的所有资源管理增强功能。 这些增强功能在2020年5月11日这一周的生产环境中提供。

有关2020.2版本可用的所有更改列表，请参阅[2020.2版本概述](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md)。

人员是一级资产。 使用工作负载均衡器，您可以保护他们免于倦怠，使他们能够完成最佳工作，同时使他们与关键的公司战略保持一致。 引入重新设计的计划体验，让您以同一视图可视化和管理人员的工作负荷和需求。 用户界面提供了关于过度利用和利用率不足的清晰直观映射，并对所有利益相关者透明。 人员经理可以将该信息用作输入，并且来自同一屏幕的操作会在时间线中重新平衡工作，该时间线随后将反映在Workfront平台的其余部分中。

>[!NOTE]
>
>工作负载均衡器在2019.4版本中开始作为测试版发布。 所有工作负载均衡器增强功能通常在2020.2版本中提供。 此页面上描述的增强功能已添加到2020.2版本。 有关工作负载均衡器的概述，请参阅[工作负载均衡器概述](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

## 在工作负载均衡器中调整每日和每周分配

为避免资源燃尽，您现在可以使用工作负载均衡器调整用户的每日和每周分配以便工作。

在此增强功能之前，只能使用“资源计划”工具实现此功能。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 工作负载均衡器过滤器

要使工作负载均衡器中的信息与您相关，您现在可以为工作负载均衡器的未分配工作和已分配工作区域创建过滤器，并保存它们以供将来使用。 然后，您可以编辑保存的版本以进行细微更改，而不是从头开始使用新筛选器。

有关在工作负载均衡器中过滤的信息，请参阅在工作负载均衡器中管理过滤器[&#128279;](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 在工作负载均衡器中显示剩余小时数

为了帮助您做出正确的分配决策，现在通过新设置可查看用户根据其计划可工作的小时数与已分配至工作的小时数（剩余小时数）之间的小时数差异。 新设置现在在工作负载均衡器中可用。

有关在工作负载均衡器中查看信息的信息，请参阅[在工作负载均衡器中导航](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅[在工作负载均衡器中导航](https://experienceleague.adobe.com/en/docs/workfront/using/home)。)

**在以下环境中可用：**

* 新的Adobe Workfront体验

## 在工作负载均衡器的未分配工作区域显示任务和项目的每日计划小时数

为了帮助您在分配任务之前了解任务将如何影响用户的工作负载，“显示分配”设置现在正在管理工作负载均衡器的未分配工作区域中显示的信息。 启用此设置后，任务和项目的计划小时数都会显示在工作负载均衡器的未分配工作区域。

在此更改之前，此设置仅更新均衡器的已分配工作区域中的信息。

有关导航工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[导航工作负载均衡器](https://experienceleague.adobe.com/en/docs/workfront/using/home)。)

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验（以前仅适用于Task）

## 工作负载均衡器的新设置框

为了简化您的体验，现在提供了一个设置框，其中显示其他工具以更新工作负载均衡器中的视图。 此框包括以下设置：

* 按项目分组
* 显示任务和项目的已分配小时数或剩余小时数。

有关在工作负载均衡器中查看信息的信息，请参阅[在工作负载均衡器中导航](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅[在工作负载均衡器中导航](https://experienceleague.adobe.com/en/docs/workfront/using/home)。)

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 使用链接共享工作负载均衡器

您现在可以与管理人员共享人员的工作量，以便他们能够了解您的人员配备需求。 为此，您现在可以通过与他人共享工作负载均衡器的唯一URL来共享工作负载均衡器。

有关导航工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[导航工作负载均衡器](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 在工作负载均衡器中更改日期范围

为进一步帮助您自定义工作负载均衡器的时间线持续时间以满足您的需求，您现在可以选择一次显示的2、4或6周的自定义时间段。

在此增强功能之前，工作负载均衡器始终显示从本周开始的信息。

有关导航工作负载均衡器的信息，请参阅[导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[导航工作负载均衡器](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront Experience（以前可用）

## 将任务移动并复制到另一个项目会保留任务限制，当任务可以适应项目的时间表时

当您复制任务或将其移动到其他项目时，我们对Workfront处理任务的特定日期任务限制的方式进行了改进。 特定日期的任务约束的示例包括“必须开始于”、“必须完成于”、“固定日期”、“开始时间不晚于”等。

例如，当您将具有“必须开始于”限制的任务移动或复制到其“计划开始日期”早于任务的“开始日期”的另一个项目时，任务会在复制或移动后保留该限制。 当您将具有必须开始日期限制的任务移动或复制到其计划开始日期在任务开始日期之后的项目时，任务限制会尽快变为。

在此更改之前，任务限制始终会尽快更改为。

有关移动任务的信息，请参阅[移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md)(或者如果您使用的是Adobe Workfront Classic，请参阅[移动任务](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

有关复制任务的信息，请参阅[复制和复制任务](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[复制和复制任务](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

有关所有任务限制的概述，请参阅[任务限制概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (或者，如果您使用的是Adobe Workfront Classic，请参阅[任务限制概述](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 在“详细信息”选项卡或任务列表中进行更改时防止数据丢失

为了防止在手动保存更改时更新项目级别任务列表中的对象或任务的“详细信息”页面上的信息时丢失数据，现在会显示一条警告消息，在您尝试编辑标题中的信息之前通知您有未保存的更改。 在保存更改之前，只允许订阅对象或将对象添加到收藏夹。

有关编辑列表中的任务的信息，请参阅[编辑列表中的任务](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**在以下环境中可用：**

* 新的Adobe Workfront体验

## 使用自定义状态为组创建批准流程

为了更便于组管理自己的独特工作流，您现在可以在审批流程中使用特定于组的自定义状态。

以前，组无法将其自身的自定义状态用于其特定于组的审批流程。 只有系统范围状态可用，并且这些状态并不总是适合组审批流程。

现在，可在一次性审批流程和系统范围审批流程中使用自定义状态：

* 为对象（项目、任务或问题）创建一次性审批流程，并将其基于与处理该对象的组相关联的状态。 这包括与该组关联的任何自定义状态。
* 创建一个全局审批流程，使其仅适用于该组或系统中的每个人。

对于具有审批流程管理访问权限的用户，有关配置审批流程的信息，请参阅[为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)(或者如果您使用的是Adobe Workfront Classic，请参阅[创建审批流程](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

对于用户，有关将审批流程与工作项关联的信息，请参阅[将新的或现有的审批流程与工作关联](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)(或者，如果您使用的是Adobe Workfront Classic，请参阅[将新的或现有的审批流程与工作关联](https://experienceleague.adobe.com/en/docs/workfront/using/home))。

**在以下环境中可用：**

* Adobe Workfront Classic
* 新的Adobe Workfront体验

## 在工作负载均衡器中更新分配的更简便方法

为了更便于管理工作负载均衡器中对工作项的分配，您现在可以双击该工作项。 您仍然可以使用现有的“编辑分配”菜单选项。 此外，您不再需要启用显示分配才能更新它们。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

## 在工作负载均衡器中更新任务已计划小时数

>[!NOTE]
>
>此增强功能将在2020.2版本发布后不久在生产中可用。

访问级别的资源管理区域中的新选项现在允许具有此访问权限的用户从工作负载均衡器编辑已计划小时数。 在工作负载均衡器调整分配时，每日分配总数无需与任务的已计划小时数匹配。 保存分配后，分配小时总数将成为任务的计划小时数。 这仅适用于具有简单持续时间类型的任务。

有关管理工作负载均衡器中的分配的信息，请参阅[管理工作负载均衡器中的用户分配](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)。

有关授予对资源管理的访问权限的信息，请参阅[授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)。

## 从工作负载均衡器中移除“beta”标签

在2020.2版本中，工作负载均衡器将不再处于测试版状态，您将能够使用资源均衡器查看和管理资源分配和分配。 已在“预览”环境中移除“beta”标签。 在20.2生产版本中将做出相同的更改。 有关工作负载均衡器的信息，请参阅[工作负载均衡器概述](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。
