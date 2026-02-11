---
title: 构建Bridge：将战略意图与项目关联
description: 了解如何在Adobe Workfront Planning中的高级计划与Adobe Workfront中的工作流日常执行之间创建“战略线程”。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# 搭建桥梁：将战略意图与项目联系起来

{{planning-important-intro}}

了解如何在Adobe Workfront Planning中的高级计划与Workfront中的日常执行之间创建战略线程。 您可以使用连接在策略和执行之间构建桥梁。

本指南面向实施Workfront Planning的Workfront管理员和工作区管理员。

## 将战略与执行相协调的概述

将您的战略与日常工作连接起来将愿景变为现实。 当高层计划与执行同步时，您将创建一个策略线程，确保每个项目和任务都向前推动业务。

要实现这种协调，需要设置一系列技术链接和流程护栏，将Workfront中的工作与Workfront Planning中的战略记录联系起来。

通过缩小规划和行动之间的差距，您可以确保团队的精力始终集中在您的最高优先目标上。

## 通过创建连接建立基础

在桥接规划和执行之前，作为工作区管理员，您必须定义哪些记录类型适用于连接。

### 连接字段概述

网桥从创建连接字段开始。

连接字段用作记录类型之间的技术握手。

此字段类型是Workfront Planning中所有关系的引擎。 它是意图的表达，因为它规定特定记录类型（如渠道策略）允许链接到其他对象类型，无论这些对象类型位于Planning还是Workfront中。

有关信息，请参阅[连接的记录类型概述](/help/quicksilver/planning/architecture/connect-record-types-overview.md)。

### 定义何时创建连接

理想情况下，您必须在创建任何工作之前决定是否需要创建连接。

通过添加连接字段，您可以构建环境以支持策略线程，而不管最终如何创建单个记录。

## 同步设置策略和执行

为了集中战略层，我们建议您在使用Workfront进行战术执行时，将规划记录集中在高级意图上。

这种方法通过以下方式利用这两个模块的独特优势：

* **Workfront规划（战略层）：**&#x200B;保持高水平。 它跟踪促销活动、渠道策略和预算。 它没有噪音，适合行政人员使用。

* **Workfront（执行层）：**&#x200B;管理战术详细信息。 您可以将单个体验或活动作为项目、任务和问题进行管理。 您可以为其分配所有权，并构建用于执行的批准。

## 通过激活桥从意图转到操作

配置连接后，您必须决定如何激活特定策略记录和执行项目之间的链接。

### 使用表引导路径

战略专家和超级用户通常使用表格视图作为其工作台，以随时间推移优化计划。

默认情况下，在表中创建记录不会建立到Workfront的链接。

当用户决定激活链接时，将建立与执行项目的连接。

可以通过以下方式完成此操作：

* 直接从Workfront Planning中的连接字段或从记录详细信息视图中的可选“连接”页面手动创建下游连接项目。

  手动创建会导致空白项目没有特定的自定义表单。

  有关信息，请参阅[连接记录](/help/quicksilver/planning/records/connect-records.md)。

* 使用Workfront Planning自动化自动满足更复杂的需求。

  在表格中选择行时，这些自动操作可用作操作栏中的按钮。

  这允许人工监督或创建占位符，确保仅在真正需要项目时才在您的工作流环境中生成项目。

  有关信息，请参阅[使用Adobe Workfront Planning记录自动创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### 构建自动激活

对于具有高容量请求或高级自动化需求的组织，可基于特定事件或请求表单中配置的字段值自动激活桥接器。

此方法需要Adobe Workfront Fusion的许可证。

有关详细信息，请参阅[设置和管理Workfront Fusion：文章索引](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc)。

* **使用提交触发器：**&#x200B;由于表单提供单个干净的提交事件，因此它们可以用作Fusion自动化的触发器。 Fusion场景可以检测表单提交并立即在Workfront中生成链接项目。

* **使用字段值触发器：**&#x200B;若要实现更深入的自动化，您可以配置Fusion以监视特定字段。 例如，标记为“执行就绪”的简单复选框可以用作催化剂，在检查桥接器时自动建立桥。

## 将查找字段添加到曲面可见性

链接项目后，您可以通过添加该项目的查找字段，直接在Planning记录中显示Workfront的实时数据。

作为工作区经理，您可以设置查找字段以将链接项目中的任何系统或自定义字段(例如实际完成日期或Creative潜在客户)提取到Planning记录类型中。 捕获这些数据后，该数据可以累计到您的战略层次结构的多个级别，一直到营销活动级别。 这在整个营销生命周期中为利益相关者提供了强大的汇总报告，无需离开规划环境即可随时了解情况。

## 通过将战略与行动联系起来，实现可视性

这座桥的最终价值在于实时可见性。

通过将意图与行动联系起来，您可以一目了然地回答关键业务问题。 以下是这些问题的示例：

* 我们的“2026财年品牌认知度”活动是否正在积极取得成效？

* 我们的战略策略在哪里需要更多创造性支持才能与时俱进？

* 我们如何根据最优先的战略支柱调整资源？

## 最佳实践和提示

### 待办事项：

* **使用“策略线程”隐喻：**&#x200B;提醒团队每个项目都应该是策略字符串上的“珠子”。

* **自动切换：**&#x200B;使用自动触发项目创建，以节省时间和精力，同时改善数据连接和治理。

* **链接，不重复：**&#x200B;使用查找字段在策略记录中显示实时执行数据（如状态或完成日期）。 这可确保您的战略视图始终是准确的，无需团队手动更新。

### 不要：

* **不要将计划记录视为任务列表：**&#x200B;桥旨在将战略意图与执行项目联系起来。 让您的规划记录重点放在“什么”和“为什么”上，让工作流模块处理任务和问题的精细化“做法”。

* **不要过度同步：**&#x200B;您不需要将每个项目级别的详细信息同步回Planning。 保持策略层高水平且无噪音。

* **不要绕过桥接器：**&#x200B;如果工作开始于“工作流”模块且没有指向Planning的链接，则您已创建领导不可见的“影子计划”。

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



