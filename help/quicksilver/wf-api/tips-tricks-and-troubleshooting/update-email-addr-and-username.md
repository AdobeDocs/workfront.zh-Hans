---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: 更新emailAddr时不会更新用户名
description: 更新emailAddr时不会更新用户名
author: John
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: a939e14cbd6936bdd0c46c1ed641acdda497b8fc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 更新emailAddr时不会更新用户名

## 问题

通常， `emailAddr` 和 `username` 属性相同。 因此，如果您更改了 `emailAddr` 属性 `username` 属性会自动更新以匹配。

当 `username` 不匹配 `emailAddr`，更新 `emailAddr` 不更新 `username` 自动。 这两种情况均适用 `emailAddr` 通过用户界面和API进行更改。

## 原因

可能会通过以下几种方式造成不匹配：

* 同步规则存在之前创建的用户。 非常旧的用户帐户可能没有这些属性同步。

* 在Workfront中的emailAddr区分大小写时，通过SSO创建的用户。 SSO自动配置选项将根据身份提供者中用户的属性，对用户运行区分大小写的检查。 当不存在完全匹配项时，自动配置服务将创建新用户。 如果用户已存在，则用户名和 `emailAddr` 不会有同一个外壳。

* 具有 `username` 属性直接通过API更新，并且 `emailAddr` 未更新。 的 `username` 和 `emailAddr` 可能不匹配。

## 解决方案

使用API更改 `username` 属性与 `emailAddr`. 在同步属性后，对 `emailAddr` 还将更新 `username` 匹配（当更新中未包含用户名字段时）。
