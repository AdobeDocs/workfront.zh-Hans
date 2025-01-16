---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion]中用于错误处理的指令'
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 12%

---

# [!DNL Adobe Workfront Fusion]中用于错误处理的指令

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* 用于错误处理的[指令](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/errors/directives-for-error-handling.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

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

## 用于错误处理的指令

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>回滚</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>方案执行立即停止，并且在所有模块上启动<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">回滚</a>阶段，以尝试将所有模块还原到其初始状态。 未处理后续模块。</p> <p>除非出现少数几种错误类型，否则在场景设置下指定连续错误数后，将停用场景。 有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">连续错误数</a>。</p> <p>场景执行状态标记为“错误”。</p> <p>注意：如果未将错误处理程序路由附加到模块，并且未选中[！UICONTROL场景设置]下的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[！UICONTROL允许存储不完整的执行]</a>设置，则这是默认行为。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>提交</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>场景执行立即停止，并且所有模块上的提交阶段都已启动。 未处理后续模块。</p> <p>将忽略所有未处理的包。</p> <p>场景执行状态将标记为“成功”。 有关提交阶段的信息，请参阅<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion中的场景执行、周期和阶段</a>一文中的<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">提交</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>恢复</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>指定替代输出并将其提供给遇到错误的模块。</p> <p>处理后续模块。</p> <p>场景执行状态标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>忽略</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>该错误会被忽略，并且后续模块不会受到处理。</p> <p>如果存在未处理的捆绑包，则场景执行会正常继续进行。</p> <p>场景执行状态标记为“成功”。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>间断</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>场景执行的状态存储在未完成执行的队列中，在该队列中可以手动解决错误。有关详细信息，请参阅<a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">在Adobe Workfront Fusion中查看和解决未完成的执行</a>。 </p> <p>不过，也有一些例外。 有关详细信息，请参阅Adobe Workfront Fusion中的项目<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">场景设置面板</a>中的<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">允许存储不完整的执行</a>。</p> <p>未处理后续模块。</p> <p>如果存在未处理的捆绑包，则场景执行会正常继续进行。</p> <p>禁用[！UICONTROL自动完成执行]选项后，场景执行状态将标记为“警告”。</p> <p>有关详细信息，请参阅下面的<a href="#break" class="MCXref xref">[！UICONTROL Break]</a>部分。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>重试</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>在某些情况下，当失败原因可能随时间推移而推移时，重新执行几次失败模块会很有用。</p> <p>Workfront Fusion当前不提供Retry指令，但可以使用多种变通方法来模拟其功能。 有关详细信息，请参阅Adobe Workfront Fusion中的<a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">重试错误处理</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 目前，错误处理指令不能在错误处理路由之外使用。
>
>   有关详细信息，请参阅Adobe Workfront Fusion中的[错误处理](../../workfront-fusion/errors/error-handling.md)一文中的[错误处理程序路由](../../workfront-fusion/errors/error-handling.md#error)。
>* [!DNL Workfront Fusion]目前不提供使您能够轻松有条件地生成（丢弃）错误的Throw模块，尽管可以使用解决方法来模拟其功能。
>
>   有关详细信息，请参阅Adobe Workfront Fusion[Throw错误处理](../../workfront-fusion/errors/throw.md)一文中的[Throw](../../workfront-fusion/errors/throw.md#workaround-for-throw)解决方法。

## 间断 {#break}

当[!DNL Break]指令处理错误时，会在“未完成执行”文件夹中创建记录。 此记录存储场景执行的状态以及来自先前模块的数据。 记录引用了引发错误的模块，并包含有关模块接收到的数据作为输入的信息。 对于每个导致错误的数据包，将创建一个单独的记录。

有关详细信息，请参阅[在Adobe Workfront Fusion中查看和解决未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

### 解决由Break指令导致的错误

您可以通过更新场景（如果需要）并运行一次来手动解决该错误。

您还可以将方案配置为通过重新执行方案来自动处理不完整的执行。 要配置模块以处理未完成的执行，请执行以下操作：

1. 在Break模块内，启用&#x200B;[!UICONTROL **自动完成执行**]&#x200B;选项。
1. 在&#x200B;**尝试次数**&#x200B;字段中，输入或映射您希望模块重试执行的最大尝试次数

   此数字必须介于1和100之间。
1. 在&#x200B;**尝试间隔**&#x200B;字段中，输入或映射每次重试间隔的分钟数。

启用此选项后，当发生错误时，将检索不完整的执行（在[!UICONTROL 尝试间隔]字段中指定的时间之后）并使用原始输入数据执行。 这将重复执行，直到模块执行完成且无错误或达到指定的尝试次数为止。

>[!NOTE]
>
>如果初始重试尝试失败，重试间隔将每隔一次尝试以指数方式增加。


当“自动完成执行”打开时，场景运行将标记为“成功”，因为Break错误处理程序的自动重试正在自动处理该问题。 在这种情况下，用户不会收到有关失败运行的电子邮件。

关闭“自动完成执行”后，该运行将标记为“警告”。

在“不完整的执行”下存储的执行存在一些异常，对于某些错误类型，无法自动重试场景执行。

有关详细信息，请参阅Adobe Workfront Fusion中的项目[场景设置面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[允许存储不完整的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)。

有关详细信息，请参阅Adobe Workfront Fusion中的[高级错误处理](../../workfront-fusion/errors/advanced-error-handling.md)。
