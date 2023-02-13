---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在中处理错误 [!DNL Adobe Workfront Fusion]
description: 在执行方案期间发生错误时，通常是因为服务因故障而不可用、服务用意外数据响应或输入数据验证失败。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 在中处理错误 [!DNL Adobe Workfront Fusion]

在执行方案期间发生错误时，通常是因为服务因故障而不可用、服务用意外数据响应或输入数据验证失败。

>[!NOTE]
>
>如果模块在方案执行期间引发错误，并且没有附加到模块的错误处理路由，则执行默认的错误处理逻辑，如 [处理中的错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

通过向模块添加错误处理程序路由，可以将默认错误处理逻辑替换为您自己的逻辑。 [!DNL Adobe Workfront Fusion] 提供了5个不同的指令，其中任何指令都可以插入到错误处理程序路由的末尾。 有关更多信息，请参阅 [中错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## 错误处理程序路由

要向模块添加错误处理程序路由（我们将将其称为模块X），请右键单击该模块并选择 **[!UICONTROL 添加错误处理程序]**:

![](assets/error-handler-route.png)

该模块显示指令列表以及方案中使用的应用程序。 如果模块X是路由中的最后一个模块，则需要选择其中一个指令。 或者，您可以继续向路由添加一个或多个模块。 在本例中， [!UICONTROL 忽略] 指令默认应用于模块X，如果出错，将处理该路由上的后续模块。

![](assets/directives-350x426.png)

如下所示，如果在执行 [!UICONTROL 创建文件夹] 模块， [!UICONTROL 忽略] 如果过滤器“数据错误发生”返回一个或多个包，则指令将被自动应用，并且方案将移至错误处理程序路由上的下一个模块。

但是，如果没有错误，方案将移至 [!UICONTROL 列出文件夹模块中的所有文件] 在常规路线上。

![](assets/if-there-is-no-error-350x234.png)

此外，为了区分错误处理器路由与常规路由，前者由如上所示的透明圆组成。

## 处理指令时出错

下文对这些指令作了简要解释。 有关更多信息，请参阅 [中错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

根据是否应继续执行方案，总共有五个指令可分为以下类别：

以下指令可确保方案继续执行：

* **[!UICONTROL 恢复]** 允许您为出错的模块指定替换输出，并且方案执行状态被标记为成功
* **[!UICONTROL 忽略]** 只会忽略错误，并将方案执行状态标记为成功
* **[!UICONTROL 中断]** 将输入存储到未完成执行的队列，并且方案执行状态标记为警告。 有关更多信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

另一方面，如果应停止方案执行，则必须使用以下指令之一：

* **[!UICONTROL 回滚]** 立即停止方案执行，并将其状态标记为错误
* **[!UICONTROL 提交]** 立即停止方案执行，并将其状态标记为成功

## 其他资源

* [中错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [中的高级错误处理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md) (包括上面引用的Dropbox方案的设置)
