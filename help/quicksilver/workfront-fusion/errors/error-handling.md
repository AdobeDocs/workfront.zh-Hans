---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中的错误处理 [!DNL Adobe Workfront Fusion]
description: 当场景执行过程中发生错误时，通常是因为服务因故障而不可用、服务以意外数据做出响应或输入数据验证失败。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 中的错误处理 [!DNL Adobe Workfront Fusion]

当场景执行过程中发生错误时，通常是因为服务因故障而不可用、服务以意外数据做出响应或输入数据验证失败。

如果模块在场景执行期间引发错误，并且没有附加到模块的错误处理路由，则执行默认错误处理逻辑，如中所述 [处理以下对象时出错： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

通过将错误处理程序路由添加到模块，可以将默认错误处理逻辑替换为您自己的错误处理逻辑。 [!DNL Adobe Workfront Fusion] 提供了五个不同的指令，它们可以在错误处理程序路由的末尾插入。

有关更多信息，请参阅 [中用于错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## 错误处理程序路由

要添加错误处理程序路由到模块，请执行以下操作：

1. 右键单击模块并选择 **[!UICONTROL 添加错误处理程序]**：

   ![](assets/error-handler-route.png)

   模块显示指令列表，以及在您的场景中使用的应用程序。

1. 如果添加错误处理程序的模块是路由中的最后一个模块，请选择其中一个指令。

   或

   将一个或多个模块添加到错误处理程序路由。

   如果向路由添加更多模块， [!UICONTROL 忽略] 默认情况下会应用指令，如果出现错误，则会处理该路由上的后续模块。


>[!INFO]
>
>在此示例中，如果在执行 [!UICONTROL 创建文件夹] 模块， [!UICONTROL 忽略] 指令将自动应用，场景将移动到错误处理程序路由上的下一个模块。
>
>但是，如果没有错误，场景将移至 [!UICONTROL 列出文件夹模块中的所有文件] 按常规路线行驶。
>
>![](assets/if-there-is-no-error-350x234.png)

请注意，错误处理程序路由由透明圆组成，而常规路由由实心圆组成。

## 处理指令时出错

这些指令简要说明如下。 有关更多信息，请参阅 [中用于错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

总共有五个指令，可根据场景执行是否继续分组为以下类别。

以下指令可确保场景执行继续进行：

* **[!UICONTROL 恢复]**：用于为出现错误的模块指定替换输出。 场景执行状态标记为成功
* **[!UICONTROL 忽略]**：忽略错误。 场景执行状态标记为成功
* **[!UICONTROL 中断]**：存储未完成执行的队列的输入。 场景执行状态标记为警告。 有关更多信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

如果发生错误时应停止场景执行，请使用以下指令之一：

* **[!UICONTROL 回滚]**：立即停止场景执行并将其状态标记为错误
* **[!UICONTROL 提交]**：立即停止场景执行并将其状态标记为成功

有关错误处理的详细信息，请参阅：

* [中用于错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [中的高级错误处理 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)