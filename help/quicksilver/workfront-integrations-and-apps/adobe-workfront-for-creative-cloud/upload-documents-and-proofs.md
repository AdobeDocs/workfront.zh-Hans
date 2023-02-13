---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 从上传文档和校样 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]
description: 从上传文档和校样 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# 从上传文档和校样 [!DNL Adobe Workfront plugin] 到 [!DNL Creative Cloud]

您可以将项目作为文档上传，以便进行快速审核和批准，或者只是存储在中 [!DNL Adobe Workfront].

>[!NOTE]
>
>当前，Premiere Pro和After Effects不支持上传文档和校样。


## 文档限制

本节概述了 [!DNL Workfront for Adobe Creative Cloud plugins].

### 新文档版本仅接受一个文件进行上传

因为 [!DNL Workfront] 文档不能包含多个文件，必须禁用某些设置才能将新文档版本上传到Workfront。

>[!NOTE]
>
>如果必须生成多个文件，则可以改为创建校样。 新校样将不会与原始文档关联。



将交换机更改回单个文件(位于 [!DNL InDesign]:

1. 打开 **设置导出文件设置** 对话框。

   ![](assets/file-export-settings.png)

1. 查找要导出的资产类型，并按如下所述调整设置：

   <table>
    <tr>
    <td><strong>PDF和PDF打印</strong>
    </td>
    <td>取消选择 <strong>创建单独的PDF文件</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>选择 <strong>范围</strong> 并键入一个页码。 
    <p>
    <strong>注意</strong>:如果要上载完整文档，则必须创建校样。 
    </td>
    </tr>
    <tr>
    <td><strong>ePub和EPUB — 固定</strong>
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
    <td>选择 <strong>范围</strong> 并键入一个页码。 
    <p>
    <strong>注意</strong>:如果要上载完整文档，则必须创建校样。 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>选择 <strong>范围</strong> 并键入一个页码。 
    <p>
    <strong>注意</strong>:如果要上载完整文档，则必须创建校样。 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>无需调整。 
    </td>
    </tr>
    </table>
