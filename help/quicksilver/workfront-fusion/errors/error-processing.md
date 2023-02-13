---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 处理中的错误 [!DNL Adobe Workfront Fusion]
description: 有时，在执行方案期间可能会发生错误。 如果服务因连接服务失败而不可用或验证失败，则通常会发生这种情况。 本文讨论了您可能遇到的常见错误。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# 处理中的错误 [!DNL Adobe Workfront Fusion]

有时，在执行方案期间可能会发生错误。 如果服务因连接服务失败而不可用或验证失败，则通常会发生这种情况。 本文讨论了您可能遇到的常见错误。

[!DNL Adobe Workfront Fusion] 区分几种基本错误类型。 根据所发生错误的类型，它会做出不同的反应。

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

## 连接错误

`ConnectionError`

连接错误是最常见的错误之一，通常是由于各种原因（过载、维护、中断等）导致第三方服务不可用。 此错误的默认处理方式取决于在哪个模块中遇到该错误：

* 如果第一个模块发生错误，则方案的执行将终止，并显示警告消息。 [!DNL Workfront Fusion] 然后，会反复尝试以增加时间间隔重新运行该方案（如下所述）。 如果所有尝试都失败， [!DNL Workfront Fusion] 停用方案。
* 如果连接错误发生在第一个模块以外的另一个模块上，则后续步骤取决于 [允许存储未完成的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 方案高级设置中的选项：

   * 如果启用了此选项，则方案的执行将移至 [!UICONTROL 未完成执行] 文件夹中 [!DNL Workfront Fusion] 会反复尝试以增加时间间隔重新运行该方案。 如果所有尝试都失败，则执行将保留在 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) 文件夹，等待用户手动解析。
   * 如果禁用了选项，则执行方案后将以错误结束，然后是回滚阶段。 [!DNL Workfront Fusion] 然后，会反复尝试以增加时间间隔重新运行该方案。 如果所有尝试都失败， [!DNL Workfront Fusion] 停用方案。

### 增加时间间隔

在发生错误时多次增加两次尝试之间的时间间隔的算法称为指数回退。 增加的时间间隔设置如下：

1. 10分钟
1. 1 小时
1. 3 小时
1. 12 小时
1. 24 小时

中国采用时间间隔增加的主要原因 [!DNL Workfront Fusion] 是防止频繁执行的方案对反复失败的尝试使用操作。

>[!INFO]
>
>**示例:**
>
>方案包含 [!DNL Google Sheets] 触发器 [!UICONTROL 监视行]. [!DNL Google Sheets] 30分钟内不可用，因为 [!DNL Workfront Fusion] 启动方案，因此无法检索新行。 此方案将在10分钟后停止并重试。 由于服务在此时间范围内仍然不可用， [!DNL Workfront Fusion] 仍无法获取有关新行的信息。 方案的下一次运行将在1小时内计划进行。 [!DNL Google Sheets] 此时间内将再次可用，并且方案成功运行。

## 数据错误

`DataError`

当项目映射不正确且未通过对执行的验证时，会生成数据错误 [!DNL Workfront Fusion] 第三方服务的侧面或侧面。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

如果发生此错误，则方案（模块失败的位置）会移至未完成的执行文件夹，您可以在该文件夹中对问题进行故障诊断。 但是，此方案不会停止，并会继续根据其计划运行。 要在出现“数据错误”时停止执行方案，请在“方案”设置面板中启用“顺序处理”选项。

如果尚未启用 [!UICONTROL 允许存储未完成的执行] 方案设置中的选项时，方案的执行将终止，并执行回滚。

有关未完成执行的信息，请参阅 [查看和解决Adobe Workfront Fusion中未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

有关方案设置面板的信息，请参阅 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

有关计划的信息，请参阅 [在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 重复数据错误

`DuplicateDataError`

如果 [!DNL Workfront Fusion] 尝试将同一包插入两次不允许重复数据的服务时，会生成重复数据错误。 如果发生此错误， [!DNL Workfront Fusion] 会像处理数据错误一样进行。

## 访问令牌错误无效

`InvalidAccessTokenError`

访问令牌错误在 [!DNL Workfront Fusion] 无法访问在第三方服务中注册的帐户。 通常情况下，当您撤消 [!DNL Workfront Fusion] 在给定服务的管理中，但相关方案会按计划继续运行。

如果发生此错误，将立即停止执行方案。 从发生错误的模块开始的方案的其余部分将移至未完成的执行文件夹。

有关未完成执行的信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## 速率限制错误

`RateLimitError`

如果超出给定服务设置的限制，则会生成速率限制错误。 如果发生此错误， [!DNL Workfront Fusion] 以与连接错误相同的方式进行。 有关更多信息，请参阅 [连接错误](#connection-error).

## 数据错误不完整

`IncompleteDataError`

仅触发器出现数据错误不完整。 如果触发器无法从给定服务下载所需数据，则会生成此错误。

如果方案终止时使用 `IncompleteDataError`，则其进一步行为将取决于其设置 [!UICONTROL 连续错误的最大数量]. 有关更多信息，请参阅 [连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**示例：** 一种情况是 [!DNL Workfront] 触发器 [!UICONTROL 观看记录] 设置为监视文档。 在您上传大型文档（如长视频）时，会执行此方案。 因为 [!UICONTROL Workfront Fusion] 当视频仍在上传到Workfront时，该方案会终止，因为 `IncompleteDataError`.

## 运行时错误

`RuntimeError`

如果在方案执行期间出现任何其他错误（如上所述），则将报告为 `RunTimeError`.

如果方案终止时使用 `RuntimeError`，则其进一步行为将取决于其设置 [!UICONTROL 连续错误的最大数量]. 有关更多信息，请参阅 [连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>如果方案以即时触发器开头，则 [!UICONTROL 连续错误的最大数量] 将忽略，并在发生第一个错误后立即停用该方案。 有关更多信息，请参阅 [即时触发器](../../workfront-fusion/modules/module-types.md#instant) 在文章中 [模块类型](../../workfront-fusion/modules/module-types.md).

## 不一致错误

`InconsistencyError`

如果在提交或回滚阶段发生上述任何错误，则方案将终止，出现“不一致错误”。 有关更多信息，请参阅 [方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

如果出现此错误，则会立即停止执行该方案。

## 警告

在执行方案时，您可能会收到一则警告，通知您问题。 但是，它并不会阻止成功完成该方案。

例如，当超出允许的最大文件大小并且 [!UICONTROL 启用数据丢失] 选项。 有关更多信息，请参阅 [启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).
