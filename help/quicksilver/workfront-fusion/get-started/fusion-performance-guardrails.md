---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 方案，性能
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion性能护栏
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 性能护栏

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除 [!DNL Adobe Workfront license].

工作自动化需要快速处理，因此 [!DNL Adobe Workfront Fusion] 专为高性能而设计。 由于长期运行的情景会减慢您的工作进度，因此我们设计了 [!DNL Workfront Fusion] 具有性能保护护，可限制执行时间、数据大小和其他方案参数。 [!DNL Workfront Fusion] 设计人员应该注意这些护栏，并将它们纳入其设计实践。

## 场景

* 默认方案执行超时为 **40分钟**. 当执行达到此超时时， [!DNL Workfront Fusion] 在下一个周期或操作后中断方案执行，具体取决于方案。 这会强制在达到40分钟限制后不久停止方案
* 方案Blueprint的最大大小为 **5 MB**&#x200B;但是，我们建议将方案大小保留为 **3 MB**.

   使用大量字段创建或更新数据的应用程序模块可能会产生非常大的蓝图。

   * 使用 [!DNL Workfront] 应用程序，请确保仅选择创建或更新用例所需的字段。
   * 使用其他应用程序时，使用自定义API模块与具有大量字段的任何记录类型进行交互。

* 虽然方案中的模块数量没有上限，但包含150个以上模块的方案会对您的 [!DNL Workfront Fusion] 系统。 因此，我们不建议创建包含超过150个模块的方案。

## 操作

* 默认操作超时通常为 **40秒**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## 文件

* Fusion对文件的总处理能力是 **1 GB**. 该限制基于总内存成本。 每项操作都会造成这一成本。 如果下载并上载单个400 MB的文件，则文件容量的总成本将为800 MB。

## 服务器内存使用率

* 单次执行的服务器内存使用率限制为 **1 GB**.

   许多因素（如大文件或复杂模块）都可能会以难以预测或控制的方式影响服务器内存的使用。 因此，即使方案遵循所有其他性能限制，您的方案执行也可能超过1 GB内存限制。 超过内存限制会导致执行失败。

## Webhooks

* 有效负载的默认最大大小为 **5 MB**.
* Webhook限于 **每秒100次请求**. 当达到此限制时，Workfront Fusion会发送[!UICONTROL 请求过多])状态。
* [!DNL Workfront Fusion] 存储30天的网页挂钩负载。 在收到WebHook负载超过30天后访问该负载会导致错误“[!UICONTROL 无法从存储中读取文件。]&quot;
* 如果出现以下任一情况，将自动停用Web挂接：

   * 网页挂接已超过5天未连接到任何方案
   * Webhook仅用于不活动情景（已处于非活动状态超过30天）。

* 如果已停用的Web挂接未连接到任何方案并且处于停用状态超过30天，则会自动删除和取消注册这些挂接。
