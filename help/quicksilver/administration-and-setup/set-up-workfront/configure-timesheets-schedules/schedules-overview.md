---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: 用户，计划
navigation-topic: configure-timesheets-and-schedules
title: 时间表概述
description: 您可以使用计划定义工作周。 您可以将时间表与用户或项目关联。 这允许 [!DNL Adobe Workfront] 计算时间表和用户可用性。 有关说明，请参阅创建计划。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# 时间表概述

<!-- Audited: 1/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

您可以使用计划定义工作周，并将计划与用户或项目关联。 这允许[!DNL Adobe Workfront]计算时间表和用户可用性。 有关说明，请参阅[创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

在Workfront中使用计划时，请考虑以下事项：

* [!DNL Workfront]管理员在计划中标识组织的操作小时。

  同样，组管理员可以确定由他们管理的组所管理的调度的运行小时数。 有关组管理员的详细信息，请参阅[组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

  例如，时间表可以定义为：星期一到星期五，上午8点到下午5点，午餐时间休息一小时。

* [!DNL Workfront]使用时间表确定工作日的开始和结束时间。

  这不会阻止用户在正常工作时间以外在[!DNL Workfront]内工作或完成工作。 通常，聚焦于晚上计划的工作，不必创建新时间表或时间表异常。

  同样，您的组织可能拥有灵活的工作日到达时间。 您可能有一组员工在早上8点到达，另一组员工在早上9点到达。 如果每个组具有相似或相同的计划，则不必为每个组创建唯一的计划。 但是，如果群组具有截然不同的计划，则其用户应该与唯一的计划相关联。 员工理解一项任务是否要在下午5点完成，这意味着工作必须在工作日结束前完成，无论他们何时开始工作。

* 我们建议您为与组织关联的每个时区创建单独的时间表。

  您可以为每个计划分配特定的时区，以确保为在不同时区工作的用户正确计划工作。

* 当用户或项目与计划无关联时，[!DNL Workfront]默认计划用于时间线计算。

  默认计划随您的[!DNL Workfront]系统提供，除非被您创建的新计划替换，否则无法删除默认计划。

* 除了计算时间表之外，[!DNL Workfront]还使用时间表计算用户可用性。

  >[!IMPORTANT]
  >
  >[!DNL Workfront]使用用户或项目计划来确定资源规划者中的资源可用性。 使用的计划取决于[!DNL Workfront]管理员为[!UICONTROL 使用]计算资源可用性设置选择的内容。 有关资源管理设置的信息，请参阅[配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

## 计划的层次结构

如果将任务分配给与时间表关联的用户，并且任务驻留在与第二时间表关联的项目中，则您至少有2个时间表可以应用于您的时间表计算。

>[!IMPORTANT]
>
>仅当[!UICONTROL 安装程序]的[!UICONTROL 资源管理]区域中的[!UICONTROL 使用计算资源可用性]设置设置为[!UICONTROL 用户计划]时，[!DNL Workfront]才使用用户的计划。 有关[!UICONTROL 使用]计算资源可用性设置如何影响用于资源管理的计划的信息，请参阅[配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)。

存在多个计划时，系统使用计划的顺序为：


* 当一个用户被分配给任务时，[!DNL Workfront]使用下列计划之一，如[!UICONTROL 设置]的[!UICONTROL 项目偏好设置]区域中所定义：

   * 分配给任务的用户的计划
   * 与项目关联的计划。

     有关个人时间的详细信息，请参阅[配置个人休息时间](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)。

* 当多个用户被分配到一项任务时，并且该用户在任务的时间范围内具有不同的计划，则[!DNL Workfront]会使用以下计划之一，如[!UICONTROL 设置]的[!UICONTROL 项目首选项]区域中所定义：

   * 被指定为主要被分配人的用户的计划
   * 与项目关联的计划。

     有关项目首选项的详细信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

* 如果分配给任务的用户没有计划，或任务仅分配给工作角色、团队或未分配，[!DNL Workfront]将项目计划用于时间表计算。
* 如果分配给任务的用户没有计划，或者任务仅分配给工作角色、团队或未分配，并且项目没有计划，则[!DNL Workfront]使用系统中指定为默认计划的时间表进行时间线计算。

  ![](assets/default-schedule.png)

## [!DNL Workfront]中的Collaboration跨时区

有关使用计划帮助用户在跨时区[!DNL Workfront]中进行协作的信息，请参阅[跨时区工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。
