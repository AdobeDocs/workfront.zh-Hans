---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]
description: 的 [!UICONTROL 未完成执行] 文件夹存储由于错误而未成功完成的方案执行。 可以手动或自动解析存储的每次未完成执行。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]

的 [!UICONTROL 未完成执行] 文件夹存储由于错误而未成功完成的方案执行。 可以手动或自动解析存储的每次未完成执行。

>[!NOTE]
>
>默认情况下，会禁用存储未完成的执行。 要启用它，请启用 [!UICONTROL 允许存储未完成的执行] 选项。
>
>有关方案设置的更多信息，请参阅 [中的“方案设置”面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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

## 查看未完成的执行

如果模块在操作过程中遇到错误，则会将新的未完成执行添加到“未完成的执行”文件夹。 每个未完成的执行都包含方案的Blueprint以及可映射到失败模块的所有包。 单击 [!UICONTROL 未完成执行] 选项卡：

![](assets/incomplete-executions-tab-350x102.png)

有关更多信息，请参阅 [导致执行不完整的错误](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>每个组织未解决的未完成执行文件夹的当前大小限制为500 MB。 如果贵组织超出此限制，您可能会看到以下错误：
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>有关更多信息，请参阅 [启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [中的“方案设置”面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 解决未完成的执行

存储新的未完成执行时，您可以按如下方式解析该执行：

1. 单击 **[!UICONTROL 未完成执行]** 选项卡。
1. 找到要解析的未完成执行，然后单击 **[!UICONTROL 详细信息]**.


   如果要在尝试解决未完成的执行之前查看所有模块操作的日志，则可以从 [!UICONTROL 历史] 文件夹：

1. 单击 **[!UICONTROL 历史]** 选项卡。
1. 找到方案失败的执行日志并单击 **[!UICONTROL 详细信息]**.
1. 打开模块的日志，其中显示了模块的所有操作。
1. 找到失败的操作并单击 **[!UICONTROL 解决]**:

   ![](assets/resolve-btn-350x188.png)

## 与未完成执行相关的选项

在 [!UICONTROL 方案设置] 面板可确定是否以及如何存储未完成的执行：

* 允许存储未完成的执行
* 顺序处理
* 启用数据丢失

有关这些选项的更多信息，请参阅 [中的“方案设置”面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 导致执行不完整的错误

存储不完整执行时会出现几类错误。 这些功能可能包括：

* 由于数据不完整或错误而导致的验证错误，主要是因为缺少一个项目，而该项目是为了成功处理通过模块的所有数据而预期会出现的。
* 由于临时或长期连接失败（例如，在与电子邮件或远程FTP服务器的连接期间）而导致最终目标不可用的错误。

如果方案中第一个模块发生错误，则执行会立即停止，并且不会存储不完整的执行。

如果任何其他模块发生错误，并且未附加错误处理程序路由，则会发生以下情况之一：

* 如果错误类型为 `ConnectionError`, `RateLimitError`, `OutOfSpaceError` 或 `ModuleTimeoutError`，则会存储自动重试的不完整执行记录。
* 如果错误类型为 `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`或 `MaxResultsExceededError`，则会存储不会自动重试的不完整执行记录。
* 如果错误类型与上述内容不同，则执行会失败。
