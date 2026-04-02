---
title: 2026年第二季度报表增强功能
description: 2026年第二季度报表增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 64ee7798e79324af0ab48af91f49d04d94ece3a9
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# 2026年第二季度报表增强功能

本页介绍了在2026年第二季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第二季度发布周期中此时可用的所有更改列表，请参阅[2026年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)。

## 在画布功能板中作为特定用户运行报表

>[!NOTE]
>
>预览： 2026年4月2日
>生产快速发布： 2026年4月15日
>适用于所有人的生产： 2026年4月16日
>
>Canvas功能板当前处于Beta版。

您现在可以在画布功能板上将报表配置为以特定用户身份运行。 启用后，报表会根据选定用户的访问权限显示数据，而不是查看者的权限。

即使对Planning工作区、记录类型或授权设置的访问权限不同，这也可以确保跨仪表板查看器的数据更加一致和可靠。

有关详细信息，请参阅[在画布仪表板中生成KPI报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md)、[在画布仪表板中生成图表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)或[在画布仪表板中生成表报告](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md)。

## 计划报表交付现在支持基于链接的电子邮件

>[!NOTE]
>
>预览： 2026年4月2日
>生产快速发布： 2026年4月15日
>适用于所有人的生产： 2026年4月16日

Workfront现在为计划报表提供了新的链接投放类型。 此选项不会生成和附加文件，而是会发送一封电子邮件，其中包含到Workfront中报表的直接链接，从而允许收件人查看应用程序中的最新数据。

链接选项现在是新创建的计划报表投放规则的默认投放类型，而现有的基于文件的格式（HTML、PDF、Excel和TSV）仍可用。

此外，借助这项更改，我们还更新了报告投放电子邮件的外观。

有关详细信息，请参阅[计划自动报告交付](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

## 数据连接连接的新身份验证选项

>[!NOTE]
>
>预览：2026年3月12日
>生产快速发布： 2026年3月12日
>适用于所有人的生产： 2026年4月16日

您现在可以使用RSA密钥或程序化访问令牌(PAT)连接验证数据连接，为传统的用户名/密码凭据添加更安全、更灵活的替代方案。

这些新选项允许组织维护与Power BI、Tableau和其他第三方BI工具的稳定连接，而不依赖于基于用户的登录方法。

>[!IMPORTANT]
>
>2026年6月，使用多重身份验证(MFA)将需要用户名/密码凭据。 我们建议转换到基于RSA或PAT的身份验证模式，服务用户帐户用于将数据从Data Connect加载到第三方可视化工具、数据处理者和脚本中，这些工具在身份验证过程中不适用于MFA。

## 构建报告时显示的自定义字段标签

>[!NOTE]
>
>预览：2026年2月26日
>生产快速发布： 2026年3月12日
>适用于所有人的生产： 2026年4月16日

现在，自定义字段标签显示在报告构建工具中的字段名称和对象之前，这有助于您更轻松地查找字段。 在列表中定义筛选器、视图和分组时，还会显示字段标签。

自定义字段标签适用于系统界面，而字段名称通常用于API和后端存储目的，并且在查找字段时可能没有那么有用。

有关详细信息，请参阅[创建自定义报表](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 可共享报告文件夹

>[!NOTE]
>
>预览：2026年2月26日
>生产快速发布： 2026年3月12日
>适用于所有人的生产： 2026年4月16日

您现在可以使用可共享报告文件夹来组织和共享报告。 此新功能可帮助管理大量报表的团队维护可扩展且一致的访问控制：

* **创建有组织的文件夹结构**：系统管理员可以创建顶层文件夹，具有管理权限的用户可以创建最多4层深的子文件夹。
* **粒度权限控制**：共享具有两个权限级别的文件夹：
   * 查看：用户可以打开报表和共享文件夹
   * 管理：用户可以编辑文件夹详细信息，添加/删除项目，并自动获得对文件夹中所有报表的管理访问权限
* **继承的权限**：权限从父文件夹级联到文件夹树中的所有子文件夹和报告
* **增强型列表体验**：启用可共享文件夹后，您将有权访问增强型列表体验。 有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。


有关详细信息，请参阅[使用可共享报表文件夹](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md)。

## 改进了画布功能板中图表分组的日期标签

>[!NOTE]
>
>预览：2026年2月26日
>生产快速发布： 2026年3月12日
>适用于所有人的生产： 2026年4月16日

>[!NOTE]
>
>Canvas功能板当前处于Beta版。

按日期分组数据的图表现在显示更清晰、更易读的日期标签。 通过此更新，日期标签会根据所选的“分组依据”选项（如日、周、月或年）进行动态调整，使图表更容易阅读和解释：

<table> <tbody> <tr> <td>Day</td> <td>显示完整日期。 示例： 3/12/2026</td> </tr> <tr> <td>周</td> <td>显示已设置好格式的周开始日期。 例如，2026年3月8日</td> </tr> <tr> <td>Month</td> <td>显示月份和年份。 示例2026年3月</td> </tr> <tr> <td>Year</td> <td>仅显示年份。 示例：2026</td> </tr> </tbody> </table>

以前，图表分组始终以数字格式显示选定时段的开始日期。
