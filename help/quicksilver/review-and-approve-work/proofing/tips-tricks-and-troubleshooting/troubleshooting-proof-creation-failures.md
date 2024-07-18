---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: 验证创建失败疑难解答
description: 验证创建过程包括导入和验证生成。 有时，在创建验证时，文件可能无法导入，或者在导入文件后无法生成验证。
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# 验证创建失败疑难解答

验证创建过程包括导入和验证生成。 有时，在创建验证时，文件可能无法导入，或者在导入文件后无法生成验证。

>[!NOTE]
>
> 如果您尝试验证的文档与本节中列出的任何条件都不匹配，请联系Adobe Workfront支持部门以进一步调查。

## 导入失败的原因

* 您已创建包含50多个文件的组合验证。

## 验证生成失败的原因

* 不支持该文件类型。\
  有关支持的文件类型的列表，请参阅[支持的校对文件类型和大小限制概述](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md)。

* 文件结构是文件类型的非标准结构。
* 文件受密码保护，或者已禁用内容复制。

  与其他类型的文件不同，如果在PDF上将PDF复制的安全设置设置为“允许”，则内容文件可以生成为验证。

* 页面长度或页数超过限制。

  栅格化后允许的最大页面长度为195英寸；单个验证允许的最大页面计数为1,000页。

* 文件已损坏或损坏。
* 新验证版本的工作流截止日期已过去。

  当您使用快速验证方法创建新验证版本，并且在上传文档时选择了&#x200B;**自动生成验证**&#x200B;时，会发生这种情况。 新验证版本尝试从之前生成的验证中获取工作流截止日期。 如果这些截止日期已过，则验证生成失败。 要解决此问题，您可以在将来在以前的版本上设置工作流截止日期，或生成新的验证版本。 如果您生成新版本，请使用&#x200B;**更多>新版本>校对**，然后选择将来的&#x200B;**工作流截止日期**。

* 验证PDF文件时，验证生成失败的原因包括：

   * 字体和图像从外部源（如本地文件系统）链接

     必须将字体和图像嵌入到PDF文件中，才能在另一台计算机上或Workfront Proof中显示。

   * PDF文件包含空图层或透明或重叠字段。

     如果无法确定导致此问题的图层或对象，请将设计/文档导出为优化PDF（这会删除所有不需要的元素）。

