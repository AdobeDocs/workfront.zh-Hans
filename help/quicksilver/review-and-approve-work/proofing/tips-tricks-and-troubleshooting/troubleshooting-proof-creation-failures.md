---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: 校样创建失败疑难解答
description: 校样创建过程包括导入和校样生成。 有时，在创建校样时，文件可能无法导入，或者在导入文件后，校样可能无法生成。
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---


# 校样创建失败疑难解答

校样创建过程包括导入和校样生成。 有时，在创建校样时，文件可能无法导入，或者在导入文件后，校样可能无法生成。

>[!NOTE]
>
> 如果您尝试验证的文档与本节中列出的任何标准都不匹配，请联系Adobe Workfront支持部门以进一步调查。

## 导入失败的原因

* 您已创建包含50个以上文件的组合校样。

## 验证生成失败的原因

* 不支持文件类型。\
   有关支持的文件类型列表，请参阅 [支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* 文件结构是文件类型的非标准结构。
* 文件受密码保护或内容复制被禁用。

   与其他类型的文件不同，如果在PDF上将内容复制的安全设置设置为允许，则PDF文件可以生成为校样。

* 页面长度或页面计数超过限制。

   最大允许页面长度在光栅化后为195英寸；对于单次校样，允许的最大页面计数为1,000页。

* 文件已损坏。
* 新校样版本的工作流截止日期已过。

   当您使用快速校样方法和创建新校样版本时，会发生这种情况 **上传文档时自动生成校样** 中。 新校样版本会尝试从之前生成的校样中获取工作流的截止时间。 如果这些截止时间已过，则生成校样会失败。 要解决此问题，您可以在将来为以前的版本设置工作流截止日期，或生成新的校样版本。 如果生成新版本，请使用 **更多>新版本>校样** 选择 **工作流的最后期限**.

* 对PDF文件进行校样时，生成校样失败的原因包括：

   * 字体和图像从外部源（例如，从本地文件系统）链接

      字体和图像必须嵌入到PDF文件中，才能在另一台计算机上或Workfront校样中显示。

   * PDF文件包含空图层或透明或重叠字段。

      如果无法确定由哪个层或对象引起此问题，请将设计/文档导出为优化PDF（这会删除所有不需要的元素）。

