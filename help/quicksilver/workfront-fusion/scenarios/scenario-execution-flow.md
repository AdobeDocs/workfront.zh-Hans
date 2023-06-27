---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion中的场景执行流程
description: 本文介绍了场景的执行方式以及数据流通过场景的情况。 它还介绍了可在何处找到有关已处理数据的信息以及如何读取该信息。
author: Becky
feature: Workfront Fusion
exl-id: 95c6e969-66b4-4b57-9e62-aae0cfb9bf98
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# 中的方案执行流程 [!DNL Adobe Workfront Fusion]

本文介绍了场景的执行方式以及数据流通过场景的情况。 它还介绍了可在何处找到有关已处理数据的信息以及如何读取该信息。

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

## 场景执行流程

正确设置并激活场景后，该场景将根据其定义的计划执行。

在场景开始时，第一个模块会响应已设置为监视的事件。 如果它返回任何包（数据），则它们会传递到下一个模块，并且场景会继续，从而逐个通过每个后续模块传递包。

如果捆绑包在所有模块中正确处理，则会在方案详细信息区域中将该方案标记为成功，如中所述 [中的方案详细信息 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

* 有关设置方案的详细信息，请参阅 [中的基本方案设置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/basic-scenario-settings.md).
* 有关激活方案的详细信息，请参阅 [在中激活或取消激活方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).
* 有关计划方案的详细信息，请参阅 [在中计划方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
* 有关模块的更多信息，请参阅 [模块类型](../../workfront-fusion/modules/module-types.md).

### 示例： [!UICONTROL [!DNL Workfront Fusion] （工作自动化）]

>[!INFO]
>
>**示例：** 在监视传入请求的场景中 [!DNL Workfront] 然后将它们转换为 [!DNL Workfront] 项目，数据将按如下方式流动。
>
>场景的第一步（由第一个模块执行）是观察请求。 传入的每个请求都被视为一个捆绑包。 如果模块运行时未找到任何捆绑包，则场景将在第一个模块后结束。
>
>如果第一个模块返回一个捆绑包，则该捆绑包将传递场景的其余部分。 在此示例中，方案的其余部分由第二个和最后一个模块组成，这两个模块会将请求转换为项目。
>
>?![](assets/example-execution-flow-wf-only-350x157.png)

### 示例： [!UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成]

>[!INFO]
>
>**示例：** 在从以下来源下载文档的场景中 [!DNL Adobe Workfront] 并将它们发送到中的文件夹 [!DNL Dropbox]，数据将按如下方式流动。
>
>场景的第一步（由第一个模块执行）是观察包（文档）。 在此示例中，模块会监视中的捆绑包 [!DNL Workfront]. 如果不返回捆绑包，则场景将在第一个模块之后结束。
>
>如果返回了某个包，则该包将传递场景的其余部分。 在此示例中，场景的其余部分由第二个和最后一个模块组成，这两个模块会将捆绑包上传到 [!DNL Dropbox] 文件夹。
>
>![](assets/example-wf-dropbox-scen-execution-flow-350x202.png)
>
>如果第一个模块返回多个包，则第一个包将上传到 [!DNL Dropbox] 上传第二个包之前。 然后上传第二个包，再上传第三个包，依此类推。

## 有关已处理包的信息

对于每个模块，捆绑包在进入下一个模块或到达其最终目标之前将经过4步的过程。 四步流程是初始化、操作、提交/回滚和最终化。 这称为事务处理，它有助于解释如何在模块中处理数据。

场景运行完成后，每个模块会显示一个图标，其中显示了执行的操作数。 您可以单击此图标以按上述格式显示有关已处理包的详细信息。 您可以查看使用了哪些模块设置以及哪个模块返回了哪些捆绑包。

![](assets/info-processed-bundles-350x396.png)

模块接收输入信息，例如：

* 已转换的图像
* 选定的图像应上传到的文件夹
* 的原始名称 [!DNL Facebook] 图像

处理完毕后，模块返回以下输出信息：

* 图像ID分配者 [!DNL Dropbox]
* 中的完整路径 [!DNL Dropbox] [!DNL Workfront Fusion] 已上传文件

将为每个捆绑包分别捕获上述信息，如下拉框中所标记 [!UICONTROL 操作1] 和 [!UICONTROL 操作2] 在图像中。

有关事务处理的详细信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## 执行场景时出错

在场景运行期间可能会发生错误。 例如，如果您删除 [!DNL Dropbox] 在模块设置中设置为目标文件夹的文件夹内，场景将终止，并显示一条错误消息。 有关如何处理错误的更多信息，请参阅 [处理以下对象时出错： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).
