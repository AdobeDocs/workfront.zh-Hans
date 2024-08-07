---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion]中的方案执行、周期和阶段'
description: 本文介绍了在 [!DNL Adobe Workfront Fusion] 方案运行时发生的事件，如初始化、操作、提交和回滚。
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion]中的方案执行、周期和阶段

[!DNL Adobe Workfront Fusion]是一个事务型系统，类似于关系数据库。 每个场景执行从初始化阶段开始，至少包含一个由操作和提交/回滚阶段组成的周期，并结束于最终确定阶段：

>[!INFO]
>
>**示例**
>
>初始化
>
>循环#1
>
>操作（读取或写入）
>
>提交或回滚
>
>循环#2
>
>操作（读取或写入）
>
>提交或回滚
>
>...
>
>循环#N
>
>操作（读取或写入）
>
>提交或回滚
>
>最终完成

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

## 初始化

在初始化阶段，将创建所有必需的连接（与数据库、电子邮件服务等的连接）。 此外，还检查每个模块是否能够执行其预期操作。

## 周期

每个周期代表由一系列操作组成的一个不可分割的工作单元。 可以在[!UICONTROL 方案设置]面板中设置最大循环数。 默认数字为1。

有关详细信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)中的[方案设置面板。

## 操作

在操作阶段期间，执行读取和/或写入操作：

* 读取操作包括从服务获取数据，然后由其它模块根据预定义场景处理该数据。 例如，[!UICONTROL Dropbox] >[!UICONTROL 监视文件]模块返回自上次方案执行以来创建的新包（文件）。
* 写入操作包括向给定服务发送数据以供进一步处理。 例如，[!DNL Dropbox] >[!UICONTROL 上载文件]模块会将文件上载到[!DNL Dropbox]文件夹。

## 提交

如果所有模块的操作阶段均成功，则提交阶段开始，在此期间将提交模块执行的所有操作。 这意味着[!DNL Workfront Fusion]向操作阶段涉及的所有服务发送有关其成功的信息。

## 回滚

如果在任何模块的操作或提交阶段发生错误，该阶段将中止，并且回滚阶段将启动，从而使给定周期内的所有操作都无效。 某些模块不支持回滚，并且无法恢复这些模块执行的操作。 有关详细信息，请参阅[ACID模块](#acid-modules)部分。

## 最终完成

在最终确定阶段，将关闭打开的连接（例如FTP连接、数据库连接等）并完成场景。

## ACID模块

所有支持回滚（也称为事务性）的[!DNL Workfront Fusion]模块均标有ACID标记。

![](assets/acid-modules-350x189.png)

当其他模块发生错误时，未使用此标记标记的模块无法恢复为初始状态。 非ACID模块的典型示例是[!UICONTROL 电子邮件] >[!UICONTROL 发送电子邮件]操作。 发送电子邮件后，无法撤消发送。
