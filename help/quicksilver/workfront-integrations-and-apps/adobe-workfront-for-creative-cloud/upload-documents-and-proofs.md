---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 将文档和验证从 [!DNL Adobe Workfront plugin] 上载到 [!DNL Creative Cloud]
description: 将文档和验证从 [!DNL Adobe Workfront plugin] 上载到 [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 将文档和验证从[!DNL Adobe Workfront plugin]上载到[!DNL Creative Cloud]

您可以将项目作为文档上传，以供快速审阅和批准，或仅将其存储在[!DNL Adobe Workfront]中。

>[!NOTE]
>
>Premiere Pro和After Effects当前不支持上传文档和验证。


## 文档限制

本节概述了[!DNL Workfront for Adobe Creative Cloud plugins]中的已知文档限制。

### 新文档版本仅接受上传一个文件

由于[!DNL Workfront]文档不能包含多个文件，因此必须禁用某些设置才能将新文档版本上传到Workfront。

>[!NOTE]
>
>如果必须生成多个文件，则可以改为创建验证。 新验证将不会与原始文档相关联。



要在[!DNL InDesign]中将切换更改回单个文件，请执行以下操作：

1. 打开&#x200B;**设置导出文件设置**&#x200B;对话框。

   ![](assets/file-export-settings.png)

1. 找到要导出的资产类型，然后按如下所述调整设置：

   <table>
    <tr>
    <td><strong>PDF和PDF打印</strong>
    </td>
    <td>取消选择<strong>创建单独的PDF文件</strong>。
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>选择<strong>范围</strong>并键入一个页码。 
    <p>
    <strong>注意</strong>：如果要上载完整文档，必须创建一个验证。 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB和EPUB已修复</strong>
    </td>
    <td>无需调整。
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>无需调整。
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>选择<strong>范围</strong>并键入一个页码。 
    <p>
    <strong>注意</strong>：如果要上载完整文档，必须创建一个验证。 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>选择<strong>范围</strong>并键入一个页码。 
    <p>
    <strong>注意</strong>：如果要上载完整文档，必须创建一个验证。 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>无需调整。 
    </td>
    </tr>
    </table>
