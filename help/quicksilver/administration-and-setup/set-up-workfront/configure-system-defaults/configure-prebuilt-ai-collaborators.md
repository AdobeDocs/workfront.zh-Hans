---
user-type: administrator
product-area: system-administration;setup
title: 配置预建的AI协作者
description: 作为Adobe Workfront管理员，您可以将Adobe中预建的AI协作者（如接收协调员）配置为用户可以分配给任务和问题的工作代理。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c95c5a71a2706d4ddbf3e53a579b348bd072a04e
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 4%
---
# 配置预建的AI协作者

## 概述

预先构建的AI协作者是Adobe中现成的工作代理，这些工作代理经过设置以执行特定工作，例如检查请求中缺少的信息。 它们作为Adobe本机工作代理提供，因此您无需在外部平台中配置代理或提供外部平台凭据。

配置工作代理时，可以选择预构建的协作器作为代理的源。 然后，您可以命名工作代理，设置其访问级别，并选择可以执行的操作。 用户将配置的工作代理分配给任务或问题，其方式与分配任何其他工作代理相同。 用户无需知道代理是预建的协作者。

有关工作代理和其他AI协作器类型的详细信息，请参阅[配置AI协作器](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>Select、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]或组管理员</td> 
  </tr> 
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

贵组织必须启用Adobe CX Coworker。 有关详细信息，请参阅[Workfront中的CX Enterprise Coworker概述](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

## 配置预建的AI协作器

在配置工作代理时，您可以配置预建的AI协作器。 在&#x200B;**选择代理的原点**&#x200B;区域，选择&#x200B;**Adobe Native**，然后从下面的列表中选择要使用的预建Collaborator。

有关完整步骤，请参阅[在Workfront中配置工作代理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront)。

配置Collaborator后，用户可以将其分配给任务或问题。 有关详细信息，请参阅[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。

## 可用的预建AI协作者

### CX Enterprise Coworker {#cx-enterprise-coworker}

由Adobe Agent Orchestrator提供支持的CX Enterprise Coworker代理。

有关详细信息，请参阅[Workfront中的CX Enterprise Coworker概述](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

### 接收协调器 {#intake-coordinator}

接收协调器检查请求的详细信息、自定义表单和附件，以查找缺失、不明确或不一致的信息。 它发布反馈或在获得用户批准的情况下进行更改。

>[!NOTE]
>
>在创建接收协调器规则时，您可以为其分配路由规则，但以后不能进行分配。

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
