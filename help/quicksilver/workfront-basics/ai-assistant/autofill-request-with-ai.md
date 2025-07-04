---
title: 使用AI自动填写请求
content-type: reference
description: 您可以使用AI自动填写请求字段。
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: a3e93311277bc5b68063e0ec1cbdcce3a40eb3dd
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# 使用AI自动填写请求

>[!NOTE]
>
>此功能目前是封闭测试版的一部分。 要启用此功能，请联系sargism@adobe.com。
>
>要获得封闭测试版的资格，您的组织必须满足使用Workfront AI Assistant的要求。 有关详细信息，请参阅[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。

AI可帮助您自动填写请求字段。 它可以根据以前的请求建议字段值，或从文本（如电子邮件和已上传的文档）中解析这些值。

您可以在提交请求之前批准或拒绝这些建议。

自动填写不会覆盖您已填写的任何字段。

## 在填写表单时获取建议

自动填写可以在您填写表单时建议字段值。 在请求字段中输入值时，Workfront会将这些值与以前的请求进行比较。 如果输入的值与以前请求中类似上下文中的其他字段值紧密相关，则Workfront会推荐这些值。

例如，如果诊所始终使用相同的计费代码，那么在输入诊所名称时，Workfront会建议在适当的字段中输入该计费代码。

要根据以前的请求使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 开始填写字段。

   当您填写字段时，其他字段可能会显示建议。

1. 对于每个字段建议，请选择该字段下的&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

## 从文本提示获取建议

自动填写可根据文本（如电子邮件）建议字段值。 将粘贴到文本块中，Workfront会处理文本以根据文本建议字段值。

例如，如果电子邮件包含“此日期在6月1日到期”，并且请求表单中存在到期日期的字段，则Workfront将建议在6月1日使用该字段值。

此类建议还会检查以前对类似上下文的请求。 例如，如果提示提及请求是针对特定客户的，Workfront可以根据之前的请求自动查找并输入该客户的账单地址。

您可以粘贴要应用于整个表单或表单单个部分的文本。

要根据粘贴的文本提示使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 要将文本提示应用于整个表单，请单击表单名称下的AI图标![AI图标](assets/request-prompt-icon.png)。

   或

   要为单个分区应用文本提示，请单击分区名称旁边的AI图标![AI图标](assets/request-prompt-icon.png)。

1. 将文本粘贴到提示框中。
1. 单击&#x200B;**填写表单**。

   Workfront会生成表单建议。
1. 对于每个字段建议，请选择该字段下的&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

## 根据您上传的文档获取建议

自动填写可以根据您上传的文档来建议字段值。

此类建议还会检查以前对类似上下文的请求。 例如，如果提示提及请求是针对特定客户的，Workfront可以根据之前的请求自动查找并输入该客户的账单地址。

### 文档上传护栏

#### 支持的文件类型

支持以下文件类型：

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### 支持的文件大小

每个文件的大小最多可达100 MB

#### 文件数

您最多可以上传50个文件（页面、幻灯片或工作表）。

>[!IMPORTANT]
>
>文档将转换为一系列图像，每个图像都被视为单独的文件。
>
>例如，您可以上传一个包含50张幻灯片的PowerPoint，或上传每个包含10页的5个Word文档。

#### 其他最佳实践

在上传请求自动填写的文档时，请考虑以下事项：

* 自动填写当前已针对拉丁字母进行了优化。
* 我们建议使用8点或更大的文本大小。
* 自动填充可能难以处理文档中的图像，例如旋转或扭曲的图像、图形、对图像中的对象进行计数或使用空间原因。
* 与往常一样，我们建议在提交请求之前检查结果的准确性。

### 上传文档以自动填写请求

您可以上载要应用于整个表单或表单单个部分的文档。

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 要将文档应用于整个表单，请单击表单名称下的AI图标![AI图标](assets/request-prompt-icon.png)。

   或

   若要将文档应用于单个分区，请单击分区名称旁边的AI图标![AI图标](assets/request-prompt-icon.png)。

1. 单击&#x200B;**上载文件**，然后从文件管理器中选择该文件。

   或

   将文档从文件管理器拖到&#x200B;**上载文件以自动填写请求表单**&#x200B;框。
1. 单击&#x200B;**填写表单**，共&#x200B;**填写部分**。

   Workfront会生成表单建议。
1. 对于每个字段建议，请选择该字段下的&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

