---
title: 在Adobe大师中共享权限概述
description: 您可以共享或删除AdobeMaestro工作区或视图的权限。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# 在Adobe大师中共享权限概述

{{maestro-important-intro}}

您可以共享或删除AdobeMaestro工作区或视图的权限。

本文介绍Maestro对象的权限级别。

有关如何共享工作区或视图的信息，请参阅以下文章：

* [共享工作区](/help/quicksilver/maestro/access/share-workspaces.md)

* [共享视图](/help/quicksilver/maestro/access/share-views.md)

## 可以在Adobe大师中共享的对象

您可以在Maestro中共享以下对象：

* Workspace

  共享工作区时，也将共享与工作区关联的所有记录类型、记录和字段。 视图不共享。

* 视图

## 关于在Maestro中共享对象的注意事项

* 您必须具有以下许可证才能在Maestro中创建工作区：

   * 新的定价模式：标准许可证
   * 当前定价模型：计划许可证。

  有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* 系统管理员可以管理和共享其他用户创建的工作区。
* 如果您不是系统管理员，则在他人创建的工作区与您共享时，您可以为其贡献内容。
* 您无法批量共享工作区。
* 您可以与以下实体共享工作区：
   * 用户
   * 群组
* 其他用户（包括系统管理员）只能访问他们自己创建的或与他们共享的视图。
* 您可以与其他人共享指向工作区或从记录类型页面查看的链接。 接收链接的用户必须是活动用户，并登录到Workfront才能访问所选视图中显示的工作区或记录类型页面。

## 共享Maestro对象的权限

以下各节中的表说明了在共享Maestro工作区或视图时可以选择的权限级别，以及每个级别允许的功能。

### 工作区权限

|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 编辑 | ✓ {\f13 } |            |       |
| 共享 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } |            |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

### 记录类型权限

向工作区授予权限时，将继承记录类型权限。

|        | 管理 | 参与 | 查看 |
|--------|--------|------------|-------|
| 创建 | ✓ {\f13 } |            |       |
| 删除 | ✓ {\f13 } |            |       |
| 编辑 | ✓ {\f13 } |            |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } | ✓ {\f13 } |

### 记录权限

向工作区授予权限时，将继承记录权限。

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

|        | 管理 | 查看 |
|--------|--------|-------|
| 编辑 | ✓ {\f13 } |       |
| 删除 | ✓ {\f13 } |       |
| 查看 | ✓ {\f13 } | ✓ {\f13 } |
| 应用 | ✓ {\f13 } | ✓ {\f13 } |






