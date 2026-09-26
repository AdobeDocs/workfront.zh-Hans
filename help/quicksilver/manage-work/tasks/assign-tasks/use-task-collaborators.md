---
title: 使用工作代理
content-type: reference
description: 了解如何使用工作代理，即可以分配给Workfront任务的AI协作者。
author: Becky
feature: Work Management, Tasks
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 1%
---
# 使用工作代理

工作代理是可直接分配给Workfront任务的AI协作者，此外还有用于文档和资产审阅的现有AI审阅者。 与其他AI协作者一样，工作代理也是在“设置”区域中配置的，并像用户一样分配给任务。

工作代理连接到您在Copilot Studio、Claude或Writer中配置的代理。

有关在Workfront中创建工作代理的信息和说明，请参阅配置AI协作者一文中的[配置工作代理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>选择、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 您必须先在Copilot、Claude或Writer.ai中配置代理，然后才能将其用作工作代理。

## 工作代理概述

工作代理是一种将MCP代理分配给Workfront中的特定任务的方法。 您可以在Copilot Studio、Claude或Writer.ai等应用程序中配置代理，然后将该代理作为工作代理连接到Workfront。 然后，您可以像分配用户一样将其分配给任务。

一些示例工作流可能包括：

* 检测上传到任务的图像，根据提供给代理的条件生成变体，并将新图像上传到任务。
* 从任务描述生成副本，根据代理中配置的准则检查副本，并将副本发布到更新流。
* 读取事件的详细信息，识别缺少的详细信息，并在更新流中发布有关缺少的详细信息的问题。

>[!NOTE]
>
>* 有关代理职责和能力的特定详细信息是在创建代理的应用程序中配置的，而不是在Workfront中配置的。
>* 不需要将Workfront MCP服务器添加到用作工作代理的代理，也不需要连接工作代理才能工作。
>* 工作代理当前支持在Copilot Studio、Claude和Writer.ai中创建的代理。
>* 在Copilot Studio中配置代理时，必须将安全性设置为&#x200B;**无身份验证**。
>* 有关在Workfront中创建工作代理的信息和说明，请参阅配置AI协作者一文中的[配置工作代理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent)。

## 工作代理读取的信息

当工作代理开始处理任务时，它会自动读取以下任务信息作为上下文：

* 任务标题
* 任务描述
* 任务更新流中的注释
* 附加到任务的任何自定义表单中的信息

此信息始终读取，不能配置为Workfront设置。

>[!TIP]
>
>为获得最佳结果，我们建议：
>
>* 包括您希望座席直接在任务描述或相关自定义表单字段中使用的任何背景信息。
>* 确保任务与工程师应执行的操作相匹配。 例如，如果指示工程师将文本从英语翻译为法语，请在任务说明中包括要翻译的文本。

## 工作代理启动触发器

当工作座席分配给任务时，它会在满足以下任何情况时开始工作：

* 工作代理分配给准备启动的任务。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 工作代理和用户被分配给任务，工作代理首先被分配。
* 已为其分配工作代理的任务变为准备开始，且工作代理是唯一或主要被分配人。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 已经为其分配了工作代理和用户的任务已准备好开始，并且工作代理是首先分配的，或者是主要被分配人。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 将用户和工作代理分配给任务，并移除该用户。
* 将用户和工作代理分配给任务，并且工作代理被设置为任务的主要被分配人。

以下情况不会导致工作代理开始处理任务：

* 将工作代理分配给已分配了用户的任务。
* 在任务中@mentioned用工作代理。
* 将工作代理分配给已经分配了工作代理的任务。 在这种情况下，分配的第一个工作代理将已开始工作，而第二个工作代理将不执行任何操作。
* 工作代理被分配给未准备好启动的任务。 （例如，如果任务具有前置任务，则前置任务尚未完成。）

## 将工作代理分配给任务

工作代理分配给任务的方式与用户分配方式相同。

在可用受分配人列表中搜索工作代理时，工作代理的名称仅为名字。

有关说明，请参阅[分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)。

>[!NOTE]
>
>不能将工作代理分派给审阅或批准文档。

## 工作代理疑难解答

如果您的工作代理未返回响应或输出，请检查以下各项：

* 确保您的代理发布在AI平台提供商端。
* 请确保您拥有工程师平台所配的足够的AI积分。
* 确保对任务采取的操作不需要特定的访问级别。
* 如果您使用Copilot作为代理提供商，请确保您使用的是“无身份验证”设置。
* 如果您使用的是Copilot，请确保在全球环境中配置了您的代理。 工作代理功能当前不支持Copilot Studio的区域版本。
* 确保Collaborator是任务的主要被分配人。
* 确保分配给工作代理的任务可以启动。 例如，检查以查看该任务的所有前置任务是否已完成。

>[!TIP]
>
>您还可以转到代理提供程序平台，要求代理在该平台内执行任务。 如果代理无法在平台内执行任务，则工作代理也会在Workfront中遇到问题。
