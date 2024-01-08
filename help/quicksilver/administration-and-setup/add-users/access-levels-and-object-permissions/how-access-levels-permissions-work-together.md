---
title: 访问级别和权限如何协同工作
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图表，级别，权限
navigation-topic: access-levels
description: Adobe Workfront管理员可确定每个用户应具有的访问权限级别。 该访问级别定义用户能够查看的对象类型和系统中的区域以及可执行的操作。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 2%

---

# 访问级别和权限如何协同工作

Adobe Workfront管理员可确定每个用户应具有的访问权限级别。 该访问级别定义用户能够查看的对象类型和系统中的区域以及可执行的操作。

此外，当其他用户共享并授予某些对象权限时，用户将获得对这些对象的访问权限。

因此，用户可以针对对象执行的活动由其访问级别和针对该项目授予他们的权限组合来定义。

![](assets/security-model-hierachy.png)

例如，如果您的访问级别表明您可以创建任务，但您获得的特定项目权限不允许您向其中添加任务，则即使您可以在Workfront的其他位置创建任务，也无法向项目添加任务。

本文介绍了此组合的工作原理。

## 访问级别

登录Workfront需要Workfront管理员分配给每个用户的访问级别。

默认访问级别为：

* 系统管理员（附于计划许可证）
* Planner （附加到Plan许可证）
* 工作人员（附加到工作许可证）
* 审阅者（附加到Review许可证）
* 请求者（附在请求许可证上）
* 外部用户（附加到外部电子邮件许可证）

每个默认访问级别的Workfront许可证决定在访问级别中可用和可配置的内容。 有关Workfront许可证的信息，请参阅 [Adobe Workfront许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

对于分配给它的用户，访问级别定义他们能够在Workfront中查看和使用以下对象类型和区域的内容：

* 项目
* 任务
* 问题
* 项目组合
* 报告、功能板和日历
* 筛选器、视图和分组
* 文档
* 其他用户
* 模板
* 财务数据
* 资源管理
* 场景计划器
* Workfront Goals

在自定义访问级别中，您可以配置这些对象和区域的设置，以更改用户对它们的访问量。 根据与访问级别关联的许可证以及对象或区域的类型，您可以将访问级别配置为不允许对对象或区域进行访问、查看访问或编辑访问。

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 (您可以对每个访问级别（系统管理员和外部用户除外）执行此操作。)

有关每个默认访问级别的详细说明，请参阅 [内置访问级别](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

有关为用户分配访问级别的说明，请参阅 [编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 权限

与系统中的某人共享对象时，用户可以向收件人授予对该对象的以下任何权限。

* **视图**：此权限级别允许收件人通过以下方式之一共享对象：

   * 系统范围，以便所有用户都可以查看它（不适用于所有对象）
   * 对于没有Workfront许可证的外部用户（不适用于所有对象）
   * 带有电子邮件地址（仅适用于文档）

* **Contribute**：（并非对所有对象都可用）
* **管理**：当有人共享对象时，收件人对对象的权限由收件人的访问级别和共享者授予的对对象的权限的组合决定。 该组合中可用的最低访问级别决定了收件人可以对对象执行的操作。

  >[!INFO]
  >
  >**示例：** 如果收件人的访问级别不允许编辑项目，则该用户无法编辑或删除项目，即使共享者授予了管理项目的权限也是如此。
  >
  >或者，如果收件人的访问级别允许编辑项目，但共享者授予了项目的仅查看权限，则用户无法编辑或删除项目。

下表将用户对对象的一般访问权限（由用户的访问级别定义）与特定共享对象的权限进行比较：

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
   <td>由Workfront管理员授予用户的访问级别</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>由在对象级别共享对象的用户授予</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td> <p>继承自较高级别的共享对象 
   </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果用户共享具有特定权限的对象，并且该对象在其下具有任何子对象，则收件人将继承这些子对象的相同权限。
>* 如果访问级别限制用户删除某些对象，则不会阻止他们删除这些对象中包含的子对象。
>

## 更多示例场景

当奥利维亚与托尼共享一个Workfront项目时，托尼能否参与该项目取决于两件事：

* Tony的访问级别，由Workfront管理员分配
* 托尼对项目的权限，由Olivia指定

Tony在该项目上的行为可以进一步限制在该项目上，但是不能不受限制地超出其访问级别所允许的限制：

* 如果Tony的访问级别不允许他创建任务，他无法将任务添加到项目，即使Olivia授予他权限将任务添加到项目中。
* 如果Tony的访问级别允许他创建任务，但Olivia未授予将任务添加到项目的权限，他不能将任务添加到该项目，但他可以将任务添加到其他项目，他有权这样做。
