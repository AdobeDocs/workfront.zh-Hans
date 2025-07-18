---
title: 在Adobe Workfront Planning中共享权限概述
description: 并非组织中的所有用户都具有相同的访问权限和权限来使用Adobe Workfront Planning。 本文介绍了有关共享或删除Adobe Workfront Planning工作区或视图的权限的一般信息。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 5%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# 在Adobe Workfront Planning中共享权限概述

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

您可以共享或删除Adobe Workfront Planning工作区、记录类型或视图的权限。

您还可以共享Planning请求表单。 有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。

本文介绍Workfront Planning工作区、记录类型、记录、字段和视图的权限级别。

## 可在Adobe Workfront Planning中共享的对象

您可以手动共享某些Workfront Planning对象，而其他对象会从其他对象继承这些权限。

您可以在Workfront Planning中手动共享以下对象：

* Workspace

   * 您可以与组织内的人员共享工作区。
   * 共享工作区时，也将共享与工作区关联的所有记录类型、记录和字段。
   * 共享工作区时，视图不共享。 视图将单独共享。

  有关详细信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

* 记录类型

   * 您可以与组织内部人员共享记录类型。
   * 授予工作区的权限级别显示为记录类型的继承权限。
   * 您无法以高于用户在工作区中的权限级别共享记录类型。

  有关详细信息，请参阅[共享记录类型](/help/quicksilver/planning/access/share-record-types.md)。


* 视图

   * 您必须向用户（包括系统管理员）授予单独访问视图的权限和访问工作区的权限。
   * 共享视图时，将共享所有视图元素，包括筛选器、分组、排序或设置。
   * 共享视图时，不会共享该视图中可见的记录。 必须通过共享工作区来共享记录。
   * 在为视图生成公共链接时，您可以与组织外部的人员公开共享视图。通过公共链接访问记录页面的人员可以查看所有记录及其字段，包括连接的记录和字段。

  有关详细信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。

在内部，您可以与以下Workfront实体共享工作区、视图或记录类型：

* 用户
* 组
* 团队
* 公司
* 工作角色

当您与他人共享工作区和记录类型时，记录类型中的权限级别会自动继承到与其关联的记录和字段。

>[!IMPORTANT]
>
>如果您组织的Workfront实例已载入到Adobe Unified Experience，则必须将要与共享Planning对象的用户添加到Adobe Admin Console。 您无法与尚未添加到Adobe Admin Console的Workfront用户共享Planning对象。


## 关于在Adobe Workfront Planning中共享对象的注意事项

* 您的Adobe Workfront许可证类型与Workfront Planning权限配合使用，允许您查看、贡献或管理工作区及其对象。

  有关许可证类型如何影响Workfront Planning权限级别的信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。
* 系统管理员可以管理系统中的所有工作区，包括他们未创建的工作区。
* 其他用户（包括系统管理员）只能访问他们自己创建的或与他们共享的视图。 只能向系统管理员授予管理视图的权限。
* 您可以与他人共享指向工作区或视图的链接。

  存在以下情况：
   * 接收工作区链接的用户必须是活动用户并登录到Workfront才能访问工作区。
   * 收到视图链接的用户可以通过以下方式访问该视图：

      * 如果指向视图的链接在内部共享，则必须是活动用户并登录到Workfront。
      * 可以是Workfront的外部用户，无需登录到Workfront即可从公共共享链接访问视图。

## 共享Adobe Workfront Planning对象的权限

以下各节中的表说明了在共享工作区或视图时可以选择哪些权限级别，以及每个级别允许哪些功能。

>[!IMPORTANT]
>
>并非所有用户都可以具有下述权限级别。 用户的个人许可证确定他们可针对Workfront Planning对象接收的权限级别。
>
>只有标准（或计划）许可证用户可以拥有工作区的“贡献”或“管理”权限以及视图的“管理”权限。
> 
>具有所有其他许可证类型的用户都可以拥有对工作区和视图的查看权限。
>
>有关信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。


### 工作区的权限

您必须向用户授予工作区权限，以便他们能够访问以下实体：

* Workspace
* 记录类型
* 记录
* 字段

以下是工作区的权限级别：

|        | 管理 | 贡献 | 查看 |
|--------|--------|------------|-------|
| 编辑 | ✓ |            |       |
| 共享 | ✓ |            |       |
| 删除 | ✓ |            |       |
| 查看 | ✓ | ✓ | ✓ |

### 记录类型的权限

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

向工作区授予权限时，始终会继承记录类型权限。

您可以删除从工作区接收的记录类型的继承权限。

您可以授予用户在记录类型上比他们在工作区上更低的权限。

但是，您不能执行以下操作：

* 授予记录类型比用户在工作区上更高的权限。
* 为工作区经理提供较低记录类型权限。
* 通过从记录类型权限中删除用户，删除对记录类型或工作区的查看权限。

存在以下情况：

| Workspace权限 | 记录类型的自动继承权限 | 关闭继承权限时可能的记录类型权限（手动授予） |
|--------|--------|-------------|
| 管理 | 管理 | 管理，删除权限* |
| 贡献 | 贡献 | Contribute、View、Remove权限* |
| 查看 | 查看 | 查看，删除权限* |

>[!NOTE]
>
>*当您从记录类型中删除权限时，用户仍保留对工作区和所有记录类型的“查看”权限，除非您从工作区中删除其权限。

### 记录的权限

向工作区和记录类型授予权限时，记录权限继承自记录类型。

以下是记录的权限级别：


|        | 管理 | 贡献 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ | ✓ |       |
| 删除 | ✓ | ✓ |       |
| 编辑 | ✓ | ✓ |       |
| 查看 | ✓ | ✓ | ✓ |

### 记录字段的权限

向工作区和记录类型授予权限时，字段权限继承自记录类型。

以下权限是指字段本身，而不是与每个字段关联的值。 要编辑字段值，您必须具有编辑记录的权限。

|        | 管理 | 贡献 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ |            |       |
| 删除 | ✓ |            |       |
| 编辑 | ✓ |            |       |
| 查看 | ✓ | ✓ | ✓ |


### 查看权限

您必须授予单独的权限以记录视图。 向工作区授予权限不会向工作区中的记录视图授予权限。

您必须授予用户查看权限，以便他们能够访问以下视图元素：

* 过滤器
* 字段可见性
* 排序
* 分组
* 行高
* 设置

您可以在内部或公开共享视图。

以下是视图和视图元素的权限级别：

| 内部共享 | 管理（只有受邀人员才能访问） | 查看（只有受邀人员才能访问） | 工作区中的每个人都可以查看* |
|--------|--------|-------|------------------------------|
| 编辑 | ✓ |       |                            |
| 删除 | ✓ |       |                            |
| 共享 | ✓ |       |                           |
| 查看 | ✓ | ✓ | ✓ |
| 应用 | ✓ | ✓ | ✓ |

| 公开共享 | 查看 |
|--------|-------|
| 查看 | ✓ |
| 应用 | ✓ |

*用户必须具有工作区的“查看”或更高权限才能获得此查看访问权限。

<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->
