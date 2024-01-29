---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: 用户，计划
navigation-topic: configure-timesheets-and-schedules
title: 时间表概述
description: 您可以使用计划定义工作周。 您可以将时间表与用户或项目关联。 这允许 [!DNL Adobe Workfront] 以计算时间线和用户可用性。 有关说明，请参阅创建计划。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 时间表概述

<!-- Audited: 1/2024 -->

您可以使用计划定义工作周，并将计划与用户或项目关联。 这允许 [!DNL Adobe Workfront] 以计算时间线和用户可用性。 有关说明，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

在Workfront中使用计划时，请考虑以下事项：

* 此 [!DNL Workfront] 管理员在计划中标识组织的营业时间。

  同样，组管理员可以确定由他们管理的组所管理的调度的运行小时数。 有关组管理员的详细信息，请参见 [组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  例如，时间表可以定义为：星期一到星期五，上午8点到下午5点，午餐时间休息一小时。

* [!DNL Workfront] 使用时间表确定工作日的开始和结束时间。

  这不会阻止用户在中工作或完成工作 [!DNL Workfront] 在正常工作时间之外。 通常，聚焦于晚上计划的工作，不必创建新时间表或时间表异常。

  同样，您的组织可能拥有灵活的工作日到达时间。 您可能有一组员工在早上8点到达，另一组员工在早上9点到达。 如果每个组具有相似或相同的计划，则不必为每个组创建唯一的计划。 但是，如果群组具有截然不同的计划，则其用户应该与唯一的计划相关联。 员工理解一项任务是否要在下午5点完成，这意味着工作必须在工作日结束前完成，无论他们何时开始工作。

* 我们建议您为与组织关联的每个时区创建单独的时间表。

  您可以为每个计划分配特定的时区，以确保为在不同时区工作的用户正确计划工作。

* 此 [!DNL Workfront] 当用户或项目未与时间表关联时，默认时间表用于时间表计算。

  默认计划随附于 [!DNL Workfront] 系统，除非将其替换为您创建的新计划，否则无法删除它。

* 除了计算时间表之外， [!DNL Workfront] 使用计划计算用户可用性。

  >[!IMPORTANT]
  >
  >[!DNL Workfront] 使用用户或项目计划确定资源规划者中的资源可用性。 使用哪个时间表取决于 [!DNL Workfront] 管理员已为 [!UICONTROL 使用以下方式计算资源可用性] 设置。 有关资源管理设置的信息，请参见 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 计划的层次结构

如果将任务分配给与时间表关联的用户，并且任务驻留在与第二时间表关联的项目中，则您至少有2个时间表可以应用于您的时间表计算。

>[!IMPORTANT]
>
>[!DNL Workfront] 仅在以下情况下使用用户计划： [!UICONTROL 使用以下方式计算资源可用性] 设置已设置为 [!UICONTROL 用户计划] 在 [!UICONTROL 资源管理] 面积 [!UICONTROL 设置]. 有关如何 [!UICONTROL 使用以下方式计算资源可用性] 设置会影响用于资源管理的计划，请参阅 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

存在多个计划时，系统使用计划的顺序为：

* 当用户被分配给任务时， [!DNL Workfront] 使用用户的计划来计算任务的时间线。 这还包括用户的个人时间。 项目的计划将被忽略。

  有关个人时间的详细信息，请参阅 [配置个人休息时间](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 当多个用户被分配到一项任务时，这些用户在任务的时间范围内具有不同的计划， [!DNL Workfront] 使用以下计划之一，如 [!UICONTROL 项目首选项] 面积 [!UICONTROL 设置]：

   * 被指定为主要被分配人的用户的计划
   * 与项目关联的计划。

     有关项目首选项的详细信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果分配给任务的用户没有计划，或者任务仅分配给工作角色、团队或未分配， [!DNL Workfront] 使用项目计划进行时间线计算。
* 如果分配给任务的用户没有计划，或者任务仅分配给工作角色、团队或未分配，并且项目没有计划，则 [!DNL Workfront] 使用系统中指定为时间表计算的默认时间表的时间表。

  ![](assets/default-schedule.png)

## 中的协作 [!DNL Workfront] 跨时区

有关使用计划帮助用户进行协作的信息 [!DNL Workfront] 跨时区，请参见 [跨时区工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
