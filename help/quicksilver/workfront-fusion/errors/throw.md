---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在Adobe Workfront Fusion中抛出错误处理
description: 在某些情况下，您可能想要强制停止方案执行，然后执行回滚或提交阶段，或者停止路由的处理，并选择将其存储在“视图”队列中，并解决Adobe Workfront Fusion中不完整的执行。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 在中引发错误处理 [!DNL Adobe Workfront Fusion]

在某些情况下，您可能希望强制停止方案执行，然后执行 [回滚](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) 或 [提交](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) 逐步或停止路由的处理，并选择性地将其存储在未完成执行的队列中。

当前，错误处理指令不能在 [错误处理程序路由](../../workfront-fusion/errors/error-handling.md#error) 和 [!DNL Adobe Workfront Fusion] 不提供可让您轻松有条件地生成（引发）错误的模块。

有关未完成执行的信息，请参阅 [查看和解决Adobe Workfront Fusion中未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

有关错误处理指令的信息，请参阅 [中错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Throw的解决方法

要有条件地引发错误，您可以配置模块，使其在操作过程中有意失败。 一种可能是利用 [!UICONTROL JSON] > [!UICONTROL 解析JSON] 模块(请参阅 [JSON模块](../../workfront-fusion/apps-and-their-modules/json-modules.md))，配置为可选地引发错误（在此例中为BundleValidationError）：

然后，可以将一个错误处理指令附加到错误处理路由：

* 强制方案执行停止并执行回滚阶段： [!UICONTROL 回滚]
* 强制方案执行停止并执行提交阶段： [!UICONTROL 提交]
* 停止处理路由： [!UICONTROL 忽略]
* 停止处理路由并将其存储在未完成执行文件夹的队列中： [!UICONTROL 中断]

以下示例显示了 [!DNL Rollback] 指令：

![](assets/rollback-directive-350x175.png)
