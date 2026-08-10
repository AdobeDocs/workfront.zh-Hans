---
title: 使用任务协作者
content-type: reference
description: 了解如何使用可分配给Workfront任务的任务协作者、AI协作者。
author: Becky
feature: Work Management, Tasks
source-git-commit: a05312fa1def1db593743e5e6d385da0b393d5d4
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 2%

---

# 使用任务协作者

{{highlighted-preview-article-level}}

任务协作者是指可直接分配给Workfront任务的AI协作者，此外还有用于文档和资产审阅的现有审阅者类型AI协作者。 与其他AI协作者一样，任务协作者在“设置”区域中配置，并像用户一样分配给任务。

任务协作者连接到已配置的代理，很像MCP服务器。

有关在Workfront中创建任务协作者的信息和说明，请参阅配置AI协作者一文中的[配置任务协作者](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)。

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

* 必须先在Copilot、Claude或Writer.ai中配置代理，然后才能将其用作“任务协作者”。

## 任务协作者概述

任务协作者是一种在Workfront中将MCP代理分配给特定任务的方法。 您可以在Copilot Studio、Claude或Writer.ai等应用程序中配置代理，然后将该代理作为任务协作者连接到Workfront。 然后，您可以像分配用户一样将其分配给任务。

一些示例工作流可能包括：

* 检测上传到任务的图像，根据提供给代理的条件生成变体，并将新图像上传到任务。
* 从任务描述生成副本，根据代理中配置的准则检查副本，并将副本发布到更新流。
* 读取事件的详细信息，识别缺少的详细信息，并在更新流中发布有关缺少的详细信息的问题。

>[!NOTE]
>
>* 有关代理职责和能力的特定详细信息是在创建代理的应用程序中配置的，而不是在Workfront中配置的。
>* 任务协作者当前支持在Copilot Studio、Claude和Writer.ai中创建的代理。
>* 在Copilot Studio中配置代理时，必须将安全性设置为&#x200B;**无身份验证**。
>* 有关在Workfront中创建任务协作者的信息和说明，请参阅配置AI协作者一文中的[配置任务协作者](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-task-collaborator)。

## 任务协作器启动触发器

当为任务分配任务协作者时，如果满足以下任一情况，任务协作者将开始工作：

* 任务协作者被分配给准备开始的任务。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 任务协作者和用户被分配给任务，任务协作者被首先分配。
* 已为其分配任务协作者的任务变得准备就绪。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 已为其分配任务协作者和用户的任务将变为准备开始。 （例如，如果任务具有前置任务，则前置任务为完成。）
* 将用户和任务协作者分配给任务，并删除用户。
* 用户和任务协作者被分配到任务，任务协作者被设置为任务的主要被分配人。

以下情况不会导致任务协作器开始处理任务：

* 任务协作者被分配给已经分配了用户的任务。
* 在任务中@mentioned有任务协作者。
* 任务协作者被分配给已经分配了任务协作者的任务。 在这种情况下，只有第一个分配的任务协作者开始处理该任务。
* 任务协作者被分配给未准备好启动的任务。 （例如，如果任务具有前置任务，则前置任务尚未完成。）

## 将任务协作者分配给任务

任务协作者被分配给任务的方式与用户被分配的方式相同。

在可用任务接受者列表中搜索任务协作者时，任务协作者的名称仅为名字。

有关说明，请参阅[分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)。
