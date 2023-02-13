---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 关于在中映射文件 [!DNL Adobe Workfront Fusion]
description: 某些模块能够处理文件。 这些模块可以返回要发送以供进一步处理的输出文件，或者需要将文件传递到它们进行处理。 在这些模块能够协同工作来处理文件之前，它们必须相互映射。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 关于在中映射文件 [!DNL Adobe Workfront Fusion]

某些模块能够处理文件。 这些模块可以返回要发送以供进一步处理的输出文件，或者需要将文件传递到它们进行处理。 在这些模块能够协同工作来处理文件之前，它们必须相互映射。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr>  </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 映射文件

能够处理文件的模块需要两个信息：

* 文件名
* 文件内容（数据）

映射文件时，在方案中选择要从中获取数据的模块。 然后，文件名和文件内容会按原样自动映射。

>[!NOTE]
>
>如果您需要通过URL处理文件，我们建议您使用 `HTTP > Get a File` 模块从URL下载文件，然后从 `HTTP > Get a File` 模块添加到场景中所需模块的字段。

>[!INFO]
>
>**示例：** 此示例说明如何从下载文档 [!DNL Adobe Workfront] to [!DNL Google Drive]. 的 [!DNL Workfront] 触发器 [!UICONTROL 观看记录] 返回有关每个文档的详细信息，包括其名称和ID。
>
>下一个模块， [!UICONTROL 下载文档]，则会下载实际数据，以便将其上传到Google Drive。
>
>将此信息映射到 [!DNL Google Drive] 为了上传该信息，您需要指定要从中映射信息的源文件。 如果您选择 [!DNL Workfront] > [!UICONTROL 下载文档] 选项， [!DNL Workfront Fusion] 映射文件名和文件内容，以便从 [!DNL Workfront] 已上传到指定的Google文件夹。
>
>![](assets/wf-download-document-350x605.png)
>
>但是，如果要重命名文件，但保留原样的数据，则可以使用 [!UICONTROL 地图] 选项，分别映射文件名和文件内容。 您应输入完整的文件名，包括扩展名。 支持文本格式和二进制格式，如照片、视频和PDF。
>
>![](assets/use-the-map-option-350x358.png)
