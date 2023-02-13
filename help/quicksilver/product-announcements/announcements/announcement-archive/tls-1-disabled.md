---
content-type: reference
navigation-topic: announcements
title: Adobe Workfront中需要使用TLS 1.2
description: 为了提供最佳安全性，Adobe Workfront要求升级所有依赖TLS 1.0或更早版本的浏览器连接和API集成，以使用TLS 1.2。在“预览”环境中，TLS 1.0已被禁用。
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Adobe Workfront中需要使用TLS 1.2

为了提供最佳安全性，Adobe Workfront要求升级所有依赖TLS 1.0或更早版本的浏览器连接和API集成，才能使用TLS 1.2。 在预览环境中，TLS 1.0已被禁用。

Workfront已于2018年3月正式终止对TLS 1.0的支持。 自2019年1月9日起，使用TLS 1.0的所有集成都将停止运行。  TLS 1.1将在2019年第4季度禁用。

以下部分提供了有关这些重要里程碑的更多详细信息，以及您如何为贵组织的此升级做好准备：

## Workfront结束对TLS 1.0的正式支持（2018年3月5日）

Workfront已于2018年3月终止官方对TLS 1.0的支持。

利用TLS 1.0的浏览器连接和API集成仍然可用，但Workfront将无法解决Workfront应用程序中与TLS 1.0相关的问题。

## Workfront集成禁用了使用TLS 1.0（2019年1月9日）

2019年1月9日，必须升级所有利用TLS 1.0的Workfront浏览器连接和API集成，才能使用TLS 1.1或更高版本。 此时后，继续利用TLS 1.0（入站或出站连接）的浏览器连接和API集成将无法再与Workfront应用程序进行通信。 

## 将在2019年第4季度禁用TLS 1.1

在生产环境中，TLS 1.1于2019年10月21日被禁用。 此后，所有使用TLS 1.1的集成都将无法再正常运行。

这项更改将于8月7日在预览和沙盒环境中生效，以帮助组织为关闭做好准备。

## 为TLS升级做准备

* [通过浏览器访问Workfront时](#when-accessing-workfront-via-the-browser)
* [通过API连接到Workfront时](#when-connecting-to-workfront-via-the-api)

### 通过浏览器访问Workfront时 {#when-accessing-workfront-via-the-browser}

确保贵组织中的用户通过支持的浏览器访问Workfront。 (有关支持的浏览器的信息，请参阅 [Adobe Workfront浏览器要求](../../../workfront-basics/workfront-browser-requirements.md).)

Workfront支持的所有浏览器都与TLS 1.2兼容。

### 通过API连接到Workfront时 {#when-connecting-to-workfront-via-the-api}

如果您要通过API（入站或出站）将第三方应用程序集成到Workfront，请确保在您的集成中启用了TLS 1.2（和TLS 1.2加密协议）。
