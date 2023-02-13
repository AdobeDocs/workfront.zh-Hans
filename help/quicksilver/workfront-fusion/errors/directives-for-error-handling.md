---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中错误处理的指令 [!DNL Adobe Workfront Fusion]
description: 本文介绍了可用于在 [!DNL Adobe Workfront Fusion] 方案。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 50b43cd4bafdfc3379eb1d73c12e15c791e28dbe
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 中错误处理的指令 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 错误处理指令

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>回滚</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>方案执行会立即停止，并且 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">回滚</a> 将在所有模块上启动阶段，尝试将所有模块还原到其初始状态。 不会处理后续模块。</p> <p>除少数错误类型外，在方案设置下指定的连续错误数后，将停用方案。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">连续错误数</a>.</p> <p>方案执行状态标记为“error”。</p> <p>注意：如果未将错误处理程序路由附加到模块，并且 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL允许存储不完整的执行]</a> 未选中[!UICONTROL方案设置]下的设置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>提交</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>方案执行立即停止，并在所有模块上启动提交阶段。 不会处理后续模块。</p> <p>将忽略所有未处理的包。</p> <p>方案执行状态标记为“成功”。 有关提交阶段的信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">提交</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion中的方案执行、周期和阶段</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>恢复</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>指定替代输出并提供给遇到错误的模块。</p> <p>后续模块被处理。</p> <p>方案执行状态标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>忽略</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>将忽略该错误，并且不会处理后续模块。</p> <p>如果存在未处理的包，则情景会继续正常执行。</p> <p>方案执行状态标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>中断</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>方案执行的状态存储在未完成执行的队列中，在该队列中可以手动解决错误。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">查看和解决Adobe Workfront Fusion中未完成的执行</a>. </p> <p>不过，也有一些例外。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">允许存储未完成的执行</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion中的“方案设置”面板</a>.</p> <p>不会处理后续模块。</p> <p>如果存在未处理的包，则情景会继续正常执行。</p> <p>禁用[!UICONTROL Automatically complete execution]选项时，方案执行状态将标记为“警告”。</p> <p>请参阅 <a href="#break" class="MCXref xref">[!UICONTROL中断]</a> 部分以了解更多信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>重新尝试</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>在某些情况下，当故障原因可能会随着时间的推移而传递时，重新执行故障模块几次可能会很有用。</p> <p>Workfront Fusion当前不提供重试指令，不过可以使用多种解决方法来模拟其功能。 有关更多信息，请参阅 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">在Adobe Workfront Fusion中处理重试错误</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>当前，错误处理指令不能在错误处理路由的范围之外使用， [!DNL Workfront Fusion] 目前不提供使您能够根据条件轻松生成（抛出）错误的“抛出”模块，不过可以使用解决方法来模拟其功能。 有关更多信息，请参阅 [错误处理程序路由](../../workfront-fusion/errors/error-handling.md#error) 在文章中 [Adobe Workfront Fusion中的错误处理](../../workfront-fusion/errors/error-handling.md). 另请参阅 [Throw的解决方法](../../workfront-fusion/errors/throw.md#workarou) 在文章中 [在Adobe Workfront Fusion中抛出错误处理](../../workfront-fusion/errors/throw.md).

## 中断 {#break}

当错误由 [!DNL Break] 指令中，将在 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) 文件夹，该文件夹存储方案执行的状态以及来自先前模块的数据。 对于导致错误的每个数据包，将创建单独的记录。

该记录引用错误源于的模块，并包含有关模块接收哪些数据作为输入的信息。 有关更多信息，请参阅 [查看和解决Adobe Workfront Fusion中未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

在此，您可以通过更新方案（如果需要）并运行一次来手动解决错误。

另一方面，通过启用 [!UICONTROL 自动完成执行] 选项，可将其配置为通过在指定的分钟数后重新执行方案来自动处理未完成的执行。

启用此选项后，当发生错误时，将检索未完成的执行(在 [!UICONTROL 尝试之间的间隔] 字段)并使用原始输入数据执行。 这将重复执行，直到模块执行完成，且没有出现错误，或直到达到指定的尝试次数。

>[!NOTE]
>
>如果初始重试尝试失败，则重试之间的间隔会呈指数级增长，而每次其他尝试都会如此。

打开“自动完成执行”后，方案运行将标记为“成功”，因为中断错误处理程序的自动重试将自动处理问题。 在这种情况下，用户不会收到有关失败运行的电子邮件。

关闭“自动完成执行”后，运行将标记为“警告”。

![](assets/break-directive-350x241.png)

但是，在未完成执行下存储的执行存在一些异常，并且存在一些错误类型，因此无法自动重试方案执行。 有关更多信息，请参阅 [允许存储未完成的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

有关其他信息，请参阅 [Adobe Workfront Fusion中的高级错误处理](../../workfront-fusion/errors/advanced-error-handling.md).
