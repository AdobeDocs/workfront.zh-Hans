---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 重试错误处理 [!DNL Adobe Workfront Fusion]
description: 在某些情况下，如果失败的原因可能会随着时间的推移而推移，则多次重新执行失败模块会很有用。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 重试错误处理 [!DNL Adobe Workfront Fusion]

在某些情况下，如果故障原因可能随时间推移而推移，则重新执行故障模块会很有用。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

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
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 解决方法 [!UICONTROL 重试] 错误处理指令

[!UICONTROL Adobe Workfront Fusion] 当前不提供 [!UICONTROL 重试] 错误处理指令，但可以采用两种解决方法来模拟其功能。 有关更多信息，请参阅 [Adobe Workfront Fusion中用于错误处理的指令](../../workfront-fusion/errors/directives-for-error-handling.md).

### 使用 [!UICONTROL 中断] 指令

1. 在场景设置面板中，启用 **[!UICONTROL 允许存储未完成的执行]** 选项。

   有关更多信息，请参阅 [中的方案设置面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. 将错误处理程序路由附加到模块，如中所述 [中的错误处理 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. 链接 [!UICONTROL 中断] 错误处理程序路由的指令并进行配置。

   有关更多信息，请参阅 [中用于错误处理的指令 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 缺点

* 最小重试间隔为1分钟。
* 如果模块正在处理多个捆绑包，并且捆绑包处理失败，则会将部分执行（仅导致错误的捆绑包）移至不完整执行文件夹并根据 [!UICONTROL 中断] 指令设置。 但是，当前执行继续，模块继续处理后续捆绑包。 您可以启用&quot;[!UICONTROL 顺序处理]中的“ ”选项 [!UICONTROL 方案设置] 以防止场景再次执行，直到成功解析存储在未完成执行文件夹中的执行为止。

  有关未完成执行的更多信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 使用 [!UICONTROL 中继器] 模块

1. 采用 **[!UICONTROL 中继器]** 模块和设置其 **[!UICONTROL 重复]** 字段至最大尝试次数。
1. 将可能故障的模块链接到 **[!UICONTROL 中继器]** 模块。
1. 将错误处理程序路由附加到此模块(请参阅 [中的错误处理 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md))。
1. 链接 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模块到错误处理程序路由并设置其 **[!UICONTROL 延迟]** 字段表示两次尝试之间的秒数。

1. 链接 **[!UICONTROL 忽略]** 指令位于 **[!UICONTROL 工具] > [!UICONTROL 睡眠]** 模块(请参阅 [Adobe Workfront Fusion中用于错误处理的指令](../../workfront-fusion/errors/directives-for-error-handling.md))。

1. 链接 **[!UICONTROL 工具] > [!UICONTROL 设置变量]** 将模块放置在可能失败的模块之后，并将其配置为将模块的结果存储到一个名为的变量中，例如， `Result`.

1. 链接 **[!UICONTROL 数组汇总]** 模块位于 **[!UICONTROL 工具] > [!UICONTROL 设置变量]** 并选择 **[!DNL Repeater]** 模块的“源模块”字段中。

1. 链接 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块到 **[!UICONTROL 数组汇总]** 模块并对其进行配置，以获取 `Result` 变量。

1. 插入 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块介于 **[!UICONTROL 中继器]** 模块和可能失败的模块，并将其配置为获得 `Result` 变量。

1. 在此之间插入筛选器 **[!UICONTROL 工具] > [!UICONTROL 获取变量]** 模块和可能故障的模块仅在 `Result` 变量不存在。

>[!INFO]
>
>**示例：** 以下是一个示例场景，其中 [!UICONTROL HTTP] >[!UICONTROL 提出请求] 模块表示可能失败的模块：
>
>![](assets/http-make-request-350x116.png)
>
>如果可能失败的模块的结果过于复杂，无法存储在一个简单的变量中，则可以使用数据存储来存储/检索结果。 数据存储将只包含一个记录。 例如，记录的键可以是， `Result`.
>
>有关数据存储的详细信息，请参阅 [数据存储位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### 缺点

此解决方法可能显得过于复杂，而且对操作也要求较高。
