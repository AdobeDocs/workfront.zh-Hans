---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion常见问题解答
description: 本文讨论与以下内容相关的常见问题： [!DNL Adobe Workfront Fusion]，包括有关Fusion工作流中常用对象的信息
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Adobe Workfront Fusion常见问题解答

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
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 什么是场景？

### 答案

场景定义了要执行的步骤序列 [!DNL Adobe Workfront Fusion]. 对于每个方案，您都可以指定数据源、如何处理数据、要使用哪些数据以及要忽略哪些数据。 [!DNL Workfront Fusion] 可让您根据需要创建尽可能复杂的场景；甚至最复杂的场景也可以。

有关更多信息，请参阅 [在中创建实践集成方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## 能否在场景中使用多个模块？ 还是只是个触发器和动作？

### 答案

您可以在场景中使用任意数量的模块。 您可以创建独立的路由并指定哪些数据应通过它们。 您还可以使用单个操作返回的结果，然后将它们传递给下一个操作。

## 可以 [!DNL Workfront Fusion] 处理文件？

### 答案

是. 使用 [!DNL Workfront Fusion]，可以接收、保存、转换、转换和加密文件，等等。 此外， [!DNL Workfront Fusion] 提供了广泛的内置功能，旨在使用户能够有效、创造性地使用文件中包含的数据。

有关更多信息，请参阅 [关于映射文件 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## 如果我让你 [!DNL Workfront Fusion] 是否处理包含多个附件的电子邮件？

### 答案

如果您使用 [!UICONTROL 电子邮件] 模块 [!UICONTROL 检索附件]，每个附件均通过场景中的其余模块单独发送。 类似的模块也可用于同时接收多个文件的其他应用程序。

有关更多信息，请参阅 [[!UICONTROL 电子邮件] 模块](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## 某些触发器允许场景立即运行。 “即时”是什么意思？

### 答案

根据您指定的计划，定期运行常见方案（例如，每小时、每5分钟、每月一次，等等）。 有一些特殊的触发器，称为即时触发器(webhook)，可以在它们从给定服务收到数据后立即启动场景。 即时触发器可能非常有用。 我们建议尽可能使用这两项功能。 它们有助于减少操作次数。 接收的数据会立即处理，而无需等待下一次计划运行。 例如， [!DNL Google Sheets] 模块 [!UICONTROL 观看更改] 在更新单元格后立即启动方案。

## 什么是聚合？

### 答案

An [!UICONTROL 汇总] 将数据合并到一个集合中。 例如，将文件压缩到zip存档中并作为电子邮件附件发送。

有关更多信息，请参阅 [[!UICONTROL 汇总] 中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## 什么是操作？

### 答案

操作是由模块执行的任何任务。 例如，每次触发器运行以及每次操作执行任务时都会执行操作。

## 什么是数据传输？

### 答案

数据传输是指通过您的方案传输的数据量。 例如，假设您有一个方案，即从FTP检索100KB的图像，将其大小减少到50KB，并将两个图像都保存到 [!DNL Dropbox]. 此方案中使用的数据量为250KB。

## 什么是连接？

### 答案

连接是指 [!DNL Workfront Fusion] 帐户以及要使用的第三方服务。 在编辑场景时，可以轻松创建连接。 要添加连接，请单击 **[!UICONTROL 添加]** 按钮，并按照分步说明操作。

有关更多信息，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
