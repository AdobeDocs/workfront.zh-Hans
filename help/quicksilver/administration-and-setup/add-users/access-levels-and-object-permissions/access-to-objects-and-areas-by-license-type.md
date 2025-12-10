---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 按许可证类型访问对象和区域
description: 下表告诉您每个Adobe Workfront许可证对Workfront中的对象和区域允许的最高访问级别（编辑或查看）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 23%

---

# 按许可证类型访问对象和区域

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>本文中的信息是指旧版访问级别。 有关当前访问级别的信息，请参阅[新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。

下表告诉您每个Adobe Workfront许可证对Workfront中的对象和区域允许的最高访问级别（编辑或查看）。

* 视图：用户可以查看和共享项目。
* 编辑：用户可以创建、编辑、删除和共享项目。

  >[!NOTE]
  >
  >当其他用户共享对象时，共享者可以指定权限来限制他们编辑该对象的能力。 有关新许可证类型的详细信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

  >[!NOTE]
  >
  >本文包含有关旧版许可证类型的对象访问的信息。 有关新许可证类型的信息，请参阅[新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)和[新许可证概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。

|   | 规划 | 工作 | 审阅 | 请求 | 外部的 |
|---|---|---|---|---|---|
| 项目 | Edit | 编辑（没有“创建”权限） | 视图 | 查看（仅详细信息页面） | 无访问权限 |
| 任务 | Edit | Edit | 视图 | 视图 | 无访问权限 |
| 问题 | Edit | Edit | Edit | Edit | 无访问权限 |
| 项目组合 | Edit | 视图 | 视图 | 无访问权限 | 无访问权限 |
| 项目群 | Edit | 视图 | 视图 | 无访问权限 | 无访问权限 |
| 报告、功能板和日历 | Edit | 视图 | 视图 | 查看&#42; | 查看（仅用于日历，无共享权限） |
| 过滤器、视图和分组 | Edit | Edit | Edit | Edit | 无访问权限 |
| 文档 | Edit | Edit | Edit | Edit | 查看（无共享权限） |
| 用户 | Edit | 视图 | 视图 | 视图 | 视图 |
| 团队 | Edit | Edit | 视图 | 视图 | 无访问权限 |
| 模板 | Edit | 无访问权限 | 无访问权限 | 无访问权限 | 无访问权限 |
| 财务数据 | Edit | 查看（仅项目详细信息中的财务区域） | 视图 | 无访问权限 | 无访问权限 |
| 资源管理 | Edit | 视图 | 视图 | 无访问权限 | 无访问权限 |
| 场景计划器 | Edit | Edit | Edit | 无访问权限 | 无访问权限 |
| Workfront Goals | Edit | Edit | Edit | Edit | 无访问权限 |

&#42;拥有请求许可证的用户只能查看与其共享的报告、功能板和日历。

>[!NOTE]
>
>具有“审阅”许可证或“请求”许可证的用户共享功能有限。 有关详细信息，请参阅[许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md)。
>
>外部用户无法在Workfront中搜索项目。 他们可以查看专门与他们共享的文档和日历。 他们还可以查看与其共享项目的用户。

您可以在以下文章中找到有关每个对象和区域的访问级别所允许的详细信息：

* [授予项目访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授予任务访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授予对文档的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授予对项目组合的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授予程序访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授予对报告、仪表板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授予对筛选器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授予团队访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授予对模板的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授予对Scenario Planner的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [授予对Adobe Workfront目标的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
