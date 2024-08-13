---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图表，级别，权限
navigation-topic: access-levels
title: 内置访问级别
description: 当前六个内置访问级别中的每一个都针对特定类型的用户而设计，这些用户包括系统管理员、规划者、工作人员、查看者、请求者和外部用户。 通过这些访问级别，您可以控制用户在系统中可以编辑和查看的内容。 如果您需要自定义访问级别，则可以复制内置访问级别，并根据您希望它允许各种Workfront对象类型的访问量对其进行修改。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 5%

---

# 内置访问级别

<!--Audited: 01/2024-->

>[!NOTE]
>
>本文介绍Adobe Workfront中当前的内置访问级别。 有关新的内置访问级别的信息，请参阅[新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)。


当前六个内置访问级别中的每一个都针对特定类型的用户而设计。 通过这些访问级别，您可以控制用户在系统中可以编辑和查看的内容。

六个内置访问级别中的每一个都针对以下类型的用户而设计：

* 系统管理员
* 规划器
* 员工
* 查看者
* 请求人
* 外部用户

根据访问级别，对于大多数Workfront对象类型，最多有3个设置可用：

<table style="table-layout:auto">
    <tr>
        <td>编辑</td>
        <td>用户可以创建、编辑、删除和共享Workfront对象</td>
    </tr>
    <tr>
        <td>查看</td>
        <td>用户可以查看和共享Workfront对象</td>
    </tr>
    <tr>
        <td>无访问权限</td>
        <td>用户无法访问Workfront对象</td>
    </tr>
</table>

如果您需要自定义“规划者”、“工作人员”、“请求者”或“查看者”访问级别，则可以复制内置访问级别，并确定允许各种Workfront对象类型的访问量。

>[!TIP]
>
>您无法修改系统管理员或外部用户访问级别。

有关创建自定义访问级别或修改内置访问级别之一的信息，请参阅[创建和修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后可以参考这些级别。

有关这些访问级别的一般信息，请参阅[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

## 系统管理员访问级别

在计划许可证上，内置的系统管理员访问级别专为负责管理Adobe Workfront系统的用户而设计。 您无法修改此内置访问级别。

具有系统管理员访问权限级别的用户可以在Workfront中执行所有操作。 他们可以查看和编辑所有其他用户在Workfront中输入的所有Workfront对象和信息。

用户还可以完全访问“设置”区域，以便更改系统级别的任何设置。 并且他们可以访问主菜单![](assets/main-menu-icon.png)或主菜单![](assets/lines-main-menu.png)中的所有区域（如果可用）。

有关详细信息，请参阅[授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)。

## Planner访问级别

计划者访问级别也附加于“计划”许可证，它专为：

* 组、团队、项目和资源的经理
* 任何负责规划、创建和管理任务、项目、项目组合和项目群的人员
* 负责将工作（任务和问题）分配给其他用户的任何人
* 构建报告以及批准工时表、工作项和文档的用户
* 需要访问主菜单![](assets/main-menu-icon.png)或主菜单![](assets/lines-main-menu.png)中所有区域的用户（如果可用）

您可以创建Planner内置访问级别的自定义版本，并确定它允许各种Workfront对象类型的访问量。 有关详细信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

以下是可用于规划者访问级别中对象的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问权限 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   |   | ✓ {\f13 } |
| 任务 |   |   | ✓ {\f13 } |
| 问题 |   |   | ✓ {\f13 } |
| 项目组合 |   |   | ✓ {\f13 } |
| 项目群 |   |   | ✓ {\f13 } |
| 报告、功能板和日历 |   |   | ✓ {\f13 } |
| 筛选器、视图和分组 |   |   | ✓ {\f13 } |
| 文档 |   |   | ✓ {\f13 } |
| 用户 |   |   | ✓ {\f13 } |
| 团队 |   |   | ✓ {\f13 } |
| 模板 |   |   | ✓ {\f13 } |
| 财务数据 |   |   | ✓ {\f13 } |
| 资源管理 |   |   | ✓ {\f13 } |
| 场景计划器 |   |   | ✓ （默认设置为“无访问权限”。） |
| Workfront Goals |   |   | ✓ （默认设置为“无访问权限”。） |

{style="table-layout:auto"}

## 工作人员访问级别

辅助进程访问级别附加到工作许可证，专为在Workfront中执行工作的用户而设计。 他们不会计划工作，而是会完成工作。

具有此访问级别的用户：

* 分配给可以贡献并记录时间的工作项
* 可以审批工作和文档，但不能审批工时表
* 可以访问和共享报告
* 可以与系统中的其他用户通信
* 无法访问主菜单![](assets/main-menu-icon.png)或主菜单![](assets/lines-main-menu.png)中的所有区域（如果可用），并且其“用户”区域名为“团队”。 在团队区域中，具有此访问级别的用户只能查看他们所属的团队，以及分配给这些团队的工作。
* 创建对象的能力有限 — 无法创建项目、项目组合、项目群或报告。

您可以创建Worker内置访问级别的自定义版本，并确定它允许各种Workfront对象类型的访问量。 有关详细信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

以下是辅助进程访问级别中对象的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问权限 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   |   | ✓ （有限：用户只能共享项目、在其中创建任务和问题，以及在已附加到项目的自定义表单中编辑数据。） |
| 任务 |   |   | ✓ {\f13 } |
| 问题 |   |   | ✓ {\f13 } |
| 项目组合 |   | ✓ （默认设置为“无访问权限”。） |   |
| 项目群 |   | ✓ （默认设置为“无访问权限”。） |   |
| 报告、功能板和日历 |   | ✓ {\f13 } |   |
| 筛选器、视图和分组 |   |   | ✓ {\f13 } |
| 文档 |   |   | ✓ {\f13 } |
| 用户 |   |   | ✓ {\f13 } |
| 团队 |   |   | ✓受限访问 |
| 模板 | ✓ {\f13 } |   |   |
| 财务数据 |   | ✓ (默认设置为“无访问权限”。 “查看”设置允许用户仅查看“财务”区域   在项目详细信息中。) |   |
| 资源管理 |   | ✓ {\f13 } |   |
| 场景计划器 |   |   | ✓ （默认设置为“无访问权限”。） |
| Workfront Goals |   |   | ✓ （默认设置为“无访问权限”。） |

{style="table-layout:auto"}

## 审阅者访问级别

“审阅人”访问级别附加到“审阅”许可证，是为向其他用户请求工作以及审阅和批准工作的执行官设计的。 他们不是项目所有者或团队成员，但他们需要访问Workfront以查看他们监督的工作项。

例如，具有此访问级别的利益相关者可以登录Workfront以参与正在进行的营销材料审核，查看工作更新，以及审核文档、批准、报告和日历。

具有审阅者访问级别的用户：

* 不能分派工作项或批准工时表
* 可以访问主菜单![](assets/main-menu-icon.png)或主菜单![](assets/lines-main-menu.png)中的请求和文档区域（如果可用）
* 创建对象的能力有限 — 无法创建项目、项目组合、项目群或报告。

您可以创建Reviewer内置访问级别的自定义版本，并确定它允许各种Workfront对象类型的访问量。 有关详细信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

对于项目和任务，比工作人员访问级别的权限更为有限，以下是适用于审核者访问级别中对象的最高访问设置：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront对象类型</th> 
   <th>无权访问</th> 
   <th>查看访问权限</th> 
   <th>编辑访问权限</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>项目</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td> </td> 
   <td>✓ （默认设置为“无访问权限”。）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td> </td> 
   <td>✓ （默认设置为“无访问权限”。）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>报告、功能板、日历</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>筛选器、视图和分组</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
<tr> 
   <td>团队</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr>

<tr> 
   <td>模板</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>财务数据</td> 
   <td> </td> 
   <td> <p>✓ (默认设置为“无访问权限”。 “查看”设置允许用户仅查看“财务”区域   在项目详细信息中。)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>资源管理</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>场景计划器 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ （默认设置为“无访问权限”。）</td> 
  </tr> 
  <tr> 
   <td>Workfront Goals </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ （默认设置为“无访问权限”。）</td> 
  </tr> 
 </tbody> 
</table>

## 请求者访问级别

请求者访问级别附加到请求许可证，专为在Workfront中发出和接收简单工作请求的用户而设计。 默认情况下，限制为“请求”区域。

例如，用户可以将问题记录到贵组织的技术支持请求队列。

具有此访问级别的用户：

* 可以提出请求并更新这些请求
* 可以上传和批准文档
* 可以检查他们已提交问题的状态
* 无法分派至工作项
* 只能从主菜单![](assets/main-menu-icon.png)中的请求区域或主菜单![](assets/lines-main-menu.png)访问请求（如果可用）。 有关请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

您可以创建请求者内置访问级别的自定义版本，并确定它允许各种Workfront对象类型的访问量。 有关详细信息，请参阅[创建和修改自定义访问级别](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

以下是请求者访问级别中对象的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问权限 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   | ✓ （仅限项目详细信息页面） |   |
| 任务 |   | ✓ Task （只有Task Details页） |   |
| 问题 |   |   | ✓ {\f13 } |
| 项目组合 | ✓ {\f13 } |   |   |
| 项目群 | ✓ {\f13 } |   |   |
| 报告、功能板和日历 |   | ✓ {\f13 } |   |
| 过滤器、视图和分组 |   |   | ✓ {\f13 } |
| 文档 |   |   | ✓ {\f13 } |
| 用户 |   | ✓ {\f13 } |   |
| 团队 |   | ✓ {\f13 } |   |
| 模板 | ✓ {\f13 } |   |   |
| 财务数据 | ✓ {\f13 } |   |   |
| 资源管理 | ✓ {\f13 } |   |   |
| 场景计划器 | ✓ {\f13 } |   |   |
| Workfront Goals |   |   | ✓ （默认设置为“无访问权限”。） |

{style="table-layout:auto"}

## 外部用户访问级别

“外部用户”访问级别未附加到付费Workfront许可证。 这是最严格的访问级别，主要针对协作者(例如未登录Workfront但偶尔需要查看、下载或查看文档的外部顾问)而设计。

即使外部用户无法登录到系统，Workfront用户也可以向外部用户分配任务。 但是，我们不建议将任务和问题分配给外部用户，因为此类工作将在系统中保持未解决状态。

具有外部用户访问级别的用户：

* 只能查看与其共享的文档和日历报告
* 可以查看与其共享文档和日历报告的用户
* 可以批准与其共享的文档

您无法修改此访问级别。

>[!IMPORTANT]
>
>仅当在“设置”的“系统首选项”区域中启用了“使用没有Workfront帐户的人员的电子邮件地址与其协作”选项时，“外部用户”才可用。 有关详细信息，请参阅[配置系统安全首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

虽然这些设置在“外部用户”访问级别的访问级别区域中不可见，但具有此访问权限的用户对Workfront对象类型具有下列最高访问权限：

| Workfront对象类型 | 无权访问 | 查看访问权限 | 编辑访问权限 |
|---|---|---|---|
| 项目 | ✓ {\f13 } |   |   |
| 任务 | ✓ {\f13 } | |   |
| 问题 | ✓ {\f13 } |   |   |
| 项目组合 | ✓ {\f13 } |   |   |
| 项目群 | ✓ {\f13 } |   |   |
| 报告、功能板和日历 |   | ✓ （仅适用于日历报表；无法共享报表） |   |
| 筛选器、视图和分组 | ✓ {\f13 } |   |   |
| 文档 |   | ✓ （无法共享文档） |   |
| 用户 |   | ✓ {\f13 } |   |
| 团队 |   | ✓ {\f13 } |   |
| 模板 | ✓ {\f13 } |   |   |
| 财务数据 | ✓ {\f13 } |   |   |
| 资源管理 | ✓ {\f13 } |   |   |
| 场景计划器 | ✓ {\f13 } |   |   |
| Workfront Goals | ✓ {\f13 } |   |   |
