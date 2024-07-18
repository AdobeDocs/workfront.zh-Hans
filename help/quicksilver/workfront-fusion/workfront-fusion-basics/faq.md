---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Adobe Workfront Fusion常见问题
description: 本文讨论与 [!DNL Adobe Workfront Fusion]相关的常见问题，包括有关Fusion工作流中常用对象的信息
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 1%

---

# Adobe Workfront Fusion常见问题

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
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 什么是场景？

### 答案

方案定义了[!DNL Adobe Workfront Fusion]要执行的步骤序列。 对于每个方案，您都可以指定数据源、如何处理数据、要使用哪些数据以及要忽略哪些数据。 [!DNL Workfront Fusion]允许您根据需要创建尽可能复杂的场景；即使是最复杂的场景也是可能的。

有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md)中创建实践集成方案。

## 能否在场景中使用多个模块？ 还是只是个触发器和动作？

### 答案

您可以在场景中使用任意数量的模块。 您可以创建独立的路由并指定哪些数据应流经它们。 您还可以使用单个操作返回的结果，然后将它们传递给下一个操作。

## [!DNL Workfront Fusion]可以使用文件吗？

### 答案

可以。使用[!DNL Workfront Fusion]，可以接收、保存、转换、转换和加密文件，等等。 此外，[!DNL Workfront Fusion]提供了多种内置功能，旨在使用户能够有效、创造性地处理文件中包含的数据。

有关详细信息，请参阅[关于在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md)中映射文件。

## 如果我允许[!DNL Workfront Fusion]处理包含多个附件的电子邮件，会发生什么情况？

### 答案

如果您使用[!UICONTROL 电子邮件]模块[!UICONTROL 检索附件]，则每个附件都将通过场景中的其余模块单独发送。 类似的模块也可用于同时接收多个文件的其他应用程序。

有关详细信息，请参阅[[!UICONTROL 电子邮件]模块](../../workfront-fusion/apps-and-their-modules/email-modules.md)。

## 某些触发器允许场景立即运行。 “即时”是什么意思？

### 答案

常见场景会根据您指定的计划定期运行（例如，每小时、每5分钟、每月运行一次，等等）。 有一些特殊的触发器，称为即时触发器(webhook)，可以在它们从给定服务收到数据后立即启动场景。 即时触发器可能非常有用。 我们建议尽可能使用它们。 它们有助于减少操作次数。 接收的数据会立即处理，而无需等待下一次计划运行。 例如，[!DNL Google Sheets]模块[!UICONTROL 监视更改]在单元格更新后立即启动方案。

## 什么是聚合？

### 答案

[!UICONTROL 聚合器]将数据合并到一个集合中。 例如，将文件压缩为zip存档并作为电子邮件附件发送。

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md)中的[[!UICONTROL 聚合器]模块。

## 什么是操作？

### 答案

操作是由模块执行的任何任务。 例如，每次触发器运行以及每次操作执行任务时都会执行操作。

## 什么是数据传输？

### 答案

数据传输是指通过您的方案传输的数据量。 例如，假设您的方案从FTP检索100KB的图像，将其大小减少到50KB，并将两个图像保存到[!DNL Dropbox]。 此方案中使用的数据量为250KB。

## 什么是连接？

### 答案

连接是指您的[!DNL Workfront Fusion]帐户与要使用的第三方服务之间的链接。 在编辑场景时，可以轻松创建连接。 要添加连接，请单击模块设置中的&#x200B;**[!UICONTROL 添加]**&#x200B;按钮，然后按照分步说明操作。

有关详细信息，请参阅[连接概述](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)。
