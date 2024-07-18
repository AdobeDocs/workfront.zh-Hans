---
title: 'Adobe Workfront规划最佳实践'
description: 作为营销运营负责人，您可以使用Adobe Workfront Planning为所有团队在营销生命周期中组织工作。 我们建议在开始Workfront规划时采用下面一些最佳实践。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Adobe Workfront规划最佳实践

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

作为营销运营负责人，您可以使用Adobe Workfront Planning为所有团队在营销生命周期中组织工作。

本文记录了在开始使用Workfront规划时推荐的一些最佳实践。

## 什么是Workfront计划？

Workfront规划模块是三个不同但相互关联的Workfront功能之一，这些功能共同创建了营销记录系统。 这三项功能包括：

* **计划**： Workfront计划中包含的新高级功能。

* **工作流**：您当前在Workfront中使用的协作工作管理功能（项目管理、资源管理等）

* **自动化和集成**：由Workfront Fusion提供支持的全面集成和自动化功能。

Workfront Planning是高度可自定义的。 有关Workfront Planning术语和关键概念的更多信息，请参阅[Adobe Workfront规划概述](/help/quicksilver/planning/general/planning-overview.md)。

## 在设置Workfront Planning之前需回答的问题

熟悉Workfront Planning术语和架构后，即可开始设置新环境。

在设置Planning时，您可能会问自己以下问题：

* **是否要将工作区用于较大的组织组？ 还是应该鼓励人们设置个人的？**

  您可能会发现两者都有很好的用途。 我们建议不要拥有太多工作区，因为它们可能会变得难以管理，并且您的工作流可能过于分散。

  >[!TIP]
  >
  >    在一个Workfront实例中可以具有1,000个工作区。

* **应在每个工作区中创建哪些自定义记录类型？**

  记录类型与Workfront的对象类型类似。 考虑您的工作流并决定哪些记录类型（工作对象、人员对象、分类等） 每个工作流可能都需要。

  有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)

* **如何创建我的记录？ 是否有外部列表或电子表格已包含我需要添加到Planning的记录，我可以使用这些记录？ 是否会根据需要逐步添加记录？ 还是将使用Fusion或自定义API集成导入它们？**

  有关信息，请参阅：

   * [创建记录](/help/quicksilver/planning/records/create-records.md)
   * [Adobe Workfront规划模块](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **我需要为记录创建哪些字段？**

  有关信息，请参阅[创建字段](/help/quicksilver/planning/fields/create-fields.md)。

* **我需要使用哪些Workfront或AEM Assets对象类型连接到Workfront Planning记录类型，才能显示依赖关系并为我的组织创建无缝工作流程？**

  有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)

* **我需要讲述哪些营销日历和视图来讲述我的营销活动？ 我可以向哪些利益相关者提供这些视图以进行无缝协作？**

  有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。


## Workfront规划最佳实践

本节列出了设置Workfront Planning时的几个注意事项和最佳实践指南。

根据您设置的对象或区域来组织指南。

### Workspace

#### 有的工作区和不的工作区

* 为组织级别的工作区的最低容量进行设计

  例如，尝试为所有营销创建一个Workspace

* 定期组织您的工作区。 您可能会发现，您可以修改现有的版本，而不是从头开始构建新的版本。

* 确实要为具有完全不同的操作动作的团队创建新的Workspace。

  “产品开发”工作区应不同于“营销”工作区

* 不要为每一件小事都创建一个独特的工作区。 将工作区更多地看作是一个记录系统，它可使整个组织受益，允许每个人映射工作流和协作，而不是一个用于跟踪个人请求的专用空间。

* 不要为组织内的每个团队或流程创建唯一的工作区。

  营销组织应努力维护一个工作区，以保持可见性，并允许数据在全球计划级别汇总。

  避免为遵循类似流程（例如，EMEA营销与APAC营销）的团队创建类似或重复的工作区，尤其是当这些团队可能会进行向上汇整到公共战略营销活动的工作时。

#### 我应该如何使用工作区部分？

* 创建部分并为它们添加标签，以帮助用户了解如何组织运营生命周期。

  例如，您可以创建一个名为“核心记录”的部分，放置促销活动、战术和交付项。

* 将“赞”记录类型组合在一起。

  您可以创建一个名为“地理位置”的部分，其中包含记录类型，如：地区、国家/地区和城市。

#### 如何管理工作区权限？

* 不要将访问限制为选定的受信任人员组，以免这些人员意外删除记录类型，或者创建不必要的记录类型和字段。

  >[!TIP]
  >
  >在测试版计划中，我们发现许多客户都希望向组管理员授予“管理”权限。

* 请将Planning区域添加到具有Standard许可证的用户的布局模板中。

* 允许具有Standard许可证的用户创建个人工作区。 这为他们提供了一个安全的空间来学习该工具并熟悉它。 这不会对他人造成体验混乱，并可能提高用户的个人工作效率。

  >[!TIP]
  >
  >    建议他们不要将共享个人工作区作为最佳实践。


### 记录类型

#### 单选或多选字段与链接记录类型

* 如果对象将在多个其他记录类型中使用，请构建新的记录类型

  例如，营销活动可以关联到多个目标受众，而战术可以关联到单个目标受众。

* 如果对象需要存储可能在查找中有用的其他元数据值，请构建新的记录类型。

  例如，渠道记录类型（如“电子邮件”）可能会将支持交付项的列表存储为原生元数据或作为与独立“交付项”记录类型的连接。

* 如果您存储的数据只需要限定为单个记录类型，请不要添加新记录类型。 请改用选择字段。

  例如，促销活动记录类型可能有一个名为“促销活动大小”的单选字段，该字段仅在与特定促销活动直接关联时才相关。

#### 如何标记我的记录类型？

创建并标记表示单个构造或名词的记录类型，如“营销活动”

:no_entry_sign:不要创建更好地表示为视图层的记录类型 — 例如，“日历”对于记录类型来说是一个糟糕的选择，因为它不是记录类型本身，而是记录的视图。

### 我应该创建多少层层次结构？

视图

...

工作流

...

### 字段管理

主字段

请务必使用唯一的主字段值，以便在建立连接时更轻松地查找和“选取”这些记录。

建立连接时，用户将按“主要”字段中的值进行搜索，如果它们不是唯一的，用户将无法知道应该选择哪一个。

避免将非唯一值用作主字段，因为这样可能会使用户在使用连接选取器菜单时必须搜索主字段时感到困惑。



克里斯·奥尼尔报道：

另一个需要考虑的不/不是最能使用Planning的用例。 例如，我们今天进行的资源管理讨论。



Alina的笔记：

ExL中的“最佳实践”文章示例： https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

来自Lauren S. https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346现场准备工作的更多信息