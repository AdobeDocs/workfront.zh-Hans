---
title: Workfront Fusion版本活动：&nbsp;2021年8月30日的一周
description: Workfront Fusion版本活动：&nbsp;2021年8月30日的一周
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Workfront Fusion版本活动： 2021年8月30日这一周

本页介绍2021年8月30日这一周Adobe Workfront Fusion中所有增强功能。

有关所有最近更改的列表，请参阅 [Adobe Workfront Fusion版本活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

有关Workfront Fusion中最近的错误修复列表，请参阅 [Workfront维护更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) 页面，并检查标记为Workfront Fusion维护更新的任何更新。

## 过滤触发Workfront >监视事件模块的事件

1. 为触发Workfront >监视事件模块的事件设置自定义过滤器

   为了减少不必要的方案运行次数，我们更新了Workfront >监视记录模块以启用事件过滤。 现在，您可以在创建网页挂接时设置过滤器。 这允许方案仅在事件满足特定条件时才触发。

   事件过滤器当前提供以下操作：

   * 等于：仅当事件与过滤器的条件匹配时才会触发方案。 例如，您可以设置一个过滤器，该过滤器仅在特定项目中发生事件时才触发方案。
   * 不等于：仅当事件与过滤器的条件不匹配时才会触发方案。 例如，您可以创建一个过滤器，该过滤器仅在发生事件的问题没有状态为“已关闭”时触发方案。

   以前，监视记录模块将检索所有记录。 用户只能在以后的方案中设置过滤器来过滤。

   要利用事件过滤，请在Watch事件模块中新建一个Webhook。 当前无法编辑现有Web挂接以包含此功能。 我们强烈建议您使用事件过滤器为现有方案创建新的Webhook。

1. 过滤掉由当前连接触发的事件。

   为了更便于为Workfront >监视事件模块设置Web挂接，我们提供了最常见的事件过滤器。 现在， Webhook具有一个选项，用于使用为Watch事件模块指定的连接过滤掉模块所做的任何更改。 换言之，启用此过滤器后，由与该连接关联的Workfront用户所做的任何更改都无法触发该方案。

   以前，此过滤器不可用。 因此，在Workfront模块中所做的更改更容易触发包含这些模块的方案，这可能会导致方案在无限循环中触发自己。

有关Workfront >监视事件模块中的事件过滤器的更多信息，请参阅 [Adobe Workfront模块](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

