---
title: 2025年第三季度报告增强功能
description: 2025年第三季度项目增强功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 2025年第三季度报告增强功能

本页介绍了在2025年第三季度版本中对“预览”环境所做的所有报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第三季度发布周期中此时可用的所有更改列表，请参阅[2025年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

## 增强报告传送安全性

* 预览：2025年6月26日
* 生产：2025年6月26日至2025年7月9日分阶段推出

我们增强了计划报告交付，以确保仅将Workfront通知发送到在允许列表中批准的电子邮件域。

以前，如果贵组织对哪些电子邮件域Workfront列入允许列表通知定义了限制，我们会在添加电子邮件时对执行检查。

现在，我们还在发送电子邮件时执行检查，以确保输入的电子邮件地址符合电子邮件允许列表。 此改进检查适用于与用户关联的电子邮件地址和添加到报表收件人列表的临时电子邮件。

有关详细信息，请参阅[计划自动报告交付](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。


## 筛选时，用户通配符不再返回空值的结果

>[!NOTE]
>
>* 预览： 2025年4月30日
>* 生产快速发布： 2025年5月15日
>* 适用于所有客户的生产： 2025年7月17日

我们更新了用户通配符行为，以在筛选报告时排除null值。 此更改有助于过滤器生成更准确的结果，而不是返回没有正确配置用户（空结果）的结果。

以前，当用户通配符生成空值时，报告会显示同时具有空值的所有记录。

此更改适用于以下通配符筛选器：

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
