---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的场景执行流程
description: 本文介绍了场景的执行方式以及数据流通过场景的方式。 它还介绍了可在何处找到有关已处理数据的信息以及如何读取该信息。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的方案执行流

本文介绍了场景的执行方式以及数据流通过场景的方式。 它还介绍了可在何处找到有关已处理数据的信息以及如何读取该信息。

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

## 方案执行流程

正确设置并激活场景后，该场景将根据其定义的计划执行。

在场景开始时，第一个模块会响应已设置为监视的事件。 如果它返回任何捆绑包（数据），则它们会传递到下一个模块，并且场景会继续，逐个通过每个后续模块传递捆绑包。

如果捆绑包在所有模块中正确处理，则将在“方案详细信息”区域中将该方案标记为成功，如 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md)中的[方案详细信息中所述。

* 有关设置方案的详细信息，请参阅[方案编辑器位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md)。
* 有关激活方案的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)中激活或停用方案。
* 有关计划方案的详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md)中计划方案。
* 有关模块的详细信息，请参阅[模块类型](../../workfront-fusion/modules/module-types.md)。

### 示例：工作自动化]的[!UICONTROL [!DNL Workfront Fusion]

>[!INFO]
>
>**示例：**&#x200B;在监视[!DNL Workfront]中的传入请求然后将其转换为[!DNL Workfront]项目的场景中，数据将按如下方式流动。
>
>场景的第一步由第一个模块执行，即监视请求。 传入的每个请求都视为一个捆绑包。 如果模块运行时未找到任何捆绑包，则场景将在第一个模块后结束。
>
>如果第一个模块返回一个捆绑包，则该捆绑包将传递场景的其余部分。 在此示例中，方案的其余部分包含第二个和最后一个模块，这两个模块会将请求转换为项目。
>
>？![](assets/example-execution-flow-wf-only-350x157.png)

### 示例： [!UICONTROL [!DNL Workfront Fusion]工作自动化和集成]

>[!INFO]
>
>**示例：**&#x200B;在从[!DNL Adobe Workfront]下载文档并将它们发送到[!DNL Dropbox]中的文件夹的情况中，数据将按如下方式流动。
>
>场景的第一步由第一个模块执行，即监视捆绑包（文档）。 在此示例中，模块监视[!DNL Workfront]中的包。 如果不返回捆绑包，则场景将在第一个模块之后结束。
>
>如果返回一个束，则该束将通过场景的其余部分。 在此示例中，方案的其余部分由第二个和最后一个模块组成，这两个模块会将包上载到[!DNL Dropbox]文件夹。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一个模块返回多个包，则在上传第二个包之前，会将第一个包上传到[!DNL Dropbox]。 然后，第二个包上传，第三个包上传，依此类推。

## 有关已处理包的信息

对于每个模块，捆绑包在进入下一个模块或到达其最终目标之前将经过4步的过程。 四步流程是初始化、操作、提交/回滚和最终化。 这称为事务处理，它有助于解释如何在模块中处理数据。

场景运行完成后，每个模块会显示一个图标，其中显示了执行的操作数。 您可以单击此图标以按上述格式显示有关已处理捆绑的详细信息。 您可以查看使用了哪些模块设置以及哪个模块返回了哪些包。

![](assets/info-processed-bundles-350x396.png)

模块接收输入信息，例如：

* 已转换的图像
* 选定的图像应上传到的文件夹
* [!DNL Facebook]图像的原始名称

处理后，模块返回以下输出信息：

* 由[!DNL Dropbox]分配的图像ID
* [!DNL Dropbox] [!DNL Workfront Fusion]中上传文件的完整路径

为各个包分别捕获上述信息，如映像中的下拉框[!UICONTROL 操作1]和[!UICONTROL 操作2]所标记。

有关事务处理的详细信息，请参阅[方案执行、周期和阶段（在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中）。

## 执行场景时出错

在场景运行期间可能会出错。 例如，如果删除在模块设置中设置为目标文件夹的[!DNL Dropbox]文件夹，则方案将终止，并出现错误消息。 有关如何处理错误的更多信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md)中处理Error。
