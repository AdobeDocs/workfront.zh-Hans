---
title: 22.2资源管理增强
description: 22.2资源管理增强
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2资源管理增强

本页介绍了在“预览”环境中22.2版本中所做的所有资源管理增强。 这些增强功能将在生产环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。

有关2.2版本中可用的所有更改的列表，请参阅 [22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 工作负载平衡器导航的改进

为了改善您在使用工作负载平衡器时的体验，我们引入了以下增强功能：

* 调整分配时的“取消”和“保存”按钮现在具有粘性，即使任务的时间超过了屏幕上包含的时间范围或显示“摘要”面板时也是如此。
* 显示用户和工作项名称的左侧面板现在具有粘性，允许您水平滚动更长的时间范围，并且仍然能够读取面板中列出的项目的名称。
* 只需单击一次，即可折叠和展开左侧面板中列出的所有项目，而不是在用户或项目级别。
* 左侧面板现在也可以调整大小。
* 工作负载平衡器现在有全屏模式。

有关导览工作负载平衡器的详细信息，请参阅 [导航工作负载平衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 访问工作负载平衡器中的高级分配

为了更方便、更准确地分配工作项，现在，在工作负载平衡器中手动分配工作项时，可以进行高级分配。 在此增强之前，您可以在编辑项目、项目标题或列表中访问“高级分配”。

有关更多信息，请参阅 [使用工作负载平衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 在选择“默认计划”首选项时计算用户可用性的新公式

为了在资源管理工具中提供更准确的信息，我们更改了Workfront在Workfront管理员选择资源管理首选项中的默认计划时用于计算用户可用性的公式。 通过新更新，Workfront使用以下公式来计算用户可用性：

用户可用小时数=（默认计划小时数 — 例外） &#42; FTE — 休息时间

在此更新之前，Workfront在选择默认计划时使用以下公式计算用户可用性：

用户可用小时数=(默认计划小时数 — （计划例外+休息时间）) &#42; 用户FTE值

有关更多信息，请参阅 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

