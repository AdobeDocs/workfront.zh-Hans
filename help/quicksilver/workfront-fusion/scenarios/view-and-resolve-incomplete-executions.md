---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 查看并解决 [!DNL Adobe Workfront Fusion]中未完成的执行
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 5%

---

# 查看并解决[!DNL Adobe Workfront Fusion]中未完成的执行

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [查看并解决未完成的执行](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-and-resolve-incomplete-executions.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

[!UICONTROL 未完成的执行]文件夹存储由于错误未成功完成的场景执行。 可以手动或自动解决每个存储的不完整执行。

>[!NOTE]
>
>默认情况下，不完整执行的存储被禁用。 要启用它，请在场景高级设置中启用[!UICONTROL 允许存储未完成的执行]选项。
>
>有关方案设置的详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板。

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

## 查看未完成的执行

如果模块在操作过程中遇到错误，则会将新的未完成执行添加到“未完成执行”文件夹。 每个不完整的执行都包含场景的Blueprint以及可以映射到失败模块的所有捆绑包。 通过单击场景详细信息页面上的[!UICONTROL 未完成的执行]选项卡，可以打开未完成的执行列表。

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

有关详细信息，请参阅[导致执行不完整的错误](#errors-resulting-into-incomplete-executions)。

>[!NOTE]
>
>每个组织未解决的执行文件夹当前的大小限制为500 MB。 如果贵组织超过此限制，您可能会看到以下错误：
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板中的[启用数据丢失](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)。

## 解决未完成的执行

在存储新的未完成执行时，您可以按如下方式解决它：

1. 单击&#x200B;**[!UICONTROL 未完成的执行]**&#x200B;选项卡。
1. 找到要解析的未完成执行，然后单击&#x200B;**[!UICONTROL 详细信息]**。


   如果您想在尝试解析未完成的执行之前查看所有模块操作的日志，可以从[!UICONTROL History]文件夹解析未完成执行：

1. 单击&#x200B;**[!UICONTROL 历史记录]**&#x200B;选项卡。
1. 找到方案的失败执行日志，然后单击&#x200B;**[!UICONTROL 详细信息]**。
1. 打开模块的日志，其中显示了模块的所有操作。
1. 找到失败的操作，然后单击&#x200B;**[!UICONTROL 解决]**：

   ![](assets/resolve-btn-350x188.png)

## 与未完成执行相关的选项

[!UICONTROL 场景设置]面板中的以下选项确定是否以及如何存储未完成的执行：

* 允许存储未完成的执行
* 顺序处理
* 启用数据丢失

有关这些选项的更多信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板。

## 导致执行不完整的错误

有几类错误会导致存储不完整的执行。 这些可能包括：

* 验证错误由不完整或错误的数据引起，主要原因是需要缺少项目才能成功处理通过模块的所有数据。
* 由于临时或长期连接故障（例如，在连接电子邮件或远程FTP服务器期间）导致最终目标不可用而发生错误。

如果场景中的第一个模块发生错误，则执行会立即停止，并且不会存储未完成的执行。

如果任何其他模块发生错误，并且没有附加错误处理程序路由，则会出现以下情况之一：

* 如果错误类型为`ConnectionError`、`RateLimitError`、`OutOfSpaceError`或`ModuleTimeoutError`，则存储具有自动重试的不完整执行记录。
* 如果错误类型为`DataError`、`InvalidConfigurationError`、`InvalidAccessTokenError`、`UnexpectedError`、`MaxFileSizeExceededError`或`MaxResultsExceededError`，则存储了不完整的执行记录而不进行自动重试。
* 如果错误类型不是上述类型，则执行失败。
