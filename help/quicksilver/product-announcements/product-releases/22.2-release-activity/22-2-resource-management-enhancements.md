---
title: 22.2资源管理增强功能
description: 22.2资源管理增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2资源管理增强功能

本页介绍了22.2版本对“预览”环境所做的所有资源管理增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。

有关22.2版本可用的所有更改列表，请参阅 [22.2发行版概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## 改进了工作负载均衡器导航

为了改进在使用工作负载均衡器时的体验，我们引入以下增强功能：

* 现在，即使任务时间长于屏幕上包含的时间范围或者显示摘要面板，调整分配时的取消和保存按钮都是粘滞的。
* 显示用户名称和工作项的左侧面板现在为“粘性”，可让您水平滚动较长的时间范围，并且仍然能够读取面板中列出的项目名称。
* 只需单击一下即可折叠和展开左侧面板中列出的所有项目，而无需在用户或项目级别单击。
* 现在，左侧面板也可以调整大小。
* 工作负载均衡器现在提供全屏模式。

有关导航工作负载均衡器的更多信息，请参阅 [导航工作负载均衡器](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 在工作负载均衡器中访问高级工作

为了使分配工作项更容易、更准确，现在当在工作负载均衡器中手动分配工作项时，可以进行高级分配。 在此增强功能之前，您可以在编辑项目、项目标题或列表中访问高级工作。

有关更多信息，请参阅 [使用工作负载均衡器手动分配工作](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 选择“默认计划”首选项时用于计算用户可用性的新公式

为了在资源管理工具中提供更准确的信息，我们更改了Workfront管理员在资源管理首选项中选择默认计划时Workfront用于计算用户可用性的公式。 通过新的更新，Workfront使用以下公式计算用户可用性：

用户可用小时数= （默认计划小时数 — 例外） &#42; FTE — 休息时间（小时）

在此更新之前，在选择了“默认计划”时，Workfront使用以下公式计算用户可用性：

用户可用小时数=(默认计划小时数 — （计划例外+休息时间小时数）) &#42; 用户FTE值

有关更多信息，请参阅 [配置资源管理首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

