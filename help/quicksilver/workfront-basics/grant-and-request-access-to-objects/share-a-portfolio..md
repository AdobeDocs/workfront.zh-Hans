---
title: 共享资产组合
description: 如果您有权访问某个项目组合，则可以与其他用户共享该项目组合。
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: e608cf5bdb0227ea5b8d3109db411e98145aaa38
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---

# 共享资产组合

在分配访问级别时，Adobe Workfront管理员可以授予您查看或编辑项目组合的访问权限。 您必须拥有计划许可证才能访问编辑项目组合。 有关更多信息，请参阅 [授予对项目组合的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

除了授予您的访问级别之外，您还可以从能够与您共享特定项目组合的用户那里接收查看或管理这些项目组合的权限。 有关访问级别和权限的更多信息，请参阅 [访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

权限特定于Workfront中的一个项目，并定义用户可以对该项目执行哪些操作。

## 有关共享项目组合的注意事项

除了以下注意事项外，另请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理员可以添加或删除系统中所有用户的任何项目的权限，而不是这些项目的所有者。

* 默认情况下，组合的创建者具有对其的“管理”权限。
* 您可以单独共享一个项目组合，也可以同时共享多个项目组合。 共享组合与在Workfront中共享其他对象相同。 有关信息，请参阅 [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 您只能授予“查看”或“管理”Portfolio权限。

   ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* 默认情况下，当您共享组合时，用户将继承与组合关联的所有子对象的相同权限。

   有关Workfront中对象层次结构的更多信息，请参阅 [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* 您可以从Portfolio中删除继承的权限。 有关从对象中删除权限的更多信息，请参阅 [从对象删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Portfolio权限

下表显示了在允许用户查看或管理Portfolio时，可以向他们授予哪些权限：

| **操作** | **管理** | **查看** |
|---|---|---|
| 编辑Portfolio详细信息 | ✓ |   |
| 查看Portfolio | ✓ | ✓ |
| 删除Portfolio | ✓ |   |
| 附加自定义表单 | ✓ |   |
| 编辑自定义字段 | ✓ |   |
| 添加或删除程序&#42; | ✓ |   |
| 添加或删除项目&#42; | ✓ |   |
| 批准项目 | ✓ |   |
| Portfolio优化&#42; | ✓ |   |
| 添加文档文件夹&#42; | ✓ | ✓ |
| 添加文档 | ✓ | ✓ |
| 更新/注释 | ✓ | ✓ |
| 共享 | ✓ | ✓ |
| 在系统范围内共享 |   | ✓ |

*这些权限受访问级别和对其他对象（如项目、程序、文档）的权限控制。
