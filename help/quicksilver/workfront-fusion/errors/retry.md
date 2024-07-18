---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中重试错误处理
description: 在某些情况下，如果失败原因可能会随着时间的推移而推移，则重新执行几次失败模块会很有用。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中重试错误处理

在某些情况下，如果失败的原因可能会随着时间的推移而推移，则重新执行失败模块会很有用。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## [!UICONTROL 重试]错误处理指令的解决方法

[!UICONTROL Adobe Workfront Fusion]当前不提供[!UICONTROL 重试]错误处理指令，但可以使用两个变通方法模拟其功能。 有关详细信息，请参阅Adobe Workfront Fusion中用于错误处理的[指令](../../workfront-fusion/errors/directives-for-error-handling.md)。

### 使用[!UICONTROL Break]指令

1. 在场景设置面板中，启用&#x200B;**[!UICONTROL 允许存储未完成的执行]**&#x200B;选项。

   有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板。

1. 将错误处理程序路由附加到模块，如[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)中的[错误处理中所述。
1. 将[!UICONTROL Break]指令链接到错误处理程序路由并对其进行配置。

   有关详细信息，请参阅[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中用于错误处理的[指令。

   ![](assets/break-directive-350x241.png)

#### 缺点

* 最小重试间隔为一分钟。
* 如果模块正在处理多个捆绑包并且捆绑包处理失败，则将部分执行（仅导致错误的捆绑包）移动到不完整执行文件夹并根据[!UICONTROL Break]指令设置计划重试。 但是，当前执行继续，模块将继续处理后续捆绑包。 您可以在[!UICONTROL 方案设置]中启用“[!UICONTROL 顺序处理]”选项，以防止在成功解析存储在“未完成执行”文件夹中的执行之前再次执行方案。

  有关未完成执行的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中查看和解决未完成的执行。

### 使用[!UICONTROL 中继器]模块

1. 使用&#x200B;**[!UICONTROL 中继器]**&#x200B;模块并将其&#x200B;**[!UICONTROL 中继器]**&#x200B;字段设置为最大尝试次数。
1. 将可能失败的模块链接到&#x200B;**[!UICONTROL 中继器]**&#x200B;模块。
1. 将错误处理程序路由附加到此模块（请参阅 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)中的[错误处理）。
1. 将&#x200B;**[!UICONTROL Tools] > [!UICONTROL Sleep]**&#x200B;模块链接到错误处理程序路由，并将其&#x200B;**[!UICONTROL Delay]**&#x200B;字段设置为尝试之间的秒数。

1. 在&#x200B;**[!UICONTROL Tools] > [!UICONTROL Sleep]**&#x200B;模块之后链接&#x200B;**[!UICONTROL Ignore]**&#x200B;指令(有关Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md)中的错误处理，请参阅[指令)。

1. 在可能失败的模块后链接&#x200B;**[!UICONTROL Tools] > [!UICONTROL Set variable]**&#x200B;模块，并将其配置为将该模块的结果存储到一个名为的变量中，例如`Result`。

1. 在&#x200B;**[!UICONTROL 工具] > [!UICONTROL 设置变量]**&#x200B;之后链接&#x200B;**[!UICONTROL 数组汇总]**&#x200B;模块，并在其Source模块字段中选择&#x200B;**[!DNL Repeater]**&#x200B;模块。

1. 将&#x200B;**[!UICONTROL Tools] > [!UICONTROL Get variable]**&#x200B;模块链接到&#x200B;**[!UICONTROL Array aggregator]**&#x200B;模块，并将其配置为获取`Result`变量的值。

1. 在&#x200B;**[!UICONTROL 中继器]**&#x200B;模块和可能失败的模块之间插入&#x200B;**[!UICONTROL Tools] > [!UICONTROL Get变量]**&#x200B;模块，并将其配置为获取`Result`变量的值。

1. 在此&#x200B;**[!UICONTROL 工具] > [!UICONTROL 获取变量]**&#x200B;模块与可能失败的模块之间插入筛选器，以仅在`Result`变量不存在时继续。

>[!INFO]
>
>**示例：**&#x200B;以下是示例场景，其中[!UICONTROL HTTP] >[!UICONTROL 发出请求]模块表示可能失败的模块：
>
>![](assets/http-make-request-350x116.png)
>
>如果可能失败的模块的结果过于复杂，无法存储在一个简单的变量中，则可以使用数据存储来存储/检索结果。 数据存储将只包含一个记录。 例如，记录的键可以是`Result`。
>
>有关数据存储的详细信息，请参阅[数据存储在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)中

#### 缺点

此解决方法可能看起来有点过于复杂，而且对操作也更加苛刻。
