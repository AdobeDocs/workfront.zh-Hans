---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的“方案设置”面板
description: 本文介绍了 [!UICONTROL 方案设置] 面板中的 [!DNL Adobe Workfront Fusion] 方案。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 4d9832d0870c3fccf847c3932ad4f985a62b9672
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# 中的方案设置面板 [!DNL Adobe Workfront Fusion]

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 对于工作自动化和集成]，[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 打开方案设置

1. 打开场景编辑器，如中所述 [中的方案编辑器 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. 单击页面左下角附近的齿轮图标。

   ![](assets/scenario-settings-350x221.png)

   在 [!UICONTROL 方案设置] 在显示的面板中，您可以为方案配置各种高级设置。

## [!UICONTROL 允许存储未完成的执行]

此选项确定 [!DNL Adobe Workfront Fusion] 如果在执行场景期间发生错误，则进行此处理。 启用此选项后，方案将暂停并移至 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 这使您能够修复问题，并从场景停止的地方继续执行。 如果禁用此选项，则方案运行将停止，并且回滚阶段将启动。

## [!UICONTROL 顺序处理]

此选项确定 [!DNL Workfront Fusion] 如果发生错误并且场景的执行被移至 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). 如果 [!UICONTROL 顺序处理] 选项，在解决所有未完成的执行之前，Workfront Fusion将完全停止处理任务序列。 如果 [!UICONTROL 顺序处理] 选项已禁用，场景会根据其计划继续运行，同时会重复尝试重新运行未完成的执行。

>[!NOTE]
>
>顺序处理可能会导致场景执行延迟。 当即时场景触发或计划场景设置为执行时，如果队列中仍存在未完成的执行，则该场景将在队列中的所有执行完成后执行，然后才在队列中执行。
>
>如果您的方案用例不需要顺序处理，我们建议禁用顺序处理选项。

有关计划的详细信息，请参阅 [在中计划方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 数据是机密的

执行方案后，您可以默认显示有关方案中的模块处理了哪些数据的信息。 如果不希望存储此信息，请启用 [!UICONTROL 数据是机密的] 选项。

有关显示信息的详细信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>如果启用此选项，则可能很难解决在执行场景期间可能发生的错误。

## 启用数据丢失

此选项与启用数据丢失有关，如果 [!DNL Workfront Fusion] 无法将捆绑包保存到的队列 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) （例如，由于缺少可用空间）。 启用此选项后，数据将丢失，以防止整个场景执行过程中的中断。 当最高优先级是连续执行并且传入的错误数据没有那么重要时，此选项非常有用。

除此之外，在执行场景时，模块有时可能会遇到大于最大允许大小的文件。 在本例中， [!DNL Workfront Fusion] 所得款项乃根据中国法律之规定，按 [!UICONTROL 启用数据丢失] 选项，并显示警告消息。

有关最大文件大小的详细信息，请参见 [关于映射文件 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

有关警告的详细信息，请参阅 [在中处理时出错 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL 自动提交]

此 [!UICONTROL 自动提交] 设置应用于事务并定义处理场景的方式。 如果自动提交选项处于打开状态，则每个模块上的提交阶段将在完成操作阶段后立即启动。 禁用自动提交选项后，直到对所有模块执行操作（这是默认模式）后，才会执行提交。

有关事务处理的详细信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 最大循环数

如果您希望防止与第三方服务的连接中断，并确保在同一场景运行内处理所有记录，则设置更多周期会很有用。

* 如果方案以轮询触发器开始，则设置定义方案执行期间允许的最大循环数。

  有关轮询触发器的详细信息，请参见 [轮询触发器](../../workfront-fusion/modules/module-types.md#polling) 在 [模块类型](../../workfront-fusion/modules/module-types.md).

* 如果方案以即时触发器开始，则忽略该设置，并在单个方案执行期间处理所有挂起事件，即每个周期一个事件。

  有关即时触发器的详细信息，请参见 [即时触发器](../../workfront-fusion/modules/module-types.md#instant) 在 [模块类型](../../workfront-fusion/modules/module-types.md).

* 如果方案不以触发器（即时/轮询）开头，则始终执行指定的最大循环数。

>[!INFO]
>
>**示例：**  [!DNL Workfront] > [!UICONTROL 观看记录] 观察出现的新问题，以及 [!DNL Workfront] >[!UICONTROL 转换对象] 将新请求转换为项目并为其分配适当的模板。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL 更多周期] 设置仅在计划场景执行时应用。 当您使用 [!UICONTROL 运行一次] 按钮，循环设置将被考虑在内。
>
>### 最大循环数设置为1（默认）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>此 [!UICONTROL 最大返回文件数] 在 [!UICONTROL Dropbox] >[!UICONTROL 监视文件] 模块设置为 `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>如果向提交100个请求 [!DNL Workfront]，和 [!UICONTROL 限制] 字段设置为10，则运行一个方案后仍有90个文件未处理。 在下次计划场景执行中处理接下来的10个文件。
>
>### 最大循环数设置为10
>
>此 [!UICONTROL 最大返回文件数] 在 [!UICONTROL Dropbox] >[!UICONTROL 监视文件] 模块设置为 `10`.
>
>如果将100个文件添加到Dropbox文件夹，并且 [!UICONTROL 最大返回文件数] 选项设置为10，则在第一个周期内处理10个文件，在第二个周期内处理接下来的10个文件，在第三个周期内处理接下来的10个文件，依此类推，直到处理完所有文件为止。
>
>所有文件都在1个场景运行内处理。
>
>您可以在方案详细信息中查看已运行的周期：
>
>![](assets/scenario-detail-350x207.png)
>
>有关此页面的详细信息，请参阅 [中的方案详细信息 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## 连续错误数

定义在停用场景执行(不包括 [!UICONTROL 数据错误]， [!UICONTROL Duplicatedataerror] 和 [!UICONTROL ConnectionError])。

有关错误的详细信息，请参阅 [在中处理时出错 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>如果方案以即时触发器开始，则忽略设置，并在发生第一个错误后立即停用方案。
