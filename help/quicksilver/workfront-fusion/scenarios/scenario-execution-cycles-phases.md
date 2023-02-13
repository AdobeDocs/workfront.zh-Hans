---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]
description: 本文介绍在 [!DNL Adobe Workfront Fusion] 方案正在运行，例如初始化、操作、提交和回滚。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] 是事务型系统，与关系型数据库类似。 每个方案执行从初始化阶段开始，继续至少一个由操作和提交/回滚阶段组成的周期，并以终止化阶段结束：

>[!INFO]
>
>**示例**
>
>初始化
>
>周期#1
>
>操作（读或写）
>
>提交或回滚
>
>周期#2
>
>操作（读或写）
>
>提交或回滚
>
>...
>
>周期#N
>
>操作（读或写）
>
>提交或回滚
>
>定稿

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 初始化

在初始化阶段，将创建所有必需的连接（与数据库的连接、电子邮件服务等）。 此外，还会检查每个模块是否能够执行其预期操作。

## 周期

每个周期代表由一系列操作组成的不可分割的工作单元。 可以在 [!UICONTROL 方案设置] 的上界。 默认数字为1。

有关更多信息，请参阅 [中的“方案设置”面板 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 操作

在操作阶段期间执行读和/或写操作：

* 读取操作包括从服务获取数据，然后由其它模块根据预定方案处理该数据。 例如， [!UICONTROL Dropbox] >[!UICONTROL 监视文件] 模块返回自上次方案执行以来创建的新包（文件）。
* 写入操作包括向给定服务发送数据以供进一步处理。 例如， [!DNL Dropbox] >[!UICONTROL 上传文件] 模块将文件上传到 [!DNL Dropbox] 文件夹。

## 提交

如果所有模块的操作阶段都成功，则提交阶段开始，在该阶段中，模块执行的所有操作都被提交。 这意味着 [!DNL Workfront Fusion] 向操作阶段涉及的所有服务发送有关其成功的信息。

## 回滚

如果在任何模块的操作或提交阶段期间发生错误，则该阶段会中止并启动回滚阶段，从而使给定周期期间的所有操作都无效。 某些模块不支持回滚，并且这些模块执行的操作无法恢复。 有关详细信息，请参阅 [酸模](#acid-modules) 中。

## 定稿

在终止化阶段，打开的连接（例如，FTP连接、数据库连接等）将关闭，并且方案已完成。

## 酸模

全部 [!DNL Workfront Fusion] 支持回滚（也称为事务性）的模块使用ACID标记进行标记。

![](assets/acid-modules-350x189.png)

当其他模块中发生错误时，未使用此标记的模块无法还原到其初始状态。 非ACID模块的典型示例是 [!UICONTROL 电子邮件] >[!UICONTROL 发送电子邮件] 操作。 发送电子邮件后，将无法撤消发送。
