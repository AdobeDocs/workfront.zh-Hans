---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的“方案设置”面板
description: 本文介绍了在您的 [!DNL Adobe Workfront Fusion] 方案中的[!UICONTROL 方案设置]面板中可用的设置。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 1b729960a23e43252bda16d9bfb7ca9656a115a1
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的方案设置面板

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
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 打开方案设置

1. 打开方案编辑器，如[方案编辑器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)中所述。
1. 单击页面左下角附近的齿轮图标。

   ![](assets/scenario-settings-350x221.png)

   在显示的[!UICONTROL 方案设置]面板中，您可以为该方案配置各种高级设置。

## [!UICONTROL 允许存储未完成的执行]

此选项确定在执行场景期间发生错误时[!DNL Adobe Workfront Fusion]如何进行。 启用此选项后，方案将暂停并移动到[查看并解决 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中未完成的执行。 这使您能够修复问题，并从场景停止的地方继续执行。 如果禁用此选项，则方案运行将停止，并且回滚阶段将启动。

## [!UICONTROL 连续处理]

此选项确定[!DNL Workfront Fusion]在发生错误并且场景的执行被移到[查看并解决 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中的未完成执行时如何进行。 如果启用了[!UICONTROL 连续处理]选项，Workfront Fusion将完全停止处理任务序列，直到解决所有未完成的执行。 如果[!UICONTROL 连续处理]选项被禁用，则场景将根据其计划继续运行，同时会重复尝试重新运行未完成的执行。

>[!NOTE]
>
>顺序处理可能会导致场景执行延迟。 当即时场景触发或计划场景设置为执行时，如果队列中仍存在未完成的执行，则该场景将在队列中的所有执行完成后执行，然后才在队列中执行。
>
>如果您的方案用例不需要顺序处理，我们建议禁用顺序处理选项。

有关计划的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中计划方案。

## 数据是机密的

执行方案后，您可以默认显示有关方案中的模块处理了哪些数据的信息。 如果不希望存储此信息，请启用[!UICONTROL 数据是机密的]选项。

有关显示信息的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[方案执行流。

>[!IMPORTANT]
>
>如果启用此选项，则可能很难解决在执行场景期间可能发生的错误。

## 启用数据丢失

此选项与启用数据丢失有关，如果[!DNL Workfront Fusion]无法将包保存到[查看队列并解决 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中未完成的执行（例如，由于缺少可用空间）。 启用此选项后，数据将丢失，以防止整个场景执行过程中的中断。 当最高优先级是连续执行并且传入的错误数据没有那么重要时，此选项非常有用。

除此之外，在执行场景时，模块有时可能会遇到大于最大允许大小的文件。 在这种情况下，[!DNL Workfront Fusion]按照[!UICONTROL 启用数据丢失]选项的设置继续进行，并显示一条警告消息。

有关最大文件大小的详细信息，请参阅[关于在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md)中映射文件。

有关警告的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中的[错误处理。

## [!UICONTROL 自动提交]

[!UICONTROL 自动提交]设置适用于事务并定义处理方案的方法。 如果自动提交选项处于打开状态，则每个模块上的提交阶段将在完成操作阶段后立即启动。 禁用自动提交选项后，直到对所有模块执行操作（这是默认模式）后，才会执行提交。

有关事务的详细信息，请参阅[方案执行、周期和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的阶段。

## 最大循环数

如果您希望防止与第三方服务的连接中断，并确保在同一场景运行内处理所有记录，则设置更多周期会很有用。

* 如果方案以轮询触发器开始，则设置定义方案执行期间允许的最大循环数。

  有关轮询触发器的详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)中的[轮询触发器](../../workfront-fusion/modules/module-types.md#polling)。

* 如果方案以即时触发器开始，则忽略该设置，并在单个方案执行期间处理所有挂起事件，即每个周期一个事件。

  有关即时触发器的详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)中的[即时触发器](../../workfront-fusion/modules/module-types.md#instant)。

* 如果方案不以触发器（即时/轮询）开头，则始终执行指定的最大循环数。

>[!INFO]
>
>**示例：** [!DNL Workfront] > [!UICONTROL 监视记录]监视新出现的问题，并且[!DNL Workfront] >[!UICONTROL 转换对象]将新请求转换为项目并为其分配适当的模板。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>仅当您计划方案执行时，才应用[!UICONTROL 更多周期]设置。 当您使用[!UICONTROL 运行一次]按钮时，周期设置将被考虑在内。
>
>### 最大循环数设置为1（默认）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL Workfront] >[!UICONTROL 监视记录]模块中的[!UICONTROL 返回文件的最大数量]设置为`10`。
>如果向[!DNL Workfront]提交了100个请求，且[!UICONTROL 限制]字段设置为10，则运行一个方案后仍有90个文件未处理。 在下次计划场景执行中处理接下来的10个文件。
>
>### 最大循环数设置为10
>
>[!UICONTROL Dropbox] >[!UICONTROL 监视文件]模块中的[!UICONTROL 最大返回文件数]设置为`10`。
>
>如果向Dropbox文件夹添加了100个文件，并且将[!UICONTROL 返回的最大文件数]选项设置为10，则会在第一个周期处理10个文件，在第二个周期处理下一个10个文件，在第三个周期处理下一个10个文件，依此类推，直到处理完所有文件为止。
>
>所有文件都在1个场景运行内处理。
>
>您可以在方案详细信息中查看已运行的周期：
>
>![](assets/scenario-detail-350x207.png)
>
>有关此页面的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)中的[方案详细信息。

## 连续错误数

定义在停用方案的执行之前连续执行尝试的最大次数（不包括[!UICONTROL DataError]、[!UICONTROL DuplicateDataError]和[!UICONTROL ConnectionError]）。

有关错误的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中的[错误处理。

>[!NOTE]
>
>如果方案以即时触发器开始，则忽略设置，并在发生第一个错误后立即停用方案。
