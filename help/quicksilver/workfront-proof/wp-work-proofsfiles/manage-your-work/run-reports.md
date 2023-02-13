---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中运行报表 [!DNL Workfront Proof]
description: Workfront Proof让您能够查看报表，以便跟踪团队的工作进度和效率。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 在中运行报表 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

Workfront Proof让您能够查看报表，以便跟踪团队的工作进度和效率。

您可以轻松查看在 [!DNL Workfront Proof] 帐户、与每个校样关联的版本数、周转时间等。

## 先决条件

报表是否可用取决于您的 [!DNL Workfront Proof] 帐户和用户权限级别。

* [帐户先决条件](#account-prerequisites)
* [用户先决条件](#user-prerequisites)

### 帐户先决条件 {#account-prerequisites}

报表信息仅在Premium计划中可用。

### 用户先决条件 {#user-prerequisites}

报表信息仅适用于拥有您帐户上所有校样的完全访问权限的用户(即至少具有 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))。

在此面板中，您可以

* 控制显示数据的时间范围
* 分析量度随时间的变化
* 通过将鼠标悬停在选定时间点上来检查其详细信息
* 检查在选定时间范围内创建的校样总数
* 检查已完成校样集中包含的平均版本数

## 查看报表 {#viewing-reports}

1. 转到 **[!UICONTROL 功能板]** 页面。
1. 单击 **[!UICONTROL 报表]** 选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 在 **[!UICONTROL 时间范围]** 下拉菜单中，选择是要显示有关过去24小时、7天、30天、90天或自定义时间段内创建的校样的信息。\
   如果选择自定义时间段，请选择开始和结束日期，然后单击 **[!UICONTROL 应用]**.\
   将显示选定时段的以下信息：\
   **创建校样：** 在选定时间段内创建的校样数。\
   **每个校样的版本：** 选定时间段内所有已完成校样（已批准或已批准更改）的每次校样的平均版本数。\
   **返回时间：** 从创建第一个版本到对最终版本作出决定的平均时间。\
   **首次活动时间：** 从创建校样到进行校样上首次活动的平均时间。\
   **延迟校样：** 至少有一个版本在选定时间段内延迟的已完成校样（已批准或已批准更改）的平均百分比。\
   **评论和回复：** 在选定时间段内对所有校样发表的评论和回复的平均数。

1. （可选）选择或取消选择 **[!UICONTROL 显示最小 — 最大范围]** 用于确定图表中是否显示最小值和最大值的选项。\
   如果选择此选项，则最小和最大记录值之间将显示蓝色底纹。

1. （可选）您可以过滤显示的数据，如 [过滤报表](#filtering-reports).

## 过滤报表 {#filtering-reports}

默认情况下，报表中显示的数据包含 [!DNL Workfront Proof] 系统。 您可以使用过滤器仅显示与您的需求相关的信息。

要过滤报表信息，请执行以下操作：

1. 转到 **[!UICONTROL 功能板]** 页面。
1. 单击 **[!UICONTROL 报表]** 选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 运行报表，如 [查看报表](#viewing-reports).
1. 单击 **[!UICONTROL 过滤器]**.

1. 在页面的左侧，从以下过滤器选项中进行选择：\
   **[!UICONTROL 校样类型]:** 选择要包含在报表中的校样类型。\
   **[!UICONTROL 决策]:** 选择选项以确定是否只做出了包含特定决策的校样。\
   **[!UICONTROL 收件人]:** 选择单个用户可查看与与选定用户共享的校样相关的信息。\
   **[!UICONTROL 校样所有者]:** 选择个人用户可查看与所选用户拥有的校样相关的信息。\
   **[!UICONTROL 校样创建者]:** 选择单个用户可查看与选定用户创建的校样相关的信息。\
   **[!UICONTROL 帐户]:** 选择要包含在报表中的帐户。

1. 单击 **[!UICONTROL 应用]**.
1. （可选）选择或取消选择 **[!UICONTROL 显示最小 — 最大范围]** 用于确定图表中是否显示最小值和最大值的选项。\
   如果选择此选项，则最小和最大记录值之间将显示蓝色底纹。

## 打印报表

1. 转到 **[!UICONTROL 功能板]** 页面。
1. 单击 **[!UICONTROL 报表]** ，然后单击 **[!UICONTROL 打印]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. 从可用的各种打印选项中进行选择。\
   打印选项因您使用的浏览器和浏览器版本而异。
