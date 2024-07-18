---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: 更新到emailAddr不会更新用户名
description: 更新emailAddr不会更新用户名
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 更新到emailAddr不会更新用户名

## 问题

通常，`emailAddr`和`username`是同一属性。 因此，如果您更改用户的`emailAddr`属性，`username`属性将自动更新以匹配。

当`username`与`emailAddr`不匹配时，`emailAddr`的更新不会自动更新`username`。 对于通过用户界面和通过API进行的`emailAddr`更改也是如此。

## 原因

可以通过多种方式创建不匹配：

* 在同步规则存在之前创建的用户。 非常旧的用户帐户可能没有同步这些属性。

* 在Workfront中的emailAddr区分大小写，通过SSO创建的用户。 SSO自动预配选项将根据来自身份提供程序的用户的属性，对用户运行区分大小写的检查。 当不存在完全匹配项时，自动资源调配服务将创建一个新用户。 如果用户已经存在，则可能用户名和`emailAddr`没有相同的大小写。

* 直接通过API更新了`username`属性的用户，其`emailAddr`未更新。 `username`和`emailAddr`可能不匹配。

## 解决方案

使用API将`username`属性更改为与`emailAddr`相同。 同步属性后，`emailAddr`的任何更新也将更新`username`以使其匹配（当更新中未包含用户名字段时）。
