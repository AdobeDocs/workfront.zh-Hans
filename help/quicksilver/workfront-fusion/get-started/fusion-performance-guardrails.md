---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 方案，性能
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion性能护栏
description: 除了Adobe Workfront许可证之外，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 00ef33666bebe434739056cb38c3dff24285d682
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] 性能护栏

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除了许可证外， [!DNL Adobe Workfront license].

工作自动化要求快速处理，因此 [!DNL Adobe Workfront Fusion] 专为高性能而设计。 由于长期运行情况会减慢您的工作速度，因此我们设计了 [!DNL Workfront Fusion] 带有可限制执行时间、数据大小和其他方案参数的保留性能的护栏。 [!DNL Workfront Fusion] 设计人员应该注意这些护栏，并将它们融入到其设计实践中。

## 浏览器

Workfront Fusion仅支持基于Chrome的浏览器。

## 方案

* 默认方案执行超时为 **40分钟**. 当执行达到此超时时， [!DNL Workfront Fusion] 中断下一个周期或操作之后的方案执行，具体取决于方案。 这将强制在达到40分钟限制后不久停止场景
* 方案Blueprint的最大大小为 **5 MB**，但我们建议将方案大小保留在 **3 MB**.

  使用大量字段创建或更新数据的应用程序模块可能会导致生成非常大的Blueprint。

   * 使用时 [!DNL Workfront] 应用程序时，请确保仅选择创建或更新用例所需的字段。
   * 使用其他应用程序时，使用自定义API模块与任何具有大量字段的记录类型进行交互。

* 虽然场景中的模块数量没有上限，但超过150个模块的场景会对您的性能产生负面影响 [!DNL Workfront Fusion] 系统。 因此，我们不建议创建超过150个模块的场景。

## 运营

* 默认操作超时通常为 **40秒**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 文件

* Fusion的文件总处理容量为 **1 GB**. 该限制基于总内存成本。 每项操作都会产生该成本。 如果下载并上传了一个400 MB的文件，则文件容量的总成本将为800 MB。

## 服务器内存使用率

* 单次执行的服务器内存使用量限制为 **1 GB**.

  许多因素（如大型文件或复杂模块）可能会以难以预测或控制的方式影响服务器内存的使用。 因此，即使场景遵循所有其他性能护栏，场景执行也可能超过1 GB内存限制。 超过内存限制会导致执行失败。

## Webhook

* 有效负载的默认最大大小为 **5 MB**.
* Webhook仅限于 **每秒100个请求**. 当达到此限制时，Workfront Fusion发送429 ([!UICONTROL 请求过多])状态。
* [!DNL Workfront Fusion] 存储webhook负载30天。 在收到webhook有效负载超过30天后对其进行访问会导致错误»[!UICONTROL 无法从存储中读取文件。]&quot;
* 如果出现以下任一情况，Webhook将自动停用：

   * webhook已超过5天未连接到任何场景
   * webhook仅用于非活动场景，这些场景已非活动超过30天。

* 如果停用的Webhook未连接到任何场景并且已处于停用状态超过30天，则会自动删除和取消注册它们。

## 执行历史记录

* 执行历史记录日志限制为 **100 MB**. 如果执行历史记录超过此大小，则仅显示前100 MB。

## 重试

使用Break模块并指定Retry指令时，如果某个方案在2分钟的时间范围内连续失败10次，则将自动停用该方案。

