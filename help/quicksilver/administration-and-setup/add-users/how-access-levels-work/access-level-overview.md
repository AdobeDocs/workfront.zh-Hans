---
title: 新访问级别概述
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，级别，系统，管理员，标准，轻量级，参与者
navigation-topic: access-levels
description: 每个用户必须具有访问级别，才能登录并在Workfront中工作。 您可以使用访问级别控制用户可以查看和处理某些Workfront对象和区域的内容。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 26da544bb8cd833d37dd6a484687495fde5060b1
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 4%

---

# 新访问级别概述

作为Adobe Workfront管理员，您可以为用户分配访问级别，具体用途如下：

* 每个用户必须具有访问级别，才能登录并在Workfront中工作。
* 您可以使用访问级别控制用户可以查看和处理某些Workfront对象和区域的内容。

## Adobe Workfront中新的内置访问级别 {#built-in-access}

Workfront具有5个新的内置访问级别：

* 系统管理员
* 标准
* 浅色
* 投稿人
* 外部的

根据访问级别，大多数Workfront对象类型最多有3个权限：

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

如果您需要自定义访问级别，则可以复制内置访问级别并调整您希望它允许的各种Workfront对象类型的访问量。 有关创建自定义访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后，您可以参考这些级别。

### 系统管理员访问级别

此内置访问级别附加到标准许可证，专为负责管理Adobe Workfront系统的用户而设计。 您无法修改此内置访问级别。

具有系统管理员访问权限级别的用户可以在Workfront中执行所有操作。 他们可以查看和编辑所有其他用户在Workfront中输入的所有Workfront对象和信息。

他们还可以访问完整的“设置”区域，在该区域中，他们可以更改系统级别的任何设置，并可以访问“主菜单”中的所有区域。

有关更多信息，请参阅 [授予用户完全管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### 标准访问级别

此访问级别也附加到标准许可证，专为以下用户设计：

* 在一个位置规划、创建和跟踪所有项目
* 自动化日常流程
* 管理资源
* 跟踪和协作请求
* 跟踪和报告项目财务
* 启动入站工作请求
* 协作处理项目、任务和问题

>[!NOTE]
>
>您可以创建标准内置访问级别的自定义版本，并调整它允许各种Workfront对象类型的访问量。 有关创建自定义访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **访问详细信息**

以下是标准访问级别中对象可用的最高访问设置：

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
| 展示板 |   |   | ✓ |
| 主页 |   |   | ✓ |
| 目标 |   |   | ✓ |

{style="table-layout:auto"}

### 轻量级

此访问级别附加到Light许可证，适用于以下用户：

* 查看与工作关联的所有项目和更新
* 批准项目、任务和问题
* 查看功能板和报表
* 跟踪时间
* 创建和管理问题
* 更新工作

具有轻量级访问级别的用户：

* 无法分配工作项或批准工时单
* 可以在主菜单中访问请求和文档。
* 创建对象的能力有限 — 无法创建项目、项目组合、项目或报告。

>[!NOTE]
>
>您可以创建Light内置访问级别的自定义版本，并调整它允许各种Workfront对象类型的访问量。 有关创建自定义访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **访问详细信息**

以下是“浅访问”级别中对象可用的最高访问设置：

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
   <td>✓（默认设置为“无权访问”。）</td> 
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
   <td>团队</td> 
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
   <td>✓</td> 
   <td> <p> </p> </td> 
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
   <td>展示板 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>主页 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>目标 </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### 参与者访问级别

此访问级别附加到参与者许可证，专为以下用户而设计：

* 提交请求
* 跟踪请求
* 更新和查看请求。

具有此内置访问级别的用户：

* 可以发出请求并更新这些请求
* 可以上传和批准文档
* 可以查看他们提交的问题的状态
* 无法分配给工作项
* 只能从主菜单访问请求。 有关请求队列的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>您可以创建参与者内置访问级别的自定义版本，并调整它允许各种Workfront对象类型的访问量。 有关创建自定义访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **访问详细信息**

以下是参与者访问级别中对象可用的最高访问设置：

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 |   | ✓（仅“项目详细信息”页面） |   |
| 任务 |   | ✓（仅详细信息页面） |   |
| 问题 |   |   | ✓ |
| 项目组合 | ✓ |   |   |
| 项目群 | ✓ |   |   |
| 报表（包括功能板和日历报表） |   | ✓（仅“详细信息”选项卡） |   |
| 过滤器、视图和分组 |   |   | ✓ |
| 文档 |   |   | ✓ |
| 用户 |   | ✓ |   |
| 团队 |   | ✓ |   |
| 模板 | ✓ |   |   |
| 财务数据 | ✓ |   |   |
| 资源管理 | ✓ |   |   |
| 场景计划器 | ✓ |   |   |
| 展示板 |   |   | ✓（简单卡片） |
| 主页 |   | ✓（我的更新） |   |
| 目标 |   |   | ✓ |

{style="table-layout:auto"}

### 外部用户访问级别

此访问级别未附加到付费的Workfront许可证。 这是最严格的访问级别，主要面向不登录Workfront但需要偶尔查看、下载或查看文档的外部顾问等协作者。

Workfront用户可以将任务分配给外部用户，即使外部用户无法登录到系统。 但我们建议不要这么做，因为这项工作在体制内仍有待解决。

具有外部用户访问级别的用户：

* 只能查看与其共享的文档和日历报表
* 查看与其共享文档和日历报表的用户
* 批准与他们共享的文档

您无法修改此访问级别。

>[!IMPORTANT]
>
>仅当在“设置”的“系统首选项”区域中启用了“与没有Workfront帐户的人员通过使用其电子邮件地址进行协作”选项时，“外部用户”才可用。 有关更多信息，请参阅 [配置系统安全首选项](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **访问详细信息**

以下是外部用户访问级别中对象可用的最高访问设置。

| Workfront对象类型 | 无权访问 | 查看访问 | 编辑访问权限 |
|---|---|---|---|
| 项目 | ✓ |   |   |
| 任务 | ✓ |   |   |
| 问题 | ✓ |   |   |
| 项目组合 | ✓ |   |   |
| 项目群 | ✓ |   |   |
| 报表（包括功能板和日历报表） |   | ✓(仅适用于日历报告；无法共享报表) |   |
| 过滤器、视图和分组 | ✓ |   |   |
| 文档 |   | ✓（无法共享文档） |   |
| 用户 |   | ✓ |   |
| 团队 | ✓ |   |   |
| 模板 | ✓ |   |   |
| 财务数据 | ✓ |   |   |
| 资源管理 | ✓ |   |   |
| 场景计划器 | ✓ |   |   |
| 展示板 | ✓ |   |   |
| 主页 | ✓ |   |   |
| 目标 | ✓ |   |   |


## 访问级别和权限如何协同工作

访问级别定义用户可以查看和处理系统中一般对象类型和区域（如项目、任务和问题）的内容。 权限定义您有权访问系统中其他人创建的特定对象（如为运行营销活动而创建的项目）。

下表将用户对对象的常规访问（由用户的访问级别定义）与特定共享对象的权限进行比较：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>访问级别 </th> 
   <th>权限 </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>由Workfront管理员在用户的访问级别中授予</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>由在对象级别共享对象的用户授予</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>继承自排名较高的共享对象 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

用户可以对对象执行的活动，由其访问级别和授予其权限的组合来定义。

![](assets/security-model-hierachy-copy.png)

### 通过共享对象授予权限

当其他用户共享这些对象并授予这些对象的特定权限时，用户即可获得对这些对象的访问权限。

>[!NOTE]
>
>* 如果用户与某些权限共享某个对象，并且该对象下有任何子对象，则收件人会继承这些子对象的相同权限。
>* 如果访问级别限制用户删除某些对象，则不会阻止用户删除这些对象中包含的子对象。


用户可以向收件人授予单个对象以下任何权限：

* **查看**:此权限级别允许收件人通过以下方式之一共享对象：

   * 系统范围，以便所有用户都可以查看该对象（并非所有对象都可用）
   * 对于没有Workfront许可证的外部用户（不适用于所有对象）
   * 具有电子邮件地址（仅适用于文档和日历）

* **Contribute**:（不适用于所有对象）
* **管理**:当某人共享某个对象时，收件人对该对象的权限由收件人的访问级别和共享者授予的对象的权限的组合来确定。 组合中可用的最低访问度决定了收件人可以对对象执行的操作。

### 示例方案

#### **场景1**

如果收件人的访问级别不允许编辑项目，则即使共享者授予了项目管理权限，该人员也无法编辑或删除项目。

或者，如果收件人的访问级别允许编辑项目，但共享者授予了项目的仅查看权限，则用户将无法编辑或删除项目。

#### **场景2**

当奥利维亚与托尼分享一个Workfront项目时，托尼的访问权限取决于两件事的组合：

* Tony的访问级别，由Workfront管理员分配
* Tony对项目的权限，由Olivia指定

托尼对项目的行动可能会受到项目的进一步限制，但这些行动不能不受限制，超出他的访问级别所允许的范围：

* 如果Tony的访问级别不允许他创建任务，他将无法向项目添加任务，即使Olivia授予他向项目添加任务的权限。
* 如果Tony的访问级别允许他创建任务，但Olivia没有授予向项目添加任务的权限，他无法向该项目添加任务，但他可以向其他项目添加任务，在其他项目中，他已获得了向该项目添加任务的权限。
