---
title: 在Adobe Workfront Planning中共享权限概述
description: 您可以共享或删除Adobe Workfront Planning工作区或视图的权限。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 6%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# 在Adobe Workfront Planning中共享权限概述

{{planning-important-intro}}

您可以在Adobe Workfront Planning中共享或删除对工作区或视图的权限。

本文介绍了Workfront Planning对象的权限级别。

有关如何共享工作区或视图的信息，请参阅以下文章：

* [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

* [共享视图](/help/quicksilver/planning/access/share-views.md)

## 可在Adobe Workfront Planning中共享的对象

您可以共享以下对象：

* Workspace

   * 您可以与组织内的人员共享工作区。
   * 共享工作区时，也将共享与工作区关联的所有记录类型、记录和字段。 视图不共享。

* 视图

   * 您必须向用户（包括系统管理员）授予单独访问视图的权限以及访问工作区的权限。
   * 在为视图生成公共链接时，您可以与组织外部的人员公开共享视图。通过公共链接访问记录页面的人员可以查看所有记录及其字段，包括连接的记录和字段。

  有关信息，请参阅[共享视图](/help/quicksilver/planning/access/share-views.md)。

在内部，您可以与以下Workfront实体共享工作区或视图：

* 用户
* 组

## 关于在Adobe Workfront Planning中共享对象的注意事项

* 您的Adobe Workfront许可证类型与Workfront Planning权限配合使用，允许您查看、贡献或管理工作区及其对象。

  有关许可证类型如何影响Workfront Planning权限级别的信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。
* 系统管理员可以管理系统中的所有工作区，包括他们未创建的工作区。
* 其他用户（包括系统管理员）只能访问他们自己创建的或与他们共享的视图。 系统管理员只能获得管理视图的权限。
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
>只有Standard（或Plan）许可证用户可以拥有Contribute或工作区的“管理”权限以及视图的“管理”权限。
> 
>具有所有其他许可证类型的用户都可以拥有对工作区和视图的查看权限。
>
>有关信息，请参阅[使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)。


### Workspace权限

您必须向用户授予工作区权限，以便他们能够访问以下实体：

* Workspace
* 记录类型
* 记录
* 字段

以下是工作区的权限级别：

|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 编辑 | ✓ {\f13 } |            |       |
| 共享 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } |            |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

### 记录类型权限

向工作区授予权限时，将继承记录类型权限。

以下是记录类型的权限级别：


|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } |            |       |
| 编辑 | ✓ {\f13 } |            |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

### 记录权限

向工作区授予权限时，将继承记录权限。

以下是记录的权限级别：


|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } | ✓ {\f13 } |       |
| 编辑 | ✓ {\f13 } | ✓ {\f13 } |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

### 字段权限

向工作区授予权限时，将继承字段权限。
以下权限是指字段本身，而不是与每个字段关联的值。 要编辑字段值，您必须具有编辑记录的权限。

|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } |            |       |
| 编辑 | ✓ {\f13 } |            |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |


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
| 编辑 | ✓ {\f13 } |       |                            |
| 删除 | ✓ {\f13 } |       |                            |
| 共享 | ✓ {\f13 } |       |                           |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |
| 应用 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

| 公开共享 | 查看 |
|--------|-------|
| 查看 | ✓ {\f13 } |
| 应用 | ✓ {\f13 } |

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