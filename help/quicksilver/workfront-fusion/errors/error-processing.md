---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 处理以下对象时出错： [!DNL Adobe Workfront Fusion]
description: 有时，在执行场景期间可能会出错。 如果服务由于无法连接到服务而不可用，或者验证失败，则通常会发生这种情况。 本文讨论您可能会遇到的常见错误。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# 处理以下对象时出错： [!DNL Adobe Workfront Fusion]

有时，在执行场景期间可能会出错。 如果服务由于无法连接到服务而不可用，或者验证失败，则通常会发生这种情况。 本文讨论您可能会遇到的常见错误。

[!DNL Adobe Workfront Fusion] 区分几种基本错误类型。 它会根据发生的错误类型做出不同的反应。

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

## 连接错误

`ConnectionError`

连接错误是最常见的错误之一，通常是由于多种原因（过载、维护、中断等）导致第三方服务不可用。 此错误的默认处理方式取决于遇到的模块：

* 如果在第一个模块中发生错误，则场景的执行将终止，并显示一条警告消息。 [!DNL Workfront Fusion] 然后反复尝试以递增的时间间隔重新运行场景（下面对此进行了说明）。 如果所有尝试都失败， [!DNL Workfront Fusion] 取消激活方案。
* 如果连接错误发生在第一个模块以外的其他模块，则后续步骤取决于 [允许存储未完成的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 方案高级设置中的选项：

   * 如果启用了此选项，则场景的执行将移至 [!UICONTROL 未完成的执行] 文件夹位置 [!DNL Workfront Fusion] 不断尝试以递增的时间间隔重新运行场景。 如果所有尝试都失败，执行将保留在“未完成执行”文件夹中，等待用户手动解析。

     有关未完成执行的更多信息，请参阅 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * 如果禁用了此选项，则场景的执行将结束并出现一个错误，然后进入回滚阶段。 [!DNL Workfront Fusion] 然后反复尝试以递增的时间间隔重新运行场景。 如果所有尝试都失败， [!DNL Workfront Fusion] 取消激活方案。

### 增加时间间隔

当出现错误时，多次增加两次尝试之间的时间间隔的算法称为指数回退。 递增时间间隔的设置如下：

1. 10分钟
1. 1 小时
1. 3 小时
1. 12 小时
1. 24 小时

采用递增时间间隔的主要原因在于 [!DNL Workfront Fusion] 是为了防止频繁执行的场景在多次失败的尝试上消耗操作。

>[!INFO]
>
>**示例:**
>
>场景包含 [!DNL Google Sheets] 触发器 [!UICONTROL 监视行]. [!DNL Google Sheets] 在以下情况下，由于进行维护，30分钟内不可用 [!DNL Workfront Fusion] 启动方案，因此无法检索新行。 该场景将停止并在10分钟后重试。 因为 [!DNL Google Sheets] 仍然不可用， [!DNL Workfront Fusion] 仍无法获取有关新行的信息。 计划的下次运行时间为1小时。 [!DNL Google Sheets] 此时再次可用，并且场景成功运行。

## 数据错误

`DataError`

当项目被错误映射并且未通过在上执行的验证时，会生成数据错误。 [!DNL Workfront Fusion] 正在使用第三方服务的一方或一方。

如果发生此错误，则将场景（直到模块失败的地方）移至不完整执行文件夹，您可以在其中解决该问题。 但是，该场景不会停止，而是继续按照其计划运行。 要在出现数据错误时停止方案的执行，请启用方案设置面板中的顺序处理选项。

如果您尚未启用 [!UICONTROL 允许存储未完成的执行] 方案设置中的选项，方案的执行因错误而终止，并会执行回滚。

有关映射的详细信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

有关未完成执行的信息，请参见 [在Adobe Workfront Fusion中查看和解决未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

有关“场景”设置面板的信息，请参阅 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

有关时间表的信息，请参阅 [在Adobe Workfront Fusion中计划场景](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 复制数据错误

`DuplicateDataError`

如果 [!DNL Workfront Fusion] 尝试将同一捆绑包两次插入到不允许重复数据的服务中，会生成重复数据错误。 如果出现此错误， [!DNL Workfront Fusion] 执行的方式与处理数据错误时相同。

## 访问令牌无效错误

`InvalidAccessTokenError`

出现以下情况时，出现无效的访问令牌错误 [!DNL Workfront Fusion] 无法访问您在第三方服务中注册的帐户。 这通常发生在您撤销对的访问权限时 [!DNL Workfront Fusion] 在管理给定服务时，但相关场景会按计划继续运行。

如果发生此错误，将立即停止执行方案。 从发生错误的模块开始的场景的其余部分被移至未完成执行文件夹。

有关未完成执行的信息，请参见 [在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## 速率限制错误

`RateLimitError`

如果超过给定服务设置的限制，则会生成速率限制错误。 如果发生此错误， [!DNL Workfront Fusion] 与处理连接错误时相同。

有关更多信息，请参阅 [连接错误](#connection-error).

## 不完整数据错误

`IncompleteDataError`

只有触发器出现不完整数据错误。 如果触发器无法从给定服务下载所需数据，则会生成此错误。

如果场景终止于 `IncompleteDataError`，则其进一步行为将取决于其设置 [!UICONTROL 最大连续错误数].

有关更多信息，请参阅 [连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**示例:**
>
>方案具有 [!DNL Workfront] 触发器 [!UICONTROL 观看记录] 设置为监视文档。 场景将在您上传大型文档（如长视频）时执行。 因为 [!UICONTROL Workfront Fusion] 尝试在视频仍上传到Workfront时下载视频，场景通过以下方式终止 `IncompleteDataError`.

## 运行时错误

`RuntimeError`

如果在场景执行期间出现任何其他错误（未提及），则会报告为 `RunTimeError`.

如果场景终止于 `RuntimeError`，则其进一步行为将取决于其设置 [!UICONTROL 最大连续错误数]. 有关更多信息，请参阅 [连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>如果场景以即时触发器开头，则设置为 [!UICONTROL 最大连续错误数] 将被忽略，一旦发生第一个错误，将立即停用场景。 有关更多信息，请参阅 [即时触发器](../../workfront-fusion/modules/module-types.md#instant) 在文章中 [模块类型](../../workfront-fusion/modules/module-types.md).

## 不一致错误

`InconsistencyError`

如果在提交或回滚阶段发生上述任何错误，则场景将终止并显示不一致错误。 有关更多信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

如果场景中出现此错误，则场景的执行将立即停止。

## 警告

在执行场景时，您可能会收到一则警告消息，向您通知问题。 但是，它不会阻止场景成功完成。

例如，当超出允许的最大文件大小且超过 [!UICONTROL 启用数据丢失] 选项已禁用。 有关更多信息，请参阅 [启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 在文章中 [Adobe Workfront Fusion中的“方案设置”面板](../../workfront-fusion/scenarios/scenario-settings-panel.md).
