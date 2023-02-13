---
title: 访问级别和权限如何协同工作
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，模型，漏斗，图，级别，权限
navigation-topic: access-levels
description: Adobe Workfront管理员确定每个用户应具有的访问级别。 该访问级别定义用户可以查看和处理系统中的对象类型和区域。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 2%

---

# 访问级别和权限如何协同工作

Adobe Workfront管理员确定每个用户应具有的访问级别。 该访问级别定义用户可以查看和处理系统中的对象类型和区域。

此外，当其他用户共享这些对象并授予这些对象的特定权限时，用户也可以访问这些对象。

因此，用户可以对对象执行的操作是通过对象的访问权限级别和为对象授予的权限的组合来定义的。

![](assets/security-model-hierachy.png)

例如，如果访问级别表示您可以创建任务，但您在特定项目上收到的权限不允许您向其添加任务，则即使您可以在Workfront的其他位置创建任务，也无法在项目上添加任务。

本文介绍了此组合的工作方式。

## 访问级别

登录Workfront时，需要由Workfront管理员分配给每个用户的访问级别。

默认访问级别为：

* 系统管理员（附加到计划许可证）
* 计划员（附加到计划许可证）
* 工作人员（附加到工作许可证）
* 审阅人（附加到审阅许可证）
* 请求者（附加到请求许可证）
* 外部用户（附加到外部电子邮件许可证）

每个默认访问级别的Workfront许可证决定了哪些内容在访问级别中可用且可配置。 有关Workfront许可证的信息，请参阅 [Adobe Workfront许可证概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

对于分配到该对象的用户，访问级别定义他们可以查看和处理Workfront中以下对象类型和区域的内容：

* 项目
* 任务
* 问题
* 项目组合
* 报表、功能板和日历
* 过滤器、视图和分组
* 文档
* 其他用户
* 模板
* 财务数据
* 资源管理
* 场景计划器
* Workfront 目标

在自定义访问级别中，您可以配置这些对象和区域的设置，以更改用户对这些对象和区域的访问量。 根据与访问级别关联的许可证以及对象或区域的类型，您可以配置访问级别以允许不访问、查看访问或编辑对对象或区域的访问。

>[!IMPORTANT]
>
>我们强烈建议您保持内置访问级别不变，以便在设置用户后，您可以参考这些级别。 要自定义访问级别，请复制默认访问级别并修改副本。 （除了“系统管理员”和“外部用户”之外，您可以对每个访问级别执行此操作。）

有关每个默认访问级别的详细说明，请参阅 [Adobe Workfront中的内置访问级别](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

有关为用户分配访问级别的说明，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 权限

在与系统中的某人共享对象时，用户可以向收件人授予该对象以下任何权限。

* **查看**:此权限级别允许收件人通过以下方式之一共享对象：

   * 系统范围，以便所有用户都可以查看该对象（并非所有对象都可用）
   * 对于没有Workfront许可证的外部用户（不适用于所有对象）
   * 具有电子邮件地址（仅适用于文档）

* **Contribute**:（不适用于所有对象）
* **管理**:当某人共享某个对象时，收件人对该对象的权限由收件人的访问级别和共享者授予的对象的权限的组合来确定。 组合中可用的最低访问度决定了收件人可以对对象执行的操作。

   >[!INFO]
   >
   >**示例：** 如果收件人的访问级别不允许编辑项目，则即使共享者授予了项目管理权限，该人员也无法编辑或删除项目。
   >
   >或者，如果收件人的访问级别允许编辑项目，但共享者授予了项目的仅查看权限，则用户将无法编辑或删除项目。

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

>[!NOTE]
>
>* 如果用户与某些权限共享某个对象，并且该对象下有任何子对象，则收件人会继承这些子对象的相同权限。
>* 如果访问级别限制用户删除某些对象，则不会阻止用户删除这些对象中包含的子对象。
>


## 更多示例方案

当奥利维亚与托尼分享一个Workfront项目时，托尼的访问权限取决于两件事的组合：

* Tony的访问级别，由Workfront管理员分配
* Tony对项目的权限，由Olivia指定

托尼对项目的行动可能会受到项目的进一步限制，但这些行动不能不受限制，超出他的访问级别所允许的范围：

* 如果Tony的访问级别不允许他创建任务，他将无法向项目添加任务，即使Olivia授予他向项目添加任务的权限。
* 如果Tony的访问级别允许他创建任务，但Olivia没有授予向项目添加任务的权限，他无法向该项目添加任务，但他可以向其他项目添加任务，在其他项目中，他已获得了向该项目添加任务的权限。
