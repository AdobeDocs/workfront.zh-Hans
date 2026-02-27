---
title: 2026年第二季度报表增强功能
description: 2026年第二季度报表增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
source-git-commit: aceb9f7bd6c62036838b15d74ee2a9b7843e5c11
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 2026年第二季度报表增强功能

本页介绍了在2026年第二季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第二季度发布周期中此时可用的所有更改列表，请参阅[2026年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)。

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
