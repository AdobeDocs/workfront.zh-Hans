---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在Adobe Workfront Fusion中处理抛出错误
description: 在某些情况下，您可能希望强制停止场景执行，然后进入“回滚”或“提交”阶段，或者停止路由处理，然后将其存储在查看队列中，并在Adobe Workfront Fusion中解决未完成的执行。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中引发错误处理

在某些情况下，您可能希望强制停止方案执行，然后执行[回滚](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)或[提交](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit)阶段，或者停止路由处理并选择性地将其存储在未完成执行的队列中。

目前，错误处理指令不能在[错误处理程序路由](../../workfront-fusion/errors/error-handling.md#error)的范围之外使用，并且[!DNL Adobe Workfront Fusion]不提供可让您轻松有条件地生成（抛出）错误的模块。

有关未完成执行的信息，请参阅[在Adobe Workfront Fusion中查看和解决未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

有关错误处理指令的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中用于错误处理的[指令。

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

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Throw解决方法

要有条件地引发错误，您可以配置模块，使其在操作期间选择性地出现故障。 一种可能是使用[!UICONTROL JSON] > [!UICONTROL 解析JSON]模块（请参阅[JSON模块](../../workfront-fusion/apps-and-their-modules/json-modules.md)），该模块配置为选择性地引发错误（在本例中为BundleValidationError）：

然后，可以将错误处理指令之一附加到错误处理路由：

* 强制停止方案执行并执行回滚阶段： [!UICONTROL 回滚]
* 强制停止方案执行并执行提交阶段： [!UICONTROL 提交]
* 停止处理路由： [!UICONTROL 忽略]
* 停止处理路由并将其存储在未完成执行的队列文件夹中： [!UICONTROL 中断]

以下示例显示了[!DNL Rollback]指令的使用：

![](assets/rollback-directive-350x175.png)
