---
title: 共享报告、功能板和日历
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: 当用户分配访问级别时，您的Adobe Workfront管理员会授予他们查看或编辑报告、功能板和日历的访问权限。 有关授予对报表、功能板和日历的访问权限的更多信息，请参阅授予对报表、功能板和日历的访问权限。
author: Courtney
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 共享报告、功能板和日历

当用户分配访问级别时，您的Adobe Workfront管理员会授予他们查看或编辑报告、功能板和日历的访问权限。 有关授予对报告、仪表板和日历的访问权限的详细信息，请参阅[授予对报告、仪表板和日历的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定报告、功能板或日历的权限。 有关授予用户共享对象权限的信息，请参阅[共享对象权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。

有关每个访问级别中的用户可以如何处理问题的信息，请参阅[适用于每个对象类型的功能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports)一文中的[报告](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)部分。

## 有关共享报表、功能板或日历的注意事项

除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

* 默认情况下，报表、功能板或日历的创建者具有管理权限。
* 共享报告、功能板和日历与在Workfront中共享任何其他对象类似。

  有关如何在Workfront中共享对象的详细信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

  另请参阅以下文章，了解如何共享报告、功能板和日历：

   * [在Adobe Workfront中共享报告](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共享仪表板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共享日历报告](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* 您可以单独共享报告和仪表板，也可以批量共享它们。

  只能单独共享日历。 不能批量共享它们。

* 您无法共享内置系统报告。 您只能共享自定义报表。

  有关将系统报告另存为新的自定义报告的详细信息，请参阅[创建报告副本](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md)。

* 您可以向报表、功能板和日历授予以下权限：

   * 视图
   * 管理

* 共享功能板时，用户默认对功能板上的所有报告、日历和外部页面具有查看权限。
* 具有“请求”许可证的用户无法查看系统范围的报告。 如果请求者需要查看报告，则必须单独与请求者共享报告。
* 如果报告有提示并且您公开共享它，则访问报告的用户必须登录到Workfront才能使用提示运行报告。 如果他们无法登录Workfront，将看到未应用提示的报告。\
  有关共享带有提示的报告限制的更多信息，请参阅文章[向报告添加提示](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)中的[共享提示报告的限制](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)部分。

* 您可以从报表或日历中删除继承的权限。

  有关从对象中删除继承权限的详细信息，请参阅[从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

* 您还可以公开或在系统范围内共享报表或日历。

  您无法公开共享仪表板，但可以在系统范围内共享仪表板。

  >[!CAUTION]
  >
  >建议在与外部用户共享包含机密信息的对象时务必谨慎。 这样，他们便可以查看信息，而无需成为Workfront用户或您组织的一部分。
