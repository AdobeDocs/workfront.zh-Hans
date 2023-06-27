---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]
description: 此 [!UICONTROL 未完成的执行] 文件夹存储由于错误未成功完成的场景执行。 可以手动或自动解决每个存储的不完整执行。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# 在中查看和解决未完成的执行 [!DNL Adobe Workfront Fusion]

此 [!UICONTROL 未完成的执行] 文件夹存储由于错误未成功完成的场景执行。 可以手动或自动解决每个存储的不完整执行。

>[!NOTE]
>
>默认情况下，不完整执行的存储处于禁用状态。 要启用该功能，请启用 [!UICONTROL 允许存储未完成的执行] 方案高级设置中的选项。
>
>有关方案设置的详细信息，请参见 [中的方案设置面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
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

## 查看未完成的执行

如果模块在操作过程中遇到错误，则会将新的未完成执行添加到未完成执行文件夹。 每个不完整的执行都包含场景的Blueprint以及可以映射到失败模块的所有捆绑包。 未完成执行的列表可以通过单击 [!UICONTROL 未完成的执行] “方案详细信息”页面上的选项卡：

![](assets/incomplete-executions-tab-350x102.png)

有关更多信息，请参阅 [导致执行不完整的错误](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>每个组织未解析的未完成执行文件夹的当前大小限制为500 MB。 如果贵组织超过此限制，您可能会看到以下错误：
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>有关更多信息，请参阅 [启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 在 [中的方案设置面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 解决未完成的执行

在存储新的未完成执行时，您可以按如下方式解决它：

1. 单击 **[!UICONTROL 未完成的执行]** 选项卡。
1. 找到要解析的未完成执行，然后单击 **[!UICONTROL 详细信息]**.


   如果您想在尝试解决未完成的执行之前查看所有模块操作的日志，可以从以下位置解决未完成执行 [!UICONTROL 历史记录] 文件夹：

1. 单击 **[!UICONTROL 历史记录]** 选项卡。
1. 找到方案的失败执行日志，然后单击 **[!UICONTROL 详细信息]**.
1. 打开模块的日志，其中显示了模块的所有操作。
1. 找到失败的操作，然后单击 **[!UICONTROL 解决]**：

   ![](assets/resolve-btn-350x188.png)

## 与未完成执行相关的选项

中的以下选项 [!UICONTROL 方案设置] 面板确定是否以及如何存储未完成的执行：

* 允许存储未完成的执行
* 顺序处理
* 启用数据丢失

有关这些选项的详细信息，请参阅 [中的方案设置面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 导致执行不完整的错误

有几类错误会导致存储不完整的执行。 这些可能包括：

* 验证错误由不完整或错误的数据引起，主要原因是缺少预期用于成功处理通过模块的所有数据的项。
* 由于临时或长期连接故障（例如，连接到电子邮件或远程FTP服务器期间）导致最终目标不可用而发生的错误。

如果场景中的第一个模块发生错误，执行将立即停止，并且不会存储不完整的执行。

如果任何其他模块发生错误，并且没有附加错误处理程序路由，则会出现以下情况之一：

* 如果错误类型为 `ConnectionError`， `RateLimitError`， `OutOfSpaceError` 或 `ModuleTimeoutError`，存储了包含自动重试的不完整执行记录。
* 如果错误类型为 `DataError`， `InvalidConfigurationError`， `InvalidAccessTokenError`， `UnexpectedError`， `MaxFileSizeExceededError`，或 `MaxResultsExceededError`，存储不完整的执行记录而不自动重试。
* 如果错误类型不是上述类型，则执行失败。
