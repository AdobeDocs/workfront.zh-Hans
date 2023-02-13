---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion常见问题解答
description: 本文介绍与 [!DNL Adobe Workfront Fusion]，包括有关融合工作流中常用对象的信息
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Adobe Workfront Fusion常见问题解答

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> <p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 什么情况？

### 回答

方案定义要执行的步骤序列 [!DNL Adobe Workfront Fusion]. 对于每个方案，您都可以指定数据源、如何处理数据、使用哪些数据以及忽略哪些数据。 [!DNL Workfront Fusion] 允许您根据需要创建复杂的场景；即使是最复杂的情景也是可能的。

有关更多信息，请参阅 [在中创建实践集成方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 我是否可以在情景中使用多个模块？ 还是只是一个触发器和动作？

### 回答

您可以在方案中使用所需数量的模块。 您可以创建独立路由并指定应通过这些路由的数据。 您还可以使用各个操作返回的结果，然后将其传递到下一个操作。

## 可以 [!DNL Workfront Fusion] 处理文件？

### 回答

是. 使用 [!DNL Workfront Fusion]、文件可以接收、保存、转换、转换、加密等。 此外， [!DNL Workfront Fusion] 提供了多种内置功能，旨在让用户能够高效、创造性地处理文件中包含的数据。

有关更多信息，请参阅 [关于在中映射文件 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 如果我让 [!DNL Workfront Fusion] 处理包含多个附件的电子邮件？

### 回答

如果您使用 [!UICONTROL 电子邮件] 模块 [!UICONTROL 检索附件]，则每个附件都会通过方案中的其余模块单独发送。 其他同时接收多个文件的应用程序中也提供了类似模块。

有关更多信息，请参阅 [[!UICONTROL 电子邮件] 模块](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 某些触发器允许场景立即运行。 “立即”是什么意思？

### 回答

常见方案会根据您指定的计划（例如，每小时、每5分钟、每月一次等）定期运行。 有一些特殊触发器，称为即时触发器(webhook)，可在从给定服务收到数据后立即启动您的方案。 即时触发器可能非常有用。 我们建议尽可能使用它们。 它们有助于减少操作数量。 接收的数据会立即进行处理，而不等待下次计划运行。 例如， [!DNL Google Sheets] 模块 [!UICONTROL 监视更改] 在更新单元格后立即启动方案。

## 什么是聚合器？

### 回答

安 [!UICONTROL 聚合器] 将数据合并到一个收藏集中。 例如，文件将压缩为zip存档并作为电子邮件附件发送。

有关更多信息，请参阅 [[!UICONTROL 聚合器] 模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 什么操作？

### 回答

操作是指模块执行的任何任务。 例如，每次触发器运行时，以及每次操作执行任务时，都会发生操作。

## 什么是数据传输？

### 回答

数据传输是指通过您的方案传输的数据量。 例如，假定您的情景是从FTP中检索100KB的图像，并将其大小减小到50KB，并将这两个图像保存到 [!DNL Dropbox]. 此方案中使用的数据量为150KB。

## 什么是联系？

### 回答

连接是 [!DNL Workfront Fusion] 帐户和要使用的第三方服务。 在编辑方案时可以轻松创建连接。 要添加连接，请单击 **[!UICONTROL 添加]** 按钮，并按照分步说明操作。

有关更多信息，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 到应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
