---
title: 架构您的成功：建模您的营销活动层次结构
description: 了解如何使用“重心”和多工作区架构，将复杂的业务流程转换为可扩展、受管理的活动层次结构。
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# 架构您的成功：建模您的营销活动层次结构

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning，它是Adobe Workfront的一项附加功能。
>
>您的组织必须具有Workfront Planning Prime或更高版本包，才能支持本文中推荐的功能。
>
>有关访问Workfront Planning的要求列表，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。
> 
>有关Workfront Planning的一般信息，请参阅[Adobe Workfront Planning入门](/help/quicksilver/planning/general/planning-overview.md)。

了解如何使用Adobe Workfront Planning中的重心和多工作区架构，将复杂的业务流程转换为可扩展、受管理的活动层次结构。

本指南面向在Workfront Planning中实施和设计环境架构的Workfront管理员和高级用户。

## 成功架构概述

随着营销操作的成熟，数据的复杂性也会随之提高。 如果没有清晰的Blueprint，您的营销记录系统可能会很快变成一个垃圾桶，里面充斥着断开连接的记录、相互冲突的术语和报告孤岛。

当您构建成功的架构时，需要在Workfront Planning中构建用于建模活动层次结构的框架。 它将您从电子表格混乱转变为受控制的面向对象模型，确保每个团队都说相同的语言，同时保持他们执行所需的灵活性。

## 构建层次结构以定义意向级别

为了保持清晰度和可扩展性，我们建议在Workfront Planning中设计工作流时，从经验证的核心路径开始。

从那里，您可以通过向架构添加更多级别来扩展您的策略。

### 核心路径：如何从战略走向行动

虽然组织可以随着其运营需求的演变而扩展此层次结构，但从以下各节所述的三个级别开始，可确保战略和执行之间架起一座稳固的桥梁。

从我们的发现中，我们注意到Workfront Planning的大多数成功实施都基于一种干净的三层模型，这种模型同时涵盖Planning和Workfront。

下面是成功的Planning实施的级别，以及您可能考虑创建以在流程中为您提供支持的对象：

* **第1级：营销活动(Workfront规划)**

   * **焦点：**&#x200B;定义长期战略支柱和年度计划。 例如，为您的组织定义一个称为“2026财年全球品牌意识”的计划。 这是给定时间范围内的焦点。 创建营销活动以支持此计划。

   * **角色：**&#x200B;此级别的利益相关者可以是营销官员、营销副总或其他战略潜在客户。

  有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

* **第2级：渠道战术(Workfront规划)**

   * **焦点：**&#x200B;定义概述特定渠道的“内容”的操作摘要。 这是工作开始前战略意图的最后一层。 例如，创建“第1季度社交媒体闪烁”策略。 然后，您可以将其与营销策划配对。

   * **角色：**&#x200B;主要利益相关者是营销运营负责人、渠道负责人或营销活动经理。

* **级别3：项目(规划和Workfront)**

   * **焦点：**&#x200B;根据最终完成计划的确切体验或活动执行。 某些交付项是具体的，例如社交帖子、电子邮件和网页。

   * **实施：**&#x200B;您可以在Planning中创建策略，并将它们直接链接到Workfront中的&#x200B;**项目**，其中各个交付项作为任务和问题进行管理。

   * **角色：**&#x200B;这里的主要利益相关者是创意人员、个人贡献者以及负责支持计划工作的任何人。

### 战略扩展：如何添加更多级别

建立核心路径后，在仔细考虑具体业务复杂性后，您可以选择添加其他层。

您可能会发现创建以下附加项目很有用：

* **渠道计划：**&#x200B;营销活动和战术之间的层，用于将跨职能策略分组。 例如，一个名为“数字战略”的计划。

* **活动：**&#x200B;如果您在低容量环境中工作（您每年可能有5,000个或更少的可交付项目），则某些团队可能倾向于在成为Workfront项目之前按照Workfront Planning记录跟踪个别体验。

>[!IMPORTANT]
>
>如果贵组织每年生产5,000多项活动，则应将各个可交付结果跟踪移至Workfront。
>
>在Planning中管理大量体验记录可能会导致数据累积，从而模糊您的战略可见性。
>我们建议采用这一宽泛的准则来最大限度地提高效率：
>
>* 使用Planning了解“原因”和“内容”
>* 将Workfront用于大容量“如何”。

## 了解重心以构建您的体系结构

企业级营销记录系统并非构建在单个工作区中。 它采用“轴辐式”架构，在这种架构中，记录类型在其自然的重心进行管理。

有关详细信息，请参阅[推出您的战略主页：30天启动板](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md)。

要使用轴辐式方法构建体系结构，您必须创建以下内容：

* 分类中心
* 战略规划工作区
* 功能辐条

### 将分类中心构建为分类

您必须首先为全局分类建立一个集中式工作区，以定义组织中每个人都必须了解的主要概念。 例如，在中央工作区中创建以下记录类型：品牌、地区、产品、角色。

有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

在创建分类时建立以下内容：

* **主要位置：**&#x200B;选择一个主要工作区。 此工作区应该是您创建的记录类型的真实来源。

* **优势：**&#x200B;通过将这些定义整合到其他业务部门，您可以解决以下问题：“地区：欧洲、中东和非洲”等概念对每个团队都意味着相同的问题。

### 创建战略规划工作区作为您的执行中心

执行中心是高级别营销活动（以及任何渠道计划）的所在地。

* **主要位置：**&#x200B;这是执行重心，为战略决策提供无噪音环境。

* **优点：**&#x200B;领导力无需倾听日常战术杂讯，即可管理营销活动组合。

### 将功能轮辐定义为团队的工作区

功能单元(社交、Creative、电子邮件)拥有自己的工作区来管理其策略。

* **主要位置：**&#x200B;这些工作区是本地团队执行的各个重心。

* **优点：**&#x200B;团队使用来自中心的全局促销活动和分类，同时维护自己的本地对象。

  例如，团队可将中央工作区中的营销活动记录类型添加到团队的工作区，但创建仅与团队工作区相关的营销活动。 营销活动的示例为“Media outlets”或“Usage rights”。

## 使用基于名词的治理方法

要确保您的架构承受压力，请遵循基于名词的治理原则。

在Workfront Planning中创建实体时，我们建议执行以下操作：

* **使用名词，而不是动词：**&#x200B;在要跟踪的内容之后命名记录类型（将其命名为“Campaign”或“Tactics”），而不是要执行的操作（不要将其命名为“Campaigning”或“Planning”）。

* **标准化命名法：**&#x200B;在所有工作区中使用相同的名称。 这样，您就可以汇总整个项目组合的数据以进行执行报告。

## 现有项目组合和项目群的情况如何？

成熟组织的一个常见问题是如何处理已在Workfront中构建的项目组合和程序。 过去，这些对象经常被用来模拟战略规划。

现在，我们建议您将该方法转变为Workfront规划方法，这自然符合规划的战略方法。

### 将项目组合和程序替换为记录类型

在许多组织中，项目组合用于表示高级品牌或业务单元，而项目群表示战略主题。

在Workfront Planning中，最好将这些分类建模为分类中心中的“记录类型”。

通过将品牌或业务部门视为记录类型，可以将它们链接到整个企业中的促销活动或策略，从而提供比静态Portfolio — 项目结构更灵活的报告。

### 使用报告桥策略

虽然Workfront Planning是未来战略意图，但其通过Canvas Dashboard的原生报表功能仍在不断完善。

许多组织仍依赖与Workfront中的旧版Portfolio和项目结构关联的强大报表功能。

我们建议查看以下内容：

* 请勿删除您的项目组合和程序。
* 使用Planning自动化功能在记录类型与项目组合和程序之间架起一座桥梁。

  在Workfront Planning中创建策略或营销策划时，该记录可以在Workfront中生成相应的Portfolio或项目。

  有关信息，请参阅[使用Adobe Workfront Planning记录自动化创建对象](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)。

这允许您：

* 通过使用时间轴和日历，尽享Workfront Planning卓越的战略可视化效果。

* 在Workfront中为尚未准备好迁移到画布的利益相关者维护旧版报表。

## 最佳实践和提示

### 待办事项

* **坚持核心路径优先方法：**&#x200B;在增加复杂性之前建立您的营销活动到战术到项目的流程。

* **指定主工作区：**&#x200B;确保每个记录类型都有一个作为报告聚合器的主工作区（请考虑其重心）。

* **为摄取流程排列请求表单的优先级：**&#x200B;在Workfront Planning中使用记录表单来记录不太复杂的组，以确保元数据的完整性。

  >[!CAUTION]
  >
  >虽然高级用户可能会从表格视图中的直接数据输入中受益，但应谨慎对待这一点。
  >对表格进行批量更改可以轻松地为其他利益相关者造成数据难题。

### 不要

* **不要使用一般化：**&#x200B;例如，在谈论执行时，不要谈论“核心”环境，而要特别提到Workfront和Project对象。

* **不要过于复杂：**&#x200B;每增加一个层次结构级别都会增加管理税。 仅添加回答当前无法回答的业务问题的级别。

* **不创建思洛存储器：**&#x200B;确保记录类型在工作区之间共享，这样团队就不会重新键入相同的数据。


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->