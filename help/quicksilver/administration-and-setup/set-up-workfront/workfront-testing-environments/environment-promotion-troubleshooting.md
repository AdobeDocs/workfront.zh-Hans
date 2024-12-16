---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 环境提升疑难解答
description: 解决环境提升的常见问题。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# 环境提升疑难解答

本文介绍了如何对环境升级问题进行疑难解答。

## 问题：环境升级包停滞或失败

如果您的环境升级包停滞或失败，请尝试以下操作：

* 如果软件包安装在10-15分钟后停止，或者软件包安装失败，请重新组装现有软件包或创建新软件包。

* 如果软件包安装失败，则一个或多个对象可能存在问题。 检查错误消息，该消息可识别对象并帮助识别问题。 解决对象问题后，重新组装软件包并重新尝试安装。

* 如果某个安装仍然存在问题，请尝试在其他目标环境中复制该安装。 尽可能接近原始安装，包括选定的对象和安装操作。

* 我们建议始终在组装软件包后检查软件包内容，以确认它包含您期望的对象。


## 问题：自定义表单无法提升

发生这种情况可能是因为自定义表单包含计算字段。 如果计算字段引用的字段未在自定义表单中引用，则包含此表单的包不会提升，并且用户可能会看到以下消息：

“以下字段无效：自定义表达式无效表达式：自定义表达式无效。”

在引用未附加到目标环境中任何自定义表单的现有字段或新创建的字段时，可能会出现此问题。

要解决此问题，请执行以下操作之一：

* 创建一个项目类型自定义表单包，其中包含引用的字段。 将此包提升到目标环境后，请提升包含计算字段的原始目标包。
* 在目标环境中手动创建引用的字段，并将其与项目类型自定义表单关联。 完成此操作后，字段将被识别，您可以提升包而不会遇到错误。
