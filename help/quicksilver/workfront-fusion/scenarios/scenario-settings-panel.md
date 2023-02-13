---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的“方案设置”面板
description: 本文介绍了 [!UICONTROL 方案设置] 面板 [!DNL Adobe Workfront Fusion] 方案。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# 中的“方案设置”面板 [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 打开方案设置

1. 打开方案编辑器，如 [中的方案编辑器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. 单击页面左下角附近的齿轮图标。

   ![](assets/scenario-settings-350x221.png)

   在 [!UICONTROL 方案设置] 面板中，您可以为方案配置各种高级设置。

## [!UICONTROL 允许存储未完成的执行]

此选项决定如何 [!DNL Adobe Workfront Fusion] 如果在执行方案期间发生错误，则会继续。 启用此选项后，方案将暂停并移至 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 这样，您就可以修复问题并继续从方案停止的位置执行。 如果禁用此选项，则方案将停止运行并启动回滚阶段。

## [!UICONTROL 顺序处理]

此选项决定如何 [!DNL Workfront Fusion] 如果发生错误并且方案的执行被移至 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 如果 [!UICONTROL 顺序处理] 选项时，Workfront Fusion会完全停止处理任务序列，直到所有未完成的执行都得到解决。 如果 [!UICONTROL 顺序处理] 选项时，方案会继续根据其计划运行，并会反复尝试重新运行未完成的执行。

有关计划的详细信息，请参阅 [在中计划方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 数据是保密的

执行方案后，默认情况下可以显示有关方案中模块处理了哪些数据的信息。 如果不希望存储此信息，请启用 [!UICONTROL 数据是保密的] 选项。

有关显示信息的更多信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>如果启用此选项，则可能很难解决在执行方案期间可能出现的错误。

## 启用数据丢失

此选项与启用数据丢失(如果 [!DNL Workfront Fusion] 无法将包保存到的队列 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) （例如，由于缺少可用空间）。 启用此选项后，数据将丢失，以防止整个方案执行中断。 当最高优先级是连续执行，而传入的错误数据不那么重要时，此方法非常有用。

除此之外，在执行方案时，模块有时可能会遇到大于允许的最大大小的文件。 在这种情况下， [!DNL Workfront Fusion] 款项，以按 [!UICONTROL 启用数据丢失] 选项，此时会显示警告消息。

有关最大文件大小的更多信息，请参阅 [关于在中映射文件 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

有关警告的更多信息，请参阅 [处理中的错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL 自动提交]

的 [!UICONTROL 自动提交] 设置适用于事务，并定义处理方案的方式。 如果“自动提交”选项处于打开状态，则每个模块的提交阶段在完成操作阶段后立即开始。 禁用“自动提交”选项后，在对所有模块执行操作（这是默认模式）之前，不会执行提交。

有关交易的详细信息，请参阅 [方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 最大循环数

如果要防止与第三方服务的连接中断并确保在一个方案运行中处理所有记录，则设置更多周期会非常有用。

* 如果方案以轮询触发器开头，则设置定义在方案执行期间允许的最大循环数。

   有关轮询触发器的更多信息，请参阅 [轮询触发器](../../workfront-fusion/modules/module-types.md#polling) in [模块类型](../../workfront-fusion/modules/module-types.md).

* 如果方案以即时触发器开始，则将忽略该设置，并在单个方案执行期间处理所有挂起事件，即每个周期处理一个事件。

   有关即时触发器的更多信息，请参阅 [即时触发器](../../workfront-fusion/modules/module-types.md#instant) in [模块类型](../../workfront-fusion/modules/module-types.md).

* 如果方案不以触发器（即时/轮询）开头，则始终执行指定的最大循环数。

>[!INFO]
>
>**示例：**  [!DNL Workfront] > [!UICONTROL 观看记录] 监视新发行， [!DNL Workfront] >[!UICONTROL 转换对象] 将新请求转换为项目，并为其分配相应的模板。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL 更多周期] 设置仅在您计划方案执行时应用。 当您使用 [!UICONTROL 运行一次] 按钮，则会考虑周期设置。
>
>### 最大周期数设置为1（默认）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>的 [!UICONTROL 返回文件的最大数量] 在 [!UICONTROL Dropbox] >[!UICONTROL 监视文件] 模块设置为 `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>如果向 [!DNL Workfront]和 [!UICONTROL 限制] 字段设置为10，则在运行一个方案后，90个文件将保留未处理。 在下一个计划方案执行中将处理接下来的10个文件。
>
>### 最大循环数设置为10
>
>的 [!UICONTROL 返回文件的最大数量] 在 [!UICONTROL Dropbox] >[!UICONTROL 监视文件] 模块设置为 `10`.
>
>如果将100个文件添加到Dropbox文件夹，并 [!UICONTROL 返回文件的最大数量] 选项设置为10，则在第一个周期期间处理10个文件，在第二个周期中处理下一个10个文件，在第三个周期中处理下一个10个文件，依此类推，直到所有文件都被处理。
>
>在1个方案运行中会处理所有文件。
>
>您可以在方案详细信息中查看已运行的周期：
>
>![](assets/scenario-detail-350x207.png)
>
>有关此页面的更多信息，请参阅 [中的方案详细信息 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## 连续错误数

定义在停用方案执行之前连续执行尝试的最大次数(不包括 [!UICONTROL 数据错误], [!UICONTROL DuplicateDataError] 和 [!UICONTROL 连接错误])。

有关错误的更多信息，请参阅 [处理中的错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>如果方案以即时触发器开头，则会忽略该设置，并在发生第一个错误后立即停用该方案。
