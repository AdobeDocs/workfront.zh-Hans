---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图，级别，权限
navigation-topic: access-levels
title: Adobe Workfront中的内置访问级别
description: 六个内置访问级别中的每个级别都针对特定类型的用户（包括系统管理员、计划员、工作人员、审核者、请求者和外部用户）而设计。 这些访问级别允许您控制用户可以在系统中编辑和查看哪些内容。 如果您需要自定义访问级别，则可以复制内置访问级别，并确定您希望它允许的各种Workfront对象类型的访问量。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 6%

---

# Adobe Workfront中的内置访问级别

六个内置访问级别中的每个级别都针对特定类型的用户而设计：

* 系统管理员
* 计划人
* 员工
* 查看者
* 请求人
* 外部用户

根据访问级别，大多数Workfront对象类型最多可使用3个设置：

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

如果您需要自定义的“计划员”、“工人”、“请求者”或“审核者”访问级别，则可以复制内置访问级别并确定您希望它允许的各种Workfront对象类型的访问量。 有关创建自定义访问级别或修改其中一个内置访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后，您可以参考这些级别。

有关这些访问级别的常规信息，请参阅 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## 系统管理员访问级别

此内置访问级别附加到“计划”许可证，专为负责管理Adobe Workfront系统的用户而设计。 您无法修改此内置访问级别。

具有系统管理员访问权限级别的用户可以在Workfront中执行所有操作。 他们可以查看和编辑所有其他用户在Workfront中输入的所有Workfront对象和信息。

他们还可以访问完整的设置区域，在该区域中，他们可以更改系统级别的任何设置。 他们可以访问主菜单中的所有区域 ![](assets/main-menu-icon.png).

有关更多信息，请参阅 [授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## 计划员访问层

此访问级别也附加到计划许可证，旨在：

* 组、团队、项目和资源的经理
* 负责规划、创建和管理任务、项目、项目组合和项目的任何人
* 负责将工作（任务和问题）分配给其他用户的任何人
* 生成报告并批准工时单、工作项和文档的用户
* 需要访问主菜单中所有区域的用户 ![](assets/main-menu-icon.png)

您可以创建计划员内置访问级别的自定义版本，并确定它允许的各种Workfront对象类型的访问量。 有关更多信息，请参阅 [Adobe Workfront中的内置访问级别](#Customiz) 在本文中。

以下是计划员访问层中对象可用的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   |   | ✓ |
| 任务 |   |   | ✓ |
| 问题 |   |   | ✓ |
| 项目组合 |   |   | ✓ |
| 项目群 |   |   | ✓ |
| 报表（包括功能板和日历报表） |   |   | ✓ |
| 过滤器、视图和分组 |   |   | ✓ |
| 文档 |   |   | ✓ |
| 用户 |   |   | ✓ |
| 模板 |   |   | ✓ |
| 财务数据 |   |   | ✓ |
| 资源管理 |   |   | ✓ |
| 场景计划器 |   |   | ✓（默认设置为“无权访问”。） |
| Workfront 目标 |   |   | ✓（默认设置为“无权访问”。） |

{style=&quot;table-layout:auto&quot;}

## 工作人员访问级别

此内置访问级别附加到工作许可证，专为在Workfront中执行工作的用户而设计。 他们没有计划工作；他们完成了。

具有此访问级别的用户：

* 被分配给可在其中贡献内容和记录时间的工作项目
* 可以批准工作和文档，但不能批准工时单
* 可以访问和共享报表
* 可以与系统中的其他用户通信
* 可以访问主菜单中的所有区域 ![](assets/main-menu-icon.png)，但其“用户”区域被命名为“团队”。 在“团队”区域中，具有此访问级别的用户只能查看他们所属的团队以及分配给这些团队的工作。
* 创建对象的能力有限 — 无法创建项目、项目组合、项目或报告。

您可以创建Worker内置访问级别的自定义版本，并确定它允许对各种Workfront对象类型的访问量。 有关更多信息，请参阅 [Adobe Workfront中的内置访问级别](#Customiz) 在本文中。

以下是工作程序访问级别中对象可用的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   |   | ✓(有限：用户只能共享项目、在项目中创建任务和问题，以及以已附加到该项目的自定义表单编辑数据。) |
| 任务 |   |   | ✓ |
| 问题 |   |   | ✓ |
| 项目组合 |   | ✓（默认设置为“无权访问”。） |   |
| 项目群 |   | ✓（默认设置为“无权访问”。） |   |
| 报表（包括功能板和日历报表） |   | ✓ |   |
| 过滤器、视图和分组 |   |   | ✓ |
| 文档 |   |   | ✓ |
| 用户 |   |   | ✓ |
| 模板 | ✓ |   |   |
| 财务数据 |   | ✓(默认设置为“无权访问”。 “查看”设置允许用户仅查看“项目详细信息”中的“财务”区域。) |   |
| 资源管理 |   | ✓ |   |
| 场景计划器 |   |   | ✓（默认设置为“无权访问”。） |
| Workfront 目标 |   |   | ✓（默认设置为“无权访问”。） |

{style=&quot;table-layout:auto&quot;}

## 审阅人访问级别

此访问级别附加在“审核”许可证中，适用于请求其他用户工作以及审核和批准工作的执行人员。 这些人员不是项目所有者或团队成员，但他们需要访问Workfront以查看他们监督的工作项目。

例如，具有此访问级别的利益相关方可登录Workfront以参与对营销材料的持续审核，查看工作的工作更新，以及审核文档、批准、报告和日历。

具有审阅人访问级别的用户：

* 无法分配工作项或批准时间表
* 可以在主菜单中访问请求和文档 ![](assets/main-menu-icon.png).
* 创建对象的能力有限 — 无法创建项目、项目组合、项目或报告。

您可以创建Reviewer内置访问级别的自定义版本，并确定它允许对各种Workfront对象类型的访问量。 有关更多信息，请参阅 [Adobe Workfront中的内置访问级别](#Customiz) 在本文中。

与工作人员访问级别相比，对项目和任务的限制更大，下面是“审阅人”访问级别中对象可用的最高访问设置：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront对象类型</th> 
   <th>无权访问</th> 
   <th>查看访问</th> 
   <th>编辑访问权限</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>项目</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td> </td> 
   <td>✓（默认设置为“无权访问”。）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>报表（包括功能板和日历报表）</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>过滤器、视图和分组</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>财务数据</td> 
   <td> </td> 
   <td> <p>✓(默认设置为“无权访问”。 “查看”设置允许用户仅查看“项目详细信息”中的“财务”区域。)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>资源管理</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>场景计划器 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓（默认设置为“无权访问”。）</td> 
  </tr> 
  <tr> 
   <td>Workfront 目标 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓（默认设置为“无权访问”。）</td> 
  </tr> 
 </tbody> 
</table>

## 请求者访问级别

此内置访问级别附加到请求许可证，专为在Workfront中发出和接收简单工作请求的用户而设计。 默认情况下，它们仅限于“请求”区域。

例如，用户可以将问题记录到贵组织的服务台请求队列。

具有此内置访问级别的用户：

* 可以发出请求并更新这些请求
* 可以上传和批准文档
* 可以查看他们提交的问题的状态
* 无法分配给工作项
* 只能从主菜单访问请求 ![](assets/main-menu-icon.png). 有关请求队列的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

您可以创建Requester内置访问级别的自定义版本，并确定它允许对各种Workfront对象类型的访问量。 有关更多信息，请参阅 [Adobe Workfront中的内置访问级别](#Customiz) 在本文中。

以下是请求者访问级别中对象可用的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   | ✓（仅“项目详细信息”页面） |   |
| 任务 |   | ✓（仅详细信息页面） |   |
| 问题 |   |   | ✓ |
| 项目组合 | ✓ |   |   |
| 项目群 | ✓ |   |   |
| 报表（包括功能板和日历报表） |   | ✓（仅详细信息页面） |   |
| 过滤器、视图和分组 |   |   | ✓ |
| 文档 |   |   | ✓ |
| 用户 |   | ✓ |   |
| 模板 | ✓ |   |   |
| 财务数据 | ✓ |   |   |
| 资源管理 | ✓ |   |   |
| 场景计划器 | ✓ |   |   |
| Workfront 目标 |   |   | ✓（默认设置为“无权访问”。） |

{style=&quot;table-layout:auto&quot;}

## 外部用户访问级别

此访问级别未附加到付费的Workfront许可证。 这是最严格的访问级别，主要面向不登录Workfront，但需要偶尔查看、下载或查看文档的外部顾问等协作者。

Workfront用户可以将任务分配给外部用户，即使外部用户无法登录到系统。 但我们建议不要这么做，因为这项工作在体制内仍有待解决。

具有外部用户访问级别的用户：

* 只能查看与其共享的文档和日历报表
* 查看与其共享文档和日历报表的用户
* 批准与他们共享的文档

您无法修改此访问级别。

>[!IMPORTANT]
>
>仅当在“设置”的“系统首选项”区域中启用了“与没有Workfront帐户的人员通过使用其电子邮件地址进行协作”选项时，“外部用户”才可用。 有关更多信息，请参阅 [配置系统安全首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

以下是外部用户访问级别中对象可用的最高访问设置。

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 | ✓ |   |   |
| 任务 | ✓ | ✓ |   |
| 问题 | ✓ |   |   |
| 项目组合 | ✓ |   |   |
| 项目群 | ✓ |   |   |
| 报表（包括功能板和日历报表） |   | ✓(仅适用于日历报告；无法共享报表) |   |
| 过滤器、视图和分组 | ✓ |   |   |
| 文档 |   | ✓（无法共享文档） |   |
| 用户 |   | ✓ |   |
| 模板 | ✓ |   |   |
| 财务数据 | ✓ |   |   |
| 资源管理 | ✓ |   |   |
| 场景计划器 | ✓ |   |   |
| Workfront 目标 | ✓ |   |   |
