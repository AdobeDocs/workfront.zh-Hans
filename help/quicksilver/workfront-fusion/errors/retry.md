---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的重试错误处理 [!DNL Adobe Workfront Fusion]
description: 在某些情况下，如果失败的原因可能会随着时间的推移而发生，则重新执行失败模块几次会很有用。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# 中的重试错误处理 [!DNL Adobe Workfront Fusion]

在某些情况下，如果失败的原因可能会随着时间的推移而发生，则重新执行失败的模块会很有用。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 解决方法 [!UICONTROL 重试] 错误处理指令

[!UICONTROL Adobe Workfront Fusion] 当前不提供 [!UICONTROL 重试] 错误处理指令，但可使用两种解决方法来模拟其功能。 有关更多信息，请参阅 [Adobe Workfront Fusion中错误处理的指令](../../workfront-fusion/errors/directives-for-error-handling.md).

### 使用 [!UICONTROL 中断] 指令

1. 在方案设置面板中，启用 **[!UICONTROL 允许存储不完整的执行]** 选项。

   有关更多信息，请参阅 [中的“方案设置”面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 将错误处理程序路由附加到模块，如 [在中处理错误 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. 链接 [!UICONTROL 中断] 指令到错误处理程序路由并对其进行配置。

   有关更多信息，请参阅 [中错误处理的指令 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 缺点

* 最小重试间隔为1分钟。
* 如果模块正在处理多个包，并且包的处理失败，则部分执行（仅导致错误的包）将移到未完成的执行文件夹中，并根据 [!UICONTROL 中断] 指令设置。 但是，当前执行会继续，并且模块会继续处理后续的包。 您可以启用“[!UICONTROL 顺序处理]“ ”选项 [!UICONTROL 方案设置] 以防止在成功解析“未完成执行”文件夹中存储的执行操作之前再次执行方案。

   有关未完成执行的更多信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 使用 [!UICONTROL 中继器] 模块

1. 使用 **[!UICONTROL 中继器]** 模块及其设置 **[!UICONTROL 重复]** 字段的长度。
1. 将可能失败的模块链接到 **[!UICONTROL 中继器]** 模块。
1. 将错误处理程序路由附加到此模块(请参阅 [在中处理错误 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md))。
1. 链接 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模块到错误处理程序路由并设置其 **[!UICONTROL 延迟]** 字段，以表示两次尝试之间间隔的秒数。

1. 链接 **[!UICONTROL 忽略]** 指令之后 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模块(请参阅 [Adobe Workfront Fusion中错误处理的指令](../../workfront-fusion/errors/directives-for-error-handling.md))。

1. 链接 **[!UICONTROL 工具] > [!UICONTROL 设置变量]** 模块，并将其配置为将模块的结果存储在名为的变量中，例如 `Result`.

1. 链接 **[!UICONTROL 阵列聚合器]** 模块之后 **[!UICONTROL 工具] > [!UICONTROL 设置变量]** 然后选择 **[!DNL Repeater]** 模块。

1. 链接 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块 **[!UICONTROL 阵列聚合器]** 模块，并对其进行配置以获取 `Result` 变量。

1. 插入 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块之间 **[!UICONTROL 中继器]** 模块和可能失败的模块，并对其进行配置，以获取 `Result` 变量。

1. 在此之间插入过滤器 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块和可能出现故障的模块仅在 `Result` 变量不存在。

>[!INFO]
>
>**示例：** 以下是一个示例情景，其中 [!UICONTROL HTTP] >[!UICONTROL 请求] 模块表示可能失败的模块：
>
>![](assets/http-make-request-350x116.png)
>
>如果潜在故障模块的结果过于复杂，无法存储在简单变量中，则可以使用数据存储来存储/检索结果。 数据存储将只包含一条记录。 例如，记录的键可以是， `Result`.
>
>有关数据存储的更多信息，请参阅 [数据存储在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### 缺点

此解决方法可能看起来有点太复杂，而且在操作方面要求也更高。
