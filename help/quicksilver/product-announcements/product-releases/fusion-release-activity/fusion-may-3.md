---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: “Workfront Fusion版本活动：2021年5月3日一周”
description: 本页介绍2021年5月3日这一周在Adobe Workfront Fusion中所做的所有增强。
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Workfront Fusion版本活动： 2021年5月3日这一周

本页介绍2021年5月3日这一周在Adobe Workfront Fusion中所做的所有增强。

有关所有最近更改的列表，请参阅 [Adobe Workfront Fusion版本活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

有关Workfront Fusion中最近的错误修复列表，请参阅 [Workfront维护更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 页面，并检查标记为Workfront Fusion维护更新的任何更新。

## Salesforce连接器现在可以使用SOQL进行搜索

“Salesforce”>“搜索记录”模块现在可以选择使用SOQL（Salesforce对象查询语言）进行搜索。 您还可以使用以前可用的选项（SOSL和简单搜索）进行搜索。

有关更多信息，请参阅 [Salesforce模块](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Azure DevOps连接器中的新连接类型需要的范围更少

为了增强安全性，我们在Workfront Fusion Azure DevOps连接器中添加了新的连接器类型。 现在，在Azure DevOps模块中创建连接时，可以从两种类型的连接中进行选择：

* Azure DevOps

   此新连接类型将范围限制为Workfront Fusion特别需要的范围。

* Azure DevOps（请求所有作用域）

   这是旧版连接类型，它请求与Azure DevOps连接时所有可用的作用域。

我们建议您在所有使用Azure DevOps的新方案中使用Azure DevOps连接类型。 我们还建议您更改现有方案中的任何Azure DevOps模块，以使用新的连接类型。 不久将弃用旧版Azure DevOps（请求所有作用域）连接类型。

有关更多信息，请参阅 [Azure DevOps模块](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
