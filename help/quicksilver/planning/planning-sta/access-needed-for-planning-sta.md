---
title: Adobe Workfront Planning作为独立产品所需的访问权限
description: 本文介绍Adobe Workfront Planning作为独立产品使用的许可证、访问级别和用户功能。
last-update: 2026-04-01T18:02:40Z
git-commit-file: 8cc175490a6aa1db68b238edbdf9da9da7fbb258
source-git-commit: b186900d58f6a422c787cef881a4d06d6cd7feed
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 2%

---

<!--

Update metadata with this at release:
---
title: Access Required for Planning Standalone
description: This article describes how you can benefit from using the standalone version of Adobe Workfront Planning.
feature: Workfront Planning (******************ask Bob for a new feature???***********)
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->

# Adobe Workfront Planning作为独立产品所需的访问权限

>[!IMPORTANT]
>
>本文中的信息是指Adobe Workfront Planning（作为独立产品购买时）。 当您的公司购买了仅限Adobe Workfront Planning的软件包，但没有购买Workfront Workflow软件包时，请参阅本文。
>
>有关与Adobe Workfront Workflow包一起购买时的Workfront Planning的信息，请参阅[Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)。

本文介绍Adobe Workfront Planning作为独立产品使用的许可证、访问级别和用户功能。

## Workfront规划包

您的组织可以购买以下独立的Workfront Planning包之一：

* Prime
* 选择
* Ultimate

下表描述了每个包中包含的内容：

| 规划功能 | 选择 | Prime | Ultimate |
|---|---|---|---|
| 规划、编排、活动管理 | ✓ | ✓ | ✓ |
| Unlimited工作区 | ✓ | ✓ | ✓ |
| 每个工作区的记录数 | 25,000 | 500,000 | 1,000,000 |
| 记录总数（所有工作区） | 500,000 | 2,000,000 | 无限制 |
| 全局记录类型和跨工作区连接 | — | ✓ | ✓ |
| 在发布时访问未来的功能 | 部分 | 部分 | 最多 |

## Workfront规划包可用性

<!--
the bullets repeat in the "Planning overview" article
-->

当您的组织购买以下Workfront包之一时，即可访问Workfront Planning：

* Workfront Workflow和Workfront Planning一起购买。 组织中的每个用户都有一个Workflow和一个Planning许可证。 这可让所有用户完全访问这两个模块的所有Workfront功能。

* Workfront Workflow适用于贵组织中的每个人，Workfront Planning仅适用于贵组织中的某些用户。 这样，用户就拥有了所有Workflow功能的完全访问权限，而分配了Planning许可证的用户则拥有对Planning功能的更多有限访问权限。

* Workfront Planning作为适用于组织中用户的独立产品。 这样，用户既无法访问任何Workfront工作流功能，也无法访问Planning功能。

有关作为独立产品包含在Planning中的功能的信息，请参阅[作为独立产品开始使用Workfront Planning &#x200B;](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)一文中的“作为独立产品包含在Adobe Workfront Planning中的功能”部分。

## 用户许可证和访问级别

<!-- should this be moved to the Manage users in Planning article??-->

Planning许可证是分配给用户的访问级别的一部分。

对于作为独立产品的Planning，不能将许可证分配给访问级别，这些许可证已经硬编码为包含在分配给用户的访问级别中。

根据组织购买的Workfront Planning包组合，用户可能会具有以下访问级别之一：

* **规划管理员**：可用于Workfront规划包。 将用户添加到Admin Console后，会自动分配Planning管理员。
* **规划标准**：适用于所有Workfront规划包。 您可以在创建用户时为其分配此访问级别。

<!--
this is not available for Planning STA: 
* **Planning Contributor**: Available for the following customers: 

    * Customers that purchase equal amounts of Workflow and Planning packages together. In this case, Planning Contributors have limited access to Planning objects.
    * Customer that purchase unequal amounts of Workflow and Planning packages. In this case, Planning Contributors have read-only access to Planning objects.

-->

每个独立的Planning许可证都映射系统中的角色，并控制产品哪些区域可供访问。

下表说明了作为独立产品购买时，Workfront Planning中的每个Planning许可证类型及其功能：

| 功能/许可证类型 | 规划管理员 | 规划标准 |
|---|---|---|
| 访问级别说明 | 完全系统访问 | 可以管理工作区和内容 |
| 主菜单中的规划区域 | ✔ | ✔ |
| 主菜单中的用户区域 | ✔ | 仅查看 |
| 主菜单中的请求区域 | ✔ | ✔ |
| 主菜单中的设置区域 | ✔ |   |
| 管理工作区及其内容 | ✔ | ✔ |
| 与团队共享Planning数据 | ✔ | ✔ |
| 提交请求 | ✔ | ✔ |
| 创建或编辑用户 | ✔ |   |
| 查看用户列表 | ✔ | 仅查看 |
| 设置>团队 | ✔ |   |
| 设置>登录身份 | ✔ |   |
| 设置>自定义季度 | ✔ |   |
| 设置>系统>客户信息 | ✔ |   |
| 设置>系统>首选项 | ✔ |   |

有关分配用户访问级别的信息，请参阅[作为独立产品在Adobe Workfront Planning中管理用户](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)。

## 导航区域和访问级别依赖关系

根据Planning许可证的不同，用户在其全局导航中可能有不同的可用区域。

<!--
>[!NOTE]
>
>Workfront-specific toolbar actions (Search, Recents, Favorites, Notifications) are not available in the Workfront header for any Standalone user.
-->

### Planning管理员导航概述

<!--
Managing your Adobe Workfront Planning instance is similar to managing an Adobe Workfront with Planning instance, but there are some differences.
-->

具有Planning管理员访问权限级别的用户具有以下权能：

* 具有对系统的完全管理访问权限。
* 可创建和编辑用户、管理团队、配置自定义季度以及访问所有设置子页面。

  有关信息，请参阅：

   * [在Adobe Workfront Planning中作为独立产品管理用户](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)
   * [在Adobe Workfront Planning中将团队作为独立产品进行管理](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)
* 可以提交和管理请求。

  有关信息，请参阅[Adobe Workfront规划请求：文章索引](/help/quicksilver/planning/requests/requests-article-index.md)。
* 在主菜单中有以下区域：

   * **Planning**：具有完整的功能，可创建、删除、共享和连接Planning对象。
   * **用户**：您可以添加用户并编辑其配置文件。
   * **请求**
   * **设置**
* 在“设置”区域包含以下部分：

   * **团队**：您可以添加、删除或编辑团队。 编辑仅限于团队名称、说明和成员；没有可用的筛选器、视图、分组或导出控件。
   * **以**&#x200B;身份登录：模拟其他用户以进行故障排除。
   * **自定义季度**：配置显示在Planning时间线视图中的自定义会计季度。
   * 系统

* 在“System（系统）”区域包含以下部分：

   * **客户信息**：查看客户和组织详细信息。
   * **首选项**：查看和配置系统级别的首选项。

### Planning Standard导航概述

具有Planning标准访问级别的用户具有以下功能：

* 可以管理工作区及其内容。
* 可以提交和管理请求。

  有关信息，请参阅[Adobe Workfront规划请求：文章索引](/help/quicksilver/planning/requests/requests-article-index.md)。
* Planning Standard用户可在主菜单中访问以下区域：

   * **计划**
   * **用户**：他们对用户具有仅查看访问权限。 他们无法创建或编辑用户。<!--not sure if this is still true-->
   * **请求**

* 无权访问“设置”或其任何部分。

## 为Planning配置独立产品的访问级别

当您作为独立产品购买Planning时，访问级别是内置的，并且无法为Planning用户配置它们。

要向用户分配访问级别，请以Planning管理员的身份执行以下操作：

* 在Adobe Console中创建用户。

  存在以下情况：

   * 作为管理员添加到Adobe Console中的用户将在Workfront Planning中获得Planning管理员访问权限级别。
   * 作为用户添加到Adobe Console中的用户，可以在Workfront Planning中为其分配Planning标准访问级别。 这是在Workfront Planning中作为独立产品分配给新用户的唯一可用访问权限。

有关详细信息，请参阅[管理用户](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md)。

## 在Workfront Planning中作为独立产品授予权限

您可以在Workfront Planning中作为独立产品共享以下对象：

* 工作区
* 记录类型
* 记录
* 视图

将对象作为独立产品共享在Planning中与在工作流包一起购买时在Planning中共享它们相同。

有关详细信息，请参阅[Adobe Workfront规划访问信息：文章索引](/help/quicksilver/planning/access/access-information.md)。

<!--

I took this out because there is NO Contributor for true STA: 

### Planning Contributor user experience

>[!IMPORTANT]
>
>Planning Contributor access level is only available for customers that purchase both Workfront Planning and a Workfront Workflow package together. 
>
>If they purchase unequal numbers of packages for the two modules, the Planning Contributor license is read-only. 

When standalone Workfront Planning users purchase a Workflow package, they receive a read-only Planning Contributor license by default. 

For more information, see [Get started with Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

A user with a Planning Standard access level has the following capabilities: 

* View-only access to Planning data, equivalent to the Contributor license in Workfront.
* Can access the following areas in the Main menu:
    * **Planning**
    * **Requests**
* Can submit requests.
* No access to the Users list.
* No access to Setup or any of its sub-pages.

-->

<!-- 
this was moved from the STA general article - some information is already above - take out here what is not needed or add above: 

## Package overview

The following packages are available for Workfront Planning as a standalone product:

* Select
* Prime
* Ultimate

The following table describes what is included in each package:  

| Capability | Select | Prime | Ultimate |
|---|---|---|---|
| Planning, orchestration, campaign management | ✓ | ✓ | ✓ |
| Unlimited workspaces | ✓ | ✓ | ✓ |
| Records per workspace | 25,000 | 500,000 | 1,000,000 |
| Total records (all workspaces) | 500,000 | 2,000,000 | Unlimited |
| Global Record Types and cross-workspace connections | — | ✓ | ✓ |
| Access to future features at release | Some | Some | Most |

## Licensing overview

Consider the following about Workfront Planning licenses:

* Your organization can purchase Workfront Planning licenses without requiring Workfront or Workflow licenses.
* You can add users to Workfront Planning using the Adobe Experience Platform.

    For more information, see [Manage users](/help/quicksilver/planning/planning-sta/manage-users-in-planning-sta.md). 
* Workfront Planning users are limited to Planning-only capabilities and do not receive access to any Workfront areas or capabilities.

The following access levels are hard-coded in Workfront Planning and cannot be modified: 

* Planning Administrator
* Planning Standard 

>[!IMPORTANT]
>
>In a Workfront Planning context, a user must hold a **Planning Standard** license to access the product. 

For more information, see [Access needed for Adobe Workfront Planning as a standalone product](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md). 

## How licensing works for customers with a Planning and Workfront combined package

Consider the following if you have both the Workfront Workflow and Planning packages:

* A Planning Contributor read-only license is available for users in Planning. 
* Any Workfront access level (including Light or Contributor) can be paired with either a Planning Standard or Planning Contributor access level, regardless of the Workfront Workflow license type.

    For example, a user with a Workfront Contributor license can still hold a Planning Standard license and have full Planning management capabilities.

### Mixed License access matrix

When a customer has both Planning and Workfront packages, access levels are determined by the combination below:

| Access Type | Planning License | Workflow License | License Origin |
|---|---|---|---|
| Default | Read Only | Workfront Light | Workfront |
| Default | Read Only | Workfront Standard | Workfront |
| Default | Read Only | Workfront Contributor | Workfront |
| Default | Read Only | Workfront External | Workfront |
| Default | Planning Standard | Workfront Contributor | Planning |
| — | Planning Standard | Workfront Light | Either Planning or Workfront |
| — | Planning Standard | Workfront Standard | Either Planning or Workfront |

Consider the following if your organization has purchased Workfront with Planning:

* Adding a new user to Planning or Workfront automatically creates default (read-only) access in the other product.
* You can upgrade the access in the opposite product. For more information, contact your account representative.

### Upgrading from standalone Planning to a Planning with a Workflow package

#### Workfront Planning with a Workfront Workflow package

When you add a Workfront Planning Standalone package to an existing Workflow license, the following changes take effect automatically:

* Planning Administrators are promoted to System Administrators.
* Non-admin Planning users (Standard and Contributor) receive Workflow Contributor licenses.
* All existing Planning data is preserved.
* All newly provisioned Workfront users are auto-assigned Planning Contributor (read-only) licenses.

#### License mapping when you upgrade to a Planning with Workflow package

| Before (Planning Standalone) | After (Workfront + Planning) |
|---|---|
| Planning Administrator | System Administrator |
| Planning Standard | Workflow Contributor |
| Planning Contributor | Workflow Contributor |

Planning and Workflow licenses remain separate after the upgrade. A Planning Standard user can hold a Workflow Contributor license, and a Planning Contributor user can hold a Workflow Standard license — these are assigned independently based on need.

All users receive an email notification when they gain access to the additional Workflow capabilities in Workfront.

-->

<!--
I took out the last column on this table and added above:

| Feature / Access | Planning Administrator | Planning Standard | Planning Contributor |
|---|---|---|---|
| Access level description | Full system access | Can manage workspaces and content | View-only access to Planning data when Planning packages are in unequal numbers to Workflow licenses. This license is not available for Planning as a standalone product.|
| Planning area in the Main Menu | ✔ | ✔ | ✔ |
| Users area in the Main Menu | ✔ | View only |   |
| Requests area in the Main Menu | ✔ | ✔ | ✔ |
| Setup area in the Main Menu | ✔ |   |   |
| Manage Workspaces and their content | ✔ | ✔ |   |
| Submit requests | ✔ | ✔ | ✔ |
| Create or edit users | ✔ |   |   |
| View users list | ✔ | View only |   |
| Setup > Teams | ✔ |   |   |
| Setup > Log In As | ✔ |   |   |
| Setup > Custom Quarters | ✔ |   |   |
| Setup > System > Customer info | ✔ |   |   |
| Setup > System > Preferences | ✔ |   |   |

-->