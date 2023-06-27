---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 中用于错误处理的指令 [!DNL Adobe Workfront Fusion]
description: 本文介绍了可用于错误处理的指令。 [!DNL Adobe Workfront Fusion] 场景。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 中用于错误处理的指令 [!DNL Adobe Workfront Fusion]

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

## 用于错误处理的指令

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>回滚</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>场景执行立即停止，并且 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">回滚</a> 所有模块都会启动阶段，以尝试将所有模块恢复到其初始状态。 不处理后续模块。</p> <p>除非存在少数几种错误类型，否则在场景设置下指定的连续错误数之后，将停用场景。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">连续错误数</a>.</p> <p>场景执行状态被标记为“错误”。</p> <p>注意：如果没有将错误处理程序路由附加到模块和 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[！UICONTROL允许存储未完成的执行]</a> 未选中[！UICONTROL场景设置]下的设置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>提交</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>立即停止场景执行，并在所有模块上启动提交阶段。 不处理后续模块。</p> <p>将忽略所有未处理的包。</p> <p>场景执行状态被标记为“成功”。 有关提交阶段的信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">提交</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion中的场景执行、周期和阶段</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>恢复</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>指定替代输出并将其提供给遇到错误的模块。</p> <p>后续模块被处理。</p> <p>场景执行状态被标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>忽略</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>将忽略该错误，并且不处理后续模块。</p> <p>如果存在未处理的包，则场景执行会正常继续。</p> <p>场景执行状态被标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>中断</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>场景执行的状态存储在未完成执行的队列中，其中的错误可以手动解决。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">在Adobe Workfront Fusion中查看和解决未完成的执行</a>. </p> <p>不过，也有一些例外。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">允许存储未完成的执行</a> 在文章中 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion中的“方案设置”面板</a>.</p> <p>不处理后续模块。</p> <p>如果存在未处理的包，则场景执行会正常继续。</p> <p>禁用[！UICONTROL自动完成执行]选项时，场景执行状态被标记为“警告”。</p> <p>请参阅 <a href="#break" class="MCXref xref">[！UICONTROL断点]</a> 部分，以了解更多信息。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>重新尝试</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>在某些情况下，当失败原因可能会随着时间的推移而消失时，重新执行几次失败模块会很有用。</p> <p>Workfront Fusion目前不提供Retry指令，但可以使用几种变通方法模拟其功能。 有关更多信息，请参阅 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">在Adobe Workfront Fusion中重试错误处理</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 目前，错误处理指令不能在错误处理路由之外使用。
>
>   有关更多信息，请参阅 [错误处理程序路由](../../workfront-fusion/errors/error-handling.md#error) 在文章中 [Adobe Workfront Fusion中的错误处理](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] 目前不提供Throw模块，该模块使您能够轻松地有条件地生成（丢弃）错误，尽管可以使用解决方法来模拟其功能。
>
>   有关更多信息，请参阅 [Throw解决方法](../../workfront-fusion/errors/throw.md#workaround-for-throw) 在文章中 [Adobe Workfront Fusion中的抛出错误处理](../../workfront-fusion/errors/throw.md).

## 中断 {#break}

当错误由 [!DNL Break] 指令，在“未完成执行”文件夹中创建记录。 此记录存储场景执行的状态以及先前模块的数据。 记录引用了错误起因的模块，并包含有关模块接收到哪些数据作为输入的信息。 对于导致错误的每个数据包，将创建一个单独的记录。

有关更多信息，请参阅 [在Adobe Workfront Fusion中查看和解决未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 解决由Break指令导致的错误

您可以通过更新场景（如果需要）并运行一次来手动解决该错误。

您还可以通过重新执行场景来配置场景以自动处理不完整的执行。 要配置模块以处理未完成的执行，请执行以下操作：

1. 在Break模块内，启用 [!UICONTROL **自动完成执行**] 选项。
1. 在 **尝试次数** 字段，输入或映射您希望模块重试执行的最大尝试次数

   此数字必须介于1和100之间。
1. 在 **尝试间隔** 字段，输入或映射每次重试之间的分钟数。

启用此选项后，当发生错误时，将检索不完整的执行(在 [!UICONTROL 尝试间隔] 字段)并使用原始输入数据执行。 此操作将重复执行，直到模块执行完成且没有错误，或者直到达到指定的尝试次数。

>[!NOTE]
>
>如果初始重试尝试失败，则重试间隔将每隔一次尝试以指数方式增加。


当“自动完成执行”打开时，场景运行将标记为“成功”，因为Break错误处理程序的自动重试正在自动处理该问题。 在这种情况下，用户不会收到有关失败运行的电子邮件。

关闭“自动完成执行”后，该运行将标记为“警告”。

在“未完成的执行”下存储的执行存在一些异常，并且由于存在某些错误类型，无法自动重试场景执行。

有关更多信息，请参阅 [允许存储未完成的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

有关其他信息，请参阅 [Adobe Workfront Fusion中的高级错误处理](../../workfront-fusion/errors/advanced-error-handling.md).
