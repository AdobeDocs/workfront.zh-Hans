---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 存档模块
description: 在 [!DNL Adobe Workfront Fusion] 方案中，您可以将存档（如压缩文件）连接到多个第三方应用程序和服务。 例如，您可以配置一个方案，该方案
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL 存档] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以在场景中使用存档文件（如压缩文件），以便在自动或集成中使用它。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). 有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL 存档] 模块及其字段

配置 [!UICONTROL 存档] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!UICONTROL 存档] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL 提取存档]](#extract-an-archive)
* [[!UICONTROL 创建存档]](#create-an-archive)
* [[!UICONTROL 膨胀]](#inflate)
* [[!UICONTROL 平减]](#deflate)

## [!UICONTROL 提取存档]

此操作模块会从存档中提取您标识的文件。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td> <p> 选择要提取的文件。 此文件可以从以前的模块(如 [!DNL Workfront] &gt;[!UICONTROL下载文档]模块)。</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 从定义的 [!DNL Dropbox] 文件夹（例如，存档），使用 [!UICONTROL 存档] 并将提取的文件作为附件发送到所需的电子邮件地址 [!UICONTROL 电子邮件] 或 [!DNL Gmail] 模块。
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL 创建存档]

此聚合模块将所需文件添加到 [!UICONTROL ZIP] 或 [!UICONTROL TAR] 存档。

配置此模块时，将显示以下字段。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL源模块]</td> 
   <td> <p> 选择要从中检索文件的模块。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>选择要将文件添加到[!UICONTROL ZIP]存档还是[!UICONTROL TAR]存档。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL注释]</td> 
   <td>输入要添加到存档的注释。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>定义要将聚合输出分组为的表达式。 此表达式可以包含一个或多个映射的项目。 然后，将使用此表达式的值将聚合数据分为多个组。 每个组以一个单独的包的形式输出，包含键（计算的表达式）和值（聚合的文本）。 您可以在后续模块中将键用作过滤器。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL空聚合后停止处理]</td> 
   <td>选择此选项可在没有结果时停止方案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL存档名称]</td> 
   <td> <p> 输入已创建存档的名称。 请勿添加扩展。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 使用 [!DNL Gmail] >[!UICONTROL 观看电子邮件] 模块。 如果收到电子邮件，其附件将被迭代到各个包中，然后存档到 [!DNL ZIP] 文件并保存到定义的Dropbox文件夹。
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 膨胀]

该变压器模块使用膨胀算法来解压缩二进制数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据] </td> 
   <td> <p>输入或映射要使用infrate函数解压缩的数据。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL 平减]

此变压器模块使用放气算法压缩二进制数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL数据] </td> 
   <td> <p>输入或映射要使用deflate函数压缩的数据。</p> </td> 
  </tr> 
 </tbody> 
</table>
