---
title: 'Adobe Workfront计划常见问题解答'
description: 作为营销运营负责人，您可以使用Adobe Workfront Planning为所有团队在营销生命周期中组织工作。 以下是有关Workfront规划的一些常见问题。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 406cd3f929d3955d196f883bf1830fd0fffe9251
workflow-type: tm+mt
source-wordcount: '1630'
ht-degree: 0%

---


# Adobe Workfront规划常见问题解答

{{planning-important-intro}}

<!-- add to TOC and mini TOC-->

本文包含有关Adobe Workfront Planning最常见问题的列表。

有关Workfront规划的详细信息，请参阅 [Adobe Workfront规划概述](/help/quicksilver/planning/general/planning-overview.md).

## 什么是Workfront计划？

Workfront Planning以前称为Project Maestro ，它是一项新功能，使团队能够集中进行端到端运营计划，如营销活动、销售、产品管理、服务等。 规划让您能够利用自定义记录、跨运营生命周期的灵活连接以及增强所有利益相关者的可见性，来为您的理想记录系统建模。

## Workfront计划如何适应更广泛的Workfront产品？

Workfront规划模块是三个不同但相互关联的Workfront功能之一，这些功能共同创建了营销记录系统。 这三项功能包括：

* 规划： Workfront规划中包含的新高级功能。

* 工作流：您当前在Workfront中使用的协作工作管理功能（项目管理、资源管理等）。

* 自动化和集成：由Workfront Fusion提供支持的全面集成和自动化功能。

## Workfront计划何时发布？

面向一般用户的最新计划Workfront规划版本是2024年8月28日。 有关当前已发布功能的最新信息，请参阅 [Adobe Workfront Planning发布活动](/help/quicksilver/planning/general/release-activity.md).

<!-- To verify this: are we even saying "Beta"? - What happens after the beta program concludes? 

Beta participants that want to leverage Planning in production will be able to purchase it at the GA date. We encourage you to reach out to your sales rep to discuss further details. The environment used for the beta program is not in production and will not be migrated. The data stored in the beta environment will be available until December 2024. -->



客户问题 — 第6/13#1会议



创建摘要的过程（人工智能使用拉入各种文档以动态创建摘要）。 那是Beta版的一部分吗？

我们希望能够测试此功能。

我们是否必须迁移到IMS？

是的，想要购买Planning的客户必须迁移到ABP。

能否提供不同工作区的示例？

您可以在不同的级别设置工作区，而且由于系统的灵活性，您可以在团队和个人级别上真正实现多种目的。 主要用例是较大的集中式工作区，供组织使用。 一些具体的工作区示例包括： ......

工作区是否可以共享资金帐户？

工作区可以相互对话吗？ 还是需要在每个工作区中输入信息？

在其当前状态下，是否可以设置工作区数量的任何软限制(即 性能在此点之后降低)？ 对可设置的工作区数量的任何硬性限制(例如 系统不允许超过此#)？

组织的Workfront实例中最多1,000个工作区。 文档链接： https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/create-workspaces

是否可以插入系统中的当前对象，或者是否必须手动构建所有对象？

您可以创建具有WF项目组合、程序、项目、组和公司的Planning记录类型之间的连接。 建立连接（例如与WF项目的连接）后，即可链接到Planning表中与WF项目的记录。 这意味着WF对象仍将在Workfront中创建和管理，但您可以根据Planning记录进行调整。 您在此提供了一些文档： https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types ，我们还计划召开一个关于Connections的反馈会议！

从测试开始，我注意到，如果您添加大量记录，当这些记录不在表视图中时，它们很难相互区分。 有没有办法让唱片颜色不同呢？ 最好能按颜色对它们进行配置，这样它们就会在时间轴和日历视图中更加引人注目。

人员是Workfront人员还是IMS人员？

Workfront实例

这些列表是否可以链接到多个工作区？

我们计划在工作区之间链接记录类型！ 还没准备好。

您添加的自定义字段是否被锁定到创建它们的记录类型？

不允许我与默认的“开始/结束日期”字段建立连接。 如果要连接到已存在的字段，是否应添加新字段？

是否计划在Planning中将真正的外部查找样式字段作为字段类型？

任何计划在记录中默认具有“Created”、“Created by”、“Modified”和“Modified by”字段 — 这好像是需要添加字段才能跟踪记录的消耗？

由于模块链接至WF中的活动对象，它们是否会受到Planning测试版活动的影响？

我们是否将获得放入Fusion中的更改的更新，或者这是单独管理的内容？

是否计划与画布功能板集成？ 如何报告数据？

很快将推出功能板画布，以便可视化Planning数据

我们是否能够创建工作区模板？

此分类/记录结构是否仅在您购买Planning时才可用？  分类结构也有利于标准Workfront用户

管理员能否创建我们自己的模板？

而不是在Beta测试期间。

您是否都有记录的ERD可用于共享规划模型和记录类型？ 目前不是ERD，但我们提供详细的帮助文章，引导您完成创建和连接记录类型的过程：https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/overview-of-record-types https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-planning/adobe-workfront-planning-architecture/connect-record-types

那么，它的一次性（年度定价）是否对PLANNING有用？在此之后，我们可以根据需要添加尽可能多的用户？ 还是按用户收费？

Planning是一种付费产品，其目标正式发布日期为8月28日，在该日期您必须购买Planning才能在生产环境中使用它。 请与您的销售代表合作以了解更多详细信息。

AI启用是否仅可供WF系统管理员使用？是否可以在特定的访问级别上启用？还是只能为特定的用户（1或2）启用？

最初，只有主要系统管理员具有访问权限，以便他们可以通过访问级别配置其组织中哪些人将获得访问权限。 6月21日之后，我们将向组织的其他成员启用AI，这些成员将拥有或不拥有访问权限，具体取决于系统管理员定义的配置。

此处创建的FIELDS位于何处？ 现有的FIELDS能否从我们为其他对象创建的那些字段中引入？ 它们是否与创建的其他字段不同？

目前，这些字段位于它们创建的记录类型内，但我们在2024年下半年有一项高优先级计划，将Planning和Workfront字段集中到一个集中的字段库中。

我们能否根据在Planning中创建的记录/字段创建报告？

是！ 即将通过Dashbaord画布推出

我们是否也可以使用API提取此数据？

是！ 我们已经提供了API和Fusion Connector。

从营销工作区 — 是最好有一个用于全球营销团队的主工作区，还是最好为每个业务线、国家/地区、品牌等拥有单独的工作区。 我发现最多可以有1000个工作区，并且可能会连接多个工作区。 是否可以在工作区之间链接记录？ 用例是 — 允许每个产品拥有自己的工作区，但共享记录类型。 然后，您会希望看到一个整合了所有内容的共享视图。

我们能否为营销活动引入Portfolio和计划？ 这又会带来项目吗？

是否可以在项目创建时将项目链接到工作区中的记录，而无需转到工作区进行链接？

目前，在项目中我们有Planning部分，其中显示来自Planning记录类型的所有连接记录。 您可以在那些连接中添加或删除记录。 我们很快还将添加链接至任何其他Planning记录类型中记录的功能，即使该连接目前没有任何链接记录。

我了解最终我们将能够从组织外部的人员那里接收信息/数据。 此功能何时在Beta版中可用？

工作区能否用于按工作角色跨营销活动进行资源和容量规划？

我们能够链接工作区记录以启动请求？

办公时间2018年6月

能够将日期链接到连接的Workfront数据。 该报表是否当前在所有级别（项目、项目组合、项目群……）均处于活动状态？

是，可以通过查找字段连接项目。

我如何知道有公开视图可供查看？

共享的公开视图可见

如何在内部共享视图？

每次创建新工作区时，您都必须重新共享视图吗？

是的，每次创建新工作区时，它都会成为新的记录类型。 视图特定于记录类型，因此您必须重新共享。

能否从内容中获取缩略图？ 即，将缩略图设置为.pdf或视频。 我们与创意人员合作，并提供一个可选的缩略图视图，这将是一个很好的让团队继续参与更高级别的会议，这些会议将讨论我们的内容图 — 直接链接到内容也会很好。

您能否自定义超出基本范围的权限？ 目前，对于其他Workfront对象，您可以自定义参与/管理/查看访问权限的功能。

目前，我们只有“工作区”和“查看”级别权限，但没有记录类型或单个记录级别权限。

我们是否可以像自定义缩略图那样自定义工作区图标？

是否有可自定义的API使用我们自己的DAM而不是Adobe的DAM？

我们已经为规划构建了一个公共API，我们还提供了Fusion连接器。 将发布API文档，该文档可用于构建连接。

我在Planning中看到了价值（员工使用Airtable）。 直到现在，我们一直在…… x之后奇怪的后端连接，将绑定到上午10点47分左右