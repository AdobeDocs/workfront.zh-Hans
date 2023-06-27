---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 关于映射文件 [!DNL Adobe Workfront Fusion]
description: 某些模块具有处理文件的功能。 这些模块可以返回要发送以供进一步处理的输出文件，也可以要求将文件传递给它们以供处理。 在这些模块可以一起工作以处理文件之前，它们必须相互映射。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# 关于映射文件 [!DNL Adobe Workfront Fusion]

某些模块具有处理文件的功能。 这些模块可以返回要发送以供进一步处理的输出文件，也可以要求将文件传递给它们以供处理。 在这些模块可以一起工作以处理文件之前，它们必须相互映射。

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
  </tr>  </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 映射文件

能够处理文件的模块需要以下两项信息：

* 文件名
* 文件内容（数据）

映射文件时，可在场景中选择要从中获取数据的模块。 然后，将自动映射文件名和文件内容。

>[!NOTE]
>
>如果您需要通过URL处理文件，我们建议使用 `HTTP > Get a File` 模块，用于从URL下载文件，然后从映射文件 `HTTP > Get a File` 模块到场景中所需模块的字段。

>[!INFO]
>
>**示例：** 此示例说明如何从下载文档 [!DNL Adobe Workfront] 到 [!DNL Google Drive]. 此 [!DNL Workfront] 触发器 [!UICONTROL 观看记录] 返回有关每个文档的详细信息，包括其名称和ID。
>
>下一模块， [!UICONTROL 下载文档]，可下载实际数据，以便将其上传到Google驱动器。
>
>将此信息映射到 [!DNL Google Drive] 为了能够上载，您需要指定信息将映射到的源文件。 如果您选择 [!DNL Workfront] > [!UICONTROL 下载文档] 源文件下的选项， [!DNL Workfront Fusion] 映射文件名和文件内容，以便文档来自 [!DNL Workfront] 上传到指定的Google文件夹。
>
>![](assets/wf-download-document-350x605.png)
>
>但是，如果要重命名文件，但保留数据不变，则可以使用 [!UICONTROL 映射] 选项分别映射文件名和文件内容。 您需要输入完整的文件名，包括扩展名。 支持文本格式和二进制格式，如照片、视频和PDF。
>
>![](assets/use-the-map-option-350x358.png)
