---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: 用户，计划
navigation-topic: configure-timesheets-and-schedules
title: 计划概述
description: 您可以使用计划来定义工作周。 您可以将计划与用户或项目关联。 这允许 [!DNL Adobe Workfront] 计算时间轴和用户可用性。 有关说明，请参阅创建计划。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 计划概述

您可以使用计划定义工作周，并将计划与用户或项目关联。 这允许 [!DNL Adobe Workfront] 计算时间轴和用户可用性。 有关说明，请参阅 [创建计划](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

在Workfront中处理计划时，请考虑以下事项：

* 的 [!DNL Workfront] 管理员确定计划中组织的操作小时数。

   同样，组管理员也可以确定由他们管理的组管理的计划的运行小时数。

   有关群组管理员的更多信息，请参阅 [组管理员](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   例如，可以将计划定义为：星期一到星期五上午8点到下午5点，午餐休息一小时。

* [!DNL Workfront] 使用计划来确定工作日的开始时间和结束时间。

   这不会阻止用户在中工作或完成工作 [!DNL Workfront] 在正常工作时间之外。 通常，不必创建新的计划或计划例外，即可专注于晚上计划的工作。

   同样，贵组织在工作日的到达时间可能会很灵活。 您可能有一组员工在上午8点到达，另一组员工在上午9点到达。 如果每个组具有相似或相同的计划，则无需为每个组创建唯一的计划。 但是，如果这些组的计划有很大的不同，则其用户应与唯一的计划相关联。 员工了解某项任务是否将在下午5点完成，这意味着无论他们何时上班，都必须在工作日结束前完成工作。

* 我们建议您为与组织关联的每个时区分别创建计划。

   您可以为每个计划分配一个特定时区，以确保为在不同时区工作的用户正确安排工作时间。

* 的 [!DNL Workfront] 当用户或项目未与计划关联时，时间轴计算中会使用默认计划。

   默认计划随您的 [!DNL Workfront] 系统，除非被您创建的新计划替换，否则无法删除。

* 除了计算时间表外， [!DNL Workfront] 使用计划来计算用户可用性。

   >[!IMPORTANT]
   >
   >[!DNL Workfront] 使用用户或项目计划来确定资源计划员中的资源可用性。 使用的计划取决于 [!DNL Workfront] 为选择的管理员 [!UICONTROL 使用计算资源可用性] 设置。 有关“资源管理”设置的信息，请参阅 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## 计划的层次结构

如果任务被分配给与某个计划相关联的用户，并且驻留在与另一个计划相关联的项目中，则您至少有2个计划可能会应用于时间轴计算。

>[!IMPORTANT]
>
>[!DNL Workfront] 仅在 [!UICONTROL 使用计算资源可用性] 设置设置为 [!UICONTROL 用户的计划] 在 [!UICONTROL 资源管理] 面积 [!UICONTROL 设置]. 有关 [!UICONTROL 使用计算资源可用性] 设置会影响用于资源管理的计划，请参阅 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

当存在多个计划时，系统使用计划的顺序是：

* 将用户分配到任务后， [!DNL Workfront] 使用用户的计划来计算任务的时间轴。 这还包括用户的个人时间。 项目的计划将被忽略。

   有关个人时间的更多信息，请参阅 [在中配置个人休息时间 [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* 当将多个用户分配到一个任务，并且这些用户在该任务的时间范围内有不同的计划时， [!DNL Workfront] 使用下列任一计划，如 [!UICONTROL 项目首选项] 面积 [!UICONTROL 设置]:

   * 指定为主要代理人的用户的计划
   * 与项目关联的计划。

      有关项目首选项的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 如果分配给任务的用户没有计划，或者该任务仅分配给作业角色、团队或未分配， [!DNL Workfront] 将项目计划用于时间轴计算。
* 如果分配给任务的用户没有计划，或者该任务仅被分配给作业角色、团队或未分配，并且项目没有计划，则 [!DNL Workfront] 在指定为时间轴计算的默认计划的系统中使用计划。

   ![](assets/default-schedule.png)

## 协作 [!DNL Workfront] 跨时区

有关使用计划帮助用户在 [!DNL Workfront] 跨时区，请参阅 [跨时区工作](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
