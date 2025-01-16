---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中处理错误
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中处理错误

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [添加错误处理](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/error-handling.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

当在执行场景期间发生错误时，通常是因为服务因故障而不可用、服务以意外数据响应或输入数据验证失败。

如果模块在场景执行期间引发错误，并且没有附加到模块的错误处理路由，则将执行默认错误处理逻辑，如 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中的[错误处理中所述。

通过将错误处理程序路由添加到模块，可以将默认错误处理逻辑替换为您自己的错误处理逻辑。 [!DNL Adobe Workfront Fusion]提供了五个不同的指令，它们可以在错误处理程序路由的末尾插入。

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中用于错误处理的[指令。

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

## 错误处理程序路由

要添加错误处理程序路由到模块，请执行以下操作：

1. 右键单击该模块并选择&#x200B;**[!UICONTROL 添加错误处理程序]**：

   ![](assets/error-handler-route.png)

   此模块显示指令列表，以及在您的方案中使用的应用程序。

1. 如果添加错误处理程序的模块是路由中的最后一个模块，请选择其中一个指令。

   或

   将一个或多个模块添加到错误处理程序路由。

   如果向路由添加更多模块，则默认应用[!UICONTROL Ignore]指令，并在出现错误时，处理该路由上的后续模块。


>[!INFO]
>
>在此示例中，如果在执行[!UICONTROL 创建文件夹]模块时出错，将自动应用[!UICONTROL Ignore]指令，并且场景将移动到错误处理程序路由上的下一个模块。
>
>但是，如果没有错误，方案将移动到常规路由上的文件夹模块]中的[!UICONTROL 列出所有文件。
>
>![](assets/if-there-is-no-error-350x234.png)

请注意，错误处理程序路由由透明圆组成，而常规路由由实心圆组成。

## 处理指令时出错

这些指令简要说明如下。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中用于错误处理的[指令。

总共有五个指令，可根据是否继续执行方案将其分组为以下类别。

以下指令可确保场景执行继续：

* **[!UICONTROL 恢复]**：允许您为出现错误的模块指定替代输出。 方案执行状态标记为成功
* **[!UICONTROL 忽略]**：忽略该错误。 方案执行状态标记为成功
* **[!UICONTROL 中断]**：将输入存储到未完成执行的队列。 方案执行状态标记为警告。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中查看和解决未完成的执行。

如果发生错误时应停止场景执行，请使用以下指令之一：

* **[!UICONTROL 回滚]**：立即停止方案执行并将其状态标记为错误
* **[!UICONTROL 提交]**：立即停止方案执行并将其状态标记为成功

有关错误处理的详细信息，请参阅：

* [ [!DNL Adobe Workfront Fusion]中用于错误处理的指令](../../workfront-fusion/errors/directives-for-error-handling.md)
* [高级错误处理（在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)中）