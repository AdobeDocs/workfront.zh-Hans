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
source-git-commit: ec5ed146456c2f75926820f5421bf4feee121399
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]性能护栏

>[!NOTE]
>
>除[!DNL Adobe Workfront license]外，[!DNL Adobe Workfront Fusion]还需要[!DNL Adobe Workfront Fusion]许可证。

工作自动化需要快速处理，因此[!DNL Adobe Workfront Fusion]专为高性能而设计。 由于长时间运行的方案可能会减慢工作的速度，因此我们设计了[!DNL Workfront Fusion]保留性能的护栏，以限制执行时间、数据大小和其他方案参数。 [!DNL Workfront Fusion]设计人员应了解这些护栏，并将它们融入到其设计实践中。

## 浏览器

* Workfront Fusion仅支持基于Chrome的浏览器。

## 方案

* 默认方案执行超时为&#x200B;**40分钟**。 当执行达到此超时时，[!DNL Workfront Fusion]将在下一个循环或操作后中断方案执行，具体取决于方案。 这将强制在达到40分钟限制后不久停止场景
* 方案Blueprint的最大大小为&#x200B;**5 MB**，但我们建议将方案大小保持在&#x200B;**3 MB**&#x200B;以下。

  使用大量字段创建或更新数据的应用程序模块可能会导致生成非常大的Blueprint。

   * 使用[!DNL Workfront]应用时，请确保仅选择创建或更新用例所需的字段。
   * 使用其他应用程序时，使用自定义API模块与任何具有大量字段的记录类型进行交互。

* 虽然某个方案中的模块数没有上限，但超过150个模块的方案会对[!DNL Workfront Fusion]系统的性能产生负面影响。 因此，我们不建议创建超过150个模块的场景。

## 运营

* 默认操作超时通常为&#x200B;**40秒**。

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 文件

* Fusion的文件总处理容量为&#x200B;**1 GB**。 该限制基于总内存成本。 每项操作都会产生该成本。 如果下载并上传了一个400 MB的文件，则文件容量的总成本将为800 MB。

## 服务器内存使用率

* 单个执行的服务器内存使用率限制为&#x200B;**1 GB**。

  许多因素（如大型文件或复杂模块）可能会以难以预测或控制的方式影响服务器内存的使用。 因此，即使场景遵循所有其他性能护栏，场景执行也可能超过1 GB内存限制。 超过内存限制会导致执行失败。

## Webhook

* 有效负载的默认最大大小为&#x200B;**5 MB**。
* Webhook限制为每秒&#x200B;**100个请求**。 达到此限制后，Workfront Fusion将发送429 （[!UICONTROL 太多请求]）状态。
* [!DNL Workfront Fusion]存储webhook负载30天。 在收到webhook有效负载超过30天后对其进行访问会导致错误“[!UICONTROL 无法从存储中读取文件。]”
* 如果出现以下任一情况，Webhook将自动停用：

   * webhook已超过5天未连接到任何场景
   * webhook仅用于非活动场景，这些场景已非活动超过30天。

* 如果停用的Webhook未连接到任何场景并且已处于停用状态超过30天，则会自动删除和取消注册它们。

## 执行历史记录

* 执行历史记录日志的大小限制为&#x200B;**100 MB**。 如果执行历史记录超过此大小，则仅显示前100 MB。
* 如果一个场景有多个并发执行。 在“场景详细信息”页面的执行区域中，只显示5个执行。 即使正在运行的执行超过5次，情况也是如此。

## 未完成的执行

* 未完成的执行限制为&#x200B;**500 MB**&#x200B;的总大小。 如果达到500 MB限制，则不会存储更多未完成的执行。

## 重试

* 使用Break模块并指定Retry指令时，如果某个方案在2分钟的时间范围内连续失败10次，则将自动停用该方案。

