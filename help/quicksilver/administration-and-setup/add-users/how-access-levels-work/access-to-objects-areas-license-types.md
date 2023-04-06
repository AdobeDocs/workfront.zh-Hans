---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: 按许可证类型访问对象和区域
description: 下表说明了每个Adobe Workfront许可证允许在Workfront中访问对象和区域的最高级别（“编辑”或“查看”）。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 0e690cf9cd6351ee89e32b8f1625e8493aa0ad4b
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 17%

---

# 按许可证类型访问对象和区域

下表说明了每个Adobe Workfront许可证允许在Workfront中访问对象和区域的最高级别（“编辑”或“查看”）。

* **查看**:用户可以查看和共享项目。
* **编辑**:用户可以创建、编辑、删除和共享项目。

   >[!NOTE]
   >
   >当其他用户共享某个对象时，共享者可以指定权限以限制其编辑对象的能力。 有关更多信息，请参阅 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>标准</td>
        <td>浅色</td>
        <td>投稿人</td>
        <td>外部的</td>
    </tr>
    <tr>
        <td>项目</td>
        <td>编辑</td>
        <td>查看</td>
        <td>查看（仅“详细信息”页面）</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>任务</td>
        <td>编辑</td>
        <td>查看</td>
        <td>查看</td>
        <td>查看</td>
    </tr>
    <tr>
        <td>问题</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>项目组合</td>
        <td>编辑</td>
        <td>查看</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>项目群</td>
        <td>编辑</td>
        <td>查看</td>
        <td>无访问权限</td>
        <td>无访问权限</td>
    </tr>
    <tr>
        <td>报表、功能板和日历</td>
        <td>编辑</td>
        <td>查看</td>
        <td>查看*</td>
        <td>查看（仅适用于日历，无共享权限）</td>
    </tr>
    <tr>
        <td>过滤器、视图和分组</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>文档</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>查看（无共享权限）</td>
    </tr>
    <tr>
        <td>用户</td>
        <td>编辑</td>
        <td>查看</td>
        <td>查看</td>
        <td>查看</td>
    </tr>
    <tr>
        <td>团队</td>
        <td>编辑</td>
        <td>查看</td>
        <td>查看</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>模板</td>
        <td>编辑</td>
        <td>无权访问</td>
        <td>无权访问</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>财务数据</td>
        <td>编辑</td>
        <td>无权访问</td>
        <td>无权访问</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>资源管理</td>
        <td>编辑</td>
        <td>查看</td>
        <td>无权访问</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>场景计划器</td>
        <td>编辑</td>
        <td>查看</td>
        <td>无权访问</td>
        <td>无权访问</td>
    </tr>
    <tr>
        <td>Workfront 目标</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>编辑</td>
        <td>无权访问</td>
    </tr>
</table>

&#42; 拥有参与者许可证的用户只能查看与其共享的报表、功能板和日历。

>[!NOTE]
>
>拥有Light许可证或参与者许可证的用户的共享功能有限。 有关更多信息，请参阅 [许可证概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>外部用户无法在Workfront中搜索项目。 他们可以查看专门与他们共享的文档和日历。 用户还可以查看与其共享项目的用户。

您可以在以下文章中找到有关访问级别允许对每个对象和区域执行哪些操作的详细信息：

* [授予对项目的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [授予对文档的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [授予对项目组合的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [授予对程序的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [授予对过滤器、视图和分组的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [授予用户访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [授予团队访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [授予对模板的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [授予对资源管理的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [授予对方案计划员的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [授予对Adobe Workfront目标的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
