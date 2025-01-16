---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 关于在 [!DNL Adobe Workfront Fusion]中映射文件
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# 关于在[!DNL Adobe Workfront Fusion]中映射文件

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [在模块之间映射文件](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

某些模块具有处理文件的功能。 这些模块可以返回要发送以供进一步处理的输出文件，也可以要求将文件传递给它们以供处理。 这些模块需要相互映射，才能共同处理文件。

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
  </tr>  </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 映射文件

能够处理文件的模块需要以下两项信息：

* 文件名
* 文件内容（数据）

在映射文件时，可以在场景中选择要从中获取数据的模块。 然后，文件名和文件内容将自动映射。

>[!NOTE]
>
>如果您需要处理来自URL的文件，我们建议使用`HTTP > Get a File`模块从URL下载文件，然后将文件从`HTTP > Get a File`模块映射到场景中所需模块的字段。

>[!INFO]
>
>**示例：**&#x200B;此示例说明如何将文档从[!DNL Adobe Workfront]下载到[!DNL Google Drive]。 [!DNL Workfront]触发器[!UICONTROL 监视记录]返回有关每个文档的详细信息，包括其名称和ID。
>
>下一个模块[!UICONTROL 下载文档]将下载实际数据，以便将其上传到Google驱动器。
>
>若要将此信息映射到[!DNL Google Drive]以便可以上载，您需要指定将从中映射该信息的源文件。 如果选择源文件下的[!DNL Workfront] > [!UICONTROL 下载文档]选项，[!DNL Workfront Fusion]将映射文件名和文件内容，以便将[!DNL Workfront]中的文档上载到指定的Google文件夹。
>
>![](assets/wf-download-document-350x605.png)
>
>但是，如果要重命名文件，但保持数据不变，则可以使用[!UICONTROL 映射]选项分别映射文件名和文件内容。 您需要输入完整的文件名，包括扩展名。 支持文本格式和二进制格式，如照片、视频和PDF。
>
>![](assets/use-the-map-option-350x358.png)
