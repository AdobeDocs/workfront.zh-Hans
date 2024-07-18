---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: 在 [!DNL Adobe Workfront Fusion]中处理时出错
description: 有时，在执行场景期间可能会出错。 如果由于无法连接到服务而导致服务不可用，或者如果验证失败，则通常会发生这种情况。 本文讨论您可能会遇到的常见错误。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中处理时出错

有时，在执行场景期间可能会出错。 如果由于无法连接到服务而导致服务不可用，或者如果验证失败，则通常会发生这种情况。 本文讨论您可能会遇到的常见错误。

[!DNL Adobe Workfront Fusion]可区分几种基本错误类型。 它会根据发生的错误类型做出不同的反应。

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

## 连接错误

`ConnectionError`

连接错误是最常见的错误之一，这些错误通常是由多种原因（过载、维护、中断等）导致第三方服务不可用造成的。 此错误的默认处理取决于遇到的模块：

* 如果第一个模块发生错误，则场景的执行将终止，并显示警告消息。 然后[!DNL Workfront Fusion]反复尝试以递增的时间间隔重新运行该方案（下面对此进行了说明）。 如果所有尝试都失败，[!DNL Workfront Fusion]将停用该方案。
* 如果连接错误发生在第一个模块以外的其他模块上，则后续步骤取决于场景高级设置中的[允许存储不完整的执行](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)选项：

   * 如果启用了此选项，则方案的执行将移到[!UICONTROL 未完成的执行]文件夹，其中[!DNL Workfront Fusion]反复尝试以递增的时间间隔重新运行方案。 如果所有尝试都失败，执行将保留在“未完成执行”文件夹中，等待用户手动解析。

     有关未完成执行的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中查看和解决未完成的执行。
   * 如果禁用了此选项，则场景的执行将结束并返回错误，然后进入回滚阶段。 然后，[!DNL Workfront Fusion]反复尝试以递增的时间间隔重新运行该方案。 如果所有尝试都失败，[!DNL Workfront Fusion]将停用该方案。

### 增加时间间隔

当出现错误时，将两次尝试之间的时间间隔乘以递增的算法称为指数回退。 增加的时间间隔设置如下：

1. 10分钟
1. 1 小时
1. 3 小时
1. 12 小时
1. 24 小时

在[!DNL Workfront Fusion]中使用增加的时间间隔的主要原因是防止频繁执行的场景在多次失败的尝试时占用操作。

>[!INFO]
>
>**示例：**
>
>方案包含[!DNL Google Sheets]触发器[!UICONTROL 监视行]。 由于在[!DNL Workfront Fusion]启动方案时进行了维护，[!DNL Google Sheets]在30分钟内不可用，因此无法检索新行。 场景将停止并在10分钟后重试。 由于[!DNL Google Sheets]仍然不可用，[!DNL Workfront Fusion]仍无法获取有关新行的信息。 方案的下次运行安排在1小时内。 [!DNL Google Sheets]此时再次可用，并且方案成功运行。

## 数据错误

`DataError`

如果项目未正确映射，并且未通过在[!DNL Workfront Fusion]端或正在使用的第三方服务端执行的验证，则会生成数据错误。

如果发生此错误，则将场景（直到模块失败）移至未完成执行文件夹，您可以在其中解决问题。 但是，场景不会停止，并且会按照其计划继续运行。 要在出现数据错误时停止方案的执行，请启用方案设置面板中的顺序处理选项。

如果尚未在方案设置中启用[!UICONTROL 允许存储不完整的执行]选项，则方案的执行将终止，并出现错误，同时会执行回滚。

有关映射的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

有关未完成执行的信息，请参阅[在Adobe Workfront Fusion中查看和解决未完成的执行](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)。

有关方案设置面板的信息，请参阅[Adobe Workfront Fusion中的方案设置面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)。

有关计划的信息，请参阅[在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md)。

## 重复数据错误

`DuplicateDataError`

如果[!DNL Workfront Fusion]尝试将同一捆绑包两次插入到不允许重复数据的服务中，则会生成重复数据错误。 如果发生此错误，[!DNL Workfront Fusion]将以与处理数据错误相同的方式进行。

## 访问令牌无效错误

`InvalidAccessTokenError`

当[!DNL Workfront Fusion]无法访问您在第三方服务中注册的帐户时，会发生访问令牌无效错误。 这通常发生在您在管理给定服务时撤销[!DNL Workfront Fusion]的访问权限时，但相关方案仍按计划运行。

如果发生此错误，将立即停止执行方案。 从发生错误的模块开始的场景的其余部分被移至未完成执行文件夹。

有关未完成执行的信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)中查看和解决未完成的执行。

## 速率限制错误

`RateLimitError`

如果超过给定服务设置的限制，则会生成速率限制错误。 如果发生此错误，[!DNL Workfront Fusion]将以与处理连接错误相同的方式进行。

有关详细信息，请参阅[连接错误](#connection-error)。

## 不完整数据错误

`IncompleteDataError`

只有触发器出现不完整数据错误。 如果触发器无法从给定服务下载所需数据，则会生成此错误。

如果方案以`IncompleteDataError`终止，则其进一步的行为将取决于其设置[!UICONTROL 最大连续错误数]。

有关详细信息，请参阅Adobe Workfront Fusion[方案设置面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的文章[连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)。

>[!INFO]
>
>**示例：**
>
>方案将[!DNL Workfront]触发器[!UICONTROL 监视记录]设置为监视文档。 场景在上传大文档（如长视频）时执行。 由于[!UICONTROL Workfront Fusion]尝试在视频仍上传到Workfront时下载视频，因此场景将通过`IncompleteDataError`终止。

## 运行时错误

`RuntimeError`

如果在场景执行期间出现任何其他错误（未提及），则将其报告为`RunTimeError`。

如果方案以`RuntimeError`终止，则其进一步的行为将取决于其设置[!UICONTROL 最大连续错误数]。 有关详细信息，请参阅Adobe Workfront Fusion[方案设置面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的文章[连续错误数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)。

>[!NOTE]
>
>如果方案以即时触发器开头，将忽略[!UICONTROL 最大连续错误数]的设置，并在发生第一个错误后立即停用该方案。 有关详细信息，请参阅文章[模块类型](../../workfront-fusion/modules/module-types.md)中的[即时触发器](../../workfront-fusion/modules/module-types.md#instant)。

## 不一致性错误

`InconsistencyError`

如果在提交或回滚阶段发生上述任何错误，则场景将终止，并出现不一致错误。 有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的[方案执行、周期和阶段。

如果某个场景中出现此错误，则该场景的执行将立即停止。

## 警告

在执行场景时，您可能会收到一则警告消息，向您通知问题。 但是，它不会阻止场景成功完成。

例如，如果超过允许的最大文件大小，并且禁用了[!UICONTROL 启用数据丢失]选项，则会显示警告。 有关详细信息，请参阅Adobe Workfront Fusion[方案设置面板](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的文章[启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)。
