---
title: 2026年第三季度报告增强功能
description: 2026年第三季度报告增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 9a86968cf8fff2c7c930aa6c8408ab8566905cb8
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# 2026年第三季度报告增强功能

本页介绍了在2026年第三季度版本中对“预览”环境所做的报表增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## 提高了画布功能板报表中的数据准确性

>[!NOTE]
>
>预览： 2026年5月14日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日
>
>Canvas功能板当前处于Beta版。

画布功能板现在可构建报表查询，以防止过滤器或字段交叉相关记录时显示重复行，这样计数、总和和其他聚合即可返回准确值。

以前，相关记录之间的连接可以为每个相关记录重复一次父记录。 例如，在筛选为分配给特定用户的任务的项目报告中，每个项目都会为每个匹配任务重复一次。 汇总项目预算的KPI可以显示6,000美元，而不是正确的1,250美元。

对画布功能板界面没有更改。 在此版本之后，现有报表会自动返回准确的数据。
