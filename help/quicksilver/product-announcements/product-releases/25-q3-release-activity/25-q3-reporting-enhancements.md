---
title: 2025年第三季度报告增强功能
description: 2025年第三季度项目增强功能
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 2025年第三季度报告增强功能

本页介绍了在2025年第三季度版本中对“预览”环境所做的所有报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2025年第三季度发布周期中此时可用的所有更改列表，请参阅[2025年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)。

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

