---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 按新许可证访问对象和区域
description: 下表告诉您每个Adobe Workfront许可证对Workfront中的对象和区域允许的最高访问级别（编辑或查看）。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 22%

---

# 通过新许可证访问对象和区域

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>本文中的信息是指当前的访问级别。 有关旧版访问级别的信息，请参阅[访问级别概述](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

下表告诉您每个Adobe Workfront许可证对Workfront中的对象和区域允许的最高访问级别（编辑或查看）。

* **查看**：用户可以查看和共享项目。
* **编辑**：用户可以创建、编辑、删除和共享项目。

  >[!NOTE]
  >
  >当其他用户共享对象时，共享者可以指定权限来限制他们编辑该对象的能力。 有关详细信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>标准</td>
        <td>轻量</td>
        <td>投稿人</td>
        <td>外部的</td>
    </tr>
    <tr>
        <td>项目</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>任务</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>问题</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>项目组合</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>项目群</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>报告、功能板和日历</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图*</td>
        <td>查看（仅用于日历，无共享权限）</td>
    </tr>
    <tr>
        <td>过滤器、视图和分组</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>文档</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>查看（无共享权限）</td>
    </tr>
    <tr>
        <td>用户</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>视图</td>
    </tr>
    <tr>
        <td>团队</td>
        <td>Edit</td>
        <td>视图</td>
        <td>视图</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>模板</td>
        <td>Edit</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>财务数据</td>
        <td>Edit</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>资源管理</td>
        <td>Edit</td>
        <td>视图</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>场景计划器</td>
        <td>Edit</td>
        <td>视图</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>Edit</td>
        <td>无访问权限</td>
    </tr>
</table>

&#42;拥有参与者许可证的用户只能查看与其共享的报告、功能板和日历。

>[!NOTE]
>
>* 拥有轻量级许可证或参与者许可证的用户共享功能有限。 有关详细信息，请参阅[许可证概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md)。
>
>* 外部用户无法在Workfront中搜索项目。 他们可以查看专门与他们共享的文档和日历。 他们还可以查看与其共享项目的用户。
>
>* 参与者用户和外部用户看不到在系统范围内共享的内容。  必须明确地与他们共享。

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
