---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的场景执行流程
description: 本文介绍了方案的执行方式以及数据如何通过它流动。 它还说明您可以在何处查找有关已处理数据的信息以及如何读取该信息。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# 中的方案执行流程 [!DNL Adobe Workfront Fusion]

本文介绍了方案的执行方式以及数据如何通过它流动。 它还说明您可以在何处查找有关已处理数据的信息以及如何读取该信息。

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

## 方案执行流程

正确设置并激活方案后，将根据其定义的计划执行方案。

当方案开始时，第一个模块将响应一个已设置为要监视的事件。 如果返回任何包（数据），则它们会传递到下一个模块，并且情景会继续，逐个通过每个连续的模块传递包。

如果包在所有模块中都正确处理，则情景将在情景详细信息区域中标记为成功，如 [中的方案详细信息 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 有关设置方案的更多信息，请参阅 [中的基本方案设置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 有关激活方案的更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 有关计划方案的更多信息，请参阅 [在中计划方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 有关模块的更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

### 示例： [!UICONTROL [!DNL Workfront Fusion] 工作自动化]

>[!INFO]
>
>**示例：** 在监控 [!DNL Workfront] 然后转化为 [!DNL Workfront] 项目，数据会以如下方式流动。
>
>方案的第一步由第一个模块执行，即监视请求。 传入的每个请求都被视为一个包。 如果模块在未找到任何包的情况下运行，则方案将在第一个模块之后结束。
>
>如果第一个模块返回包，则包将通过方案的其余部分。 在此示例中，方案的其余部分由第二个和最后一个模块组成，这两个模块会将请求转换为项目。
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 示例： [!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）]

>[!INFO]
>
>**示例：** 在从下载文档的场景中 [!DNL Adobe Workfront] 并将它们发送到 [!DNL Dropbox]，则数据会按如下方式流动。
>
>方案的第一步由第一个模块执行，即监视包（文档）。 在此示例中，模块监视中的包 [!DNL Workfront]. 如果它不返回包，则场景将在第一个模块之后结束。
>
>如果返回包，则包将通过方案的其余部分。 在此示例中，方案的其余部分由第二个和最后一个模块组成，这两个模块将包上传到 [!DNL Dropbox] 文件夹。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一个模块返回多个包，则第一个包将上传到 [!DNL Dropbox] ，然后再上传第二个包。 然后第二个包上载，然后是第三个包，依此类推。

## 有关已处理包的信息

对于每个模块，包将经过4步流程后再转到下一个模块或到达其最终目标。 四步流程是初始化、操作、提交/回滚和终止化。 这称为交易处理，有助于解释如何在模块中处理数据。

方案运行完成后，每个模块都会显示一个图标，其中显示了已执行的操作数。 您可以单击此图标以按上述格式显示已处理包的详细信息。 您可以查看使用了哪些模块设置以及哪些模块返回了哪些包。

![](assets/info-processed-bundles-350x396.png)

模块接收诸如：

* 已转换的图像
* 将图像上传到的选定文件夹
* 的原始名称 [!DNL Facebook] 图像

处理后，模块返回了以下输出信息：

* 图像ID分配者 [!DNL Dropbox]
* 入口的完整路径 [!DNL Dropbox] [!DNL Workfront Fusion] 已上传文件

将分别为每个包捕获上述信息，如下拉框所标记的 [!UICONTROL 操作1] 和 [!UICONTROL 操作2] 中。

有关交易处理的详细信息，请参阅 [方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 执行方案时出错

在方案运行期间可能会出错。 例如，如果删除 [!DNL Dropbox] 文件夹（您已在“模块”设置中设置为“目标文件夹”），此方案将终止，并显示一则错误消息。 有关如何处理错误的详细信息，请参阅 [处理中的错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
