---
content-type: reference
navigation-topic: betas
title: '报告画布测试版：概述'
description: 有关即将推出的Adobe Workfront报表画布工具的Beta版计划的信息
author: Nolan
feature: Product Announcements
hidefromtoc: true
source-git-commit: 2fa10260b54e4ba2e9ab661ac5a4985a91e69191
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 1%

---


# 报告画布测试版：概述

## 报告画布

目前正在开发新的报告画布工具，这是对Workfront中报告的全面再思考。 在设计报告画布时，我们努力提供可提供最大灵活性的体验以及直观的模块化设计，以便像您这样的用户能够最有效地利用自己的数据来创建和共享报告。 通过新的、统一的报告类型，您可以将几乎每个元素拖放到无限的画布上，很快即可创建可视数据杰作，比以往任何时候都更轻松。

本文包含有关当前私人测试版的信息，该测试版仅限于特定客户。 新的报告画布功能现在正通过画布仪表板部署。 参见 **开发计划** 有关更多信息，请参阅下文。

### 开发计划

我们正处于解决数据质量问题的最后阶段，该问题我们在Reporting Canvas测试版的早期发现中发现了。 我们很快将恢复提供新的可视化图表的工作，扩大可报告Workfront对象的选择，并改善报告创建和分发体验，所有这些对于实现我们的报告画布目标都是不可或缺的。

我们将从23.2版本开始，通过现在在预览环境中可用的新“画布功能板”页面逐步提供这些新体验。 画布功能板允许您在我们构建的新报告功能之外显示现有报告，并且将用作我们部署和测试报告画布新功能的主要环境。 有关启用和使用画布功能板的更多信息，请参阅 [画布功能板概述](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/canvas-dashboards-overview.md).

## 参与测试版

>[!IMPORTANT]
>
>以下测试版信息适用于已包含在Reporting Canvas测试版中的管理员，该测试版不再接受新参与者。 如果您要在添加时测试报表画布的新功能，请参阅 **开发计划** 以上提供了有关启用画布功能板的信息。

### 可用性

报表画布测试版适用于AWS上的所有组织，无论区域如何。

### 加入Beta

报表画布测试版是完全可选的，但只能由Workfront管理员选择加入。 要选择以系统管理员身份加入，请执行以下操作：

1. 选择 **报告（测试版）** 图标(在Workfront实例的主菜单中)。
1. 单击 **接受** 接受条款和条件。
1. 允许将贵组织的数据添加到报告画布（这可能需要几个小时）。
1. 开始使用报告画布。

将贵组织的数据添加到报表画布后，其他系统管理员可以选择以相同的方式逐个加入（无需等待再次添加数据）。

要选择加入非Workfront管理员的其他用户，请执行以下操作：

1. 选择 **报告（测试版）** 图标(在Workfront实例的主菜单中)。
1. 单击 **报告画布权限**.
1. 搜索并选择要参与的特定用户。

   >[!IMPORTANT]
   >
   >您授予报告画布访问权限的用户将有权访问 **所有** 系统中的数据是只读的，无论其查看此数据的标准权限如何。

1. 单击&#x200B;**保存**。
1. 添加 **报告（测试版）** 图标添加到每个所选用户的主布局模板中。 有关更多信息，请参阅 [使用布局模板自定义主菜单](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).
1. 然后，每个用户必须单独导航到 **报告（测试版）** 图标，并接受条款和条件。

### 提交反馈

要提交关于测试版的反馈，请执行以下操作：

1. 在Workfront的报告画布中，单击 **发送反馈** 按钮。
1. 填写表单，然后单击 **提交**.

## Beta版常见问题解答

+++我是否可以将旧版报表迁移到报告画布？

总之，迁移旧版报表在Beta测试版期间不可用。 但是，它是正式发布的计划功能（包含下面描述的一些注意事项）。

虽然使用报告画布构建新报告的障碍已显着降低，但我们理解，引入一些现有报告和仪表板将有助于加快采用过程。 因此，我们希望提供必要的工具和资源，以确保您能够带来任何相关的旧版项目，从而确保您从报告画布的正确立场出发。 但是，由于报告画布对当前报告的工作方式进行了如此根本的改变，因此不可能完全按照现在的情况迁移每个报告或仪表板。

我们当前官方版本中的迁移策略使您能够执行以下操作：

1. 确定相关的报告和仪表板

   1. 让您能够导出系统中所有报告和仪表板的CSV以及任何相关跟踪信息（查看次数、查看时间和查看者）。
   1. 提供对与计划投放一起设置的报告的导出以及收件人。

1. 选择要迁移的报表和功能板，然后单击 **迁移**

   这是单向迁移。 它会创建选定报表和功能板的副本以将其复制到报表画布，并将旧版报表或功能板完整保留在当前报表工具中。

   您可以根据需要多次迁移同一报表或功能板。

1. 在报告画布中，确保已迁移您选择的所有报告和仪表板。
+++

+++为什么我看不到我平常做的所有东西？

为了尽早将测试版提供给我们的客户，我们仅发布了它的Workfront中现在提供的许多对象类型的子集。 以下是测试版中当前支持的对象类型：

* 分配
* 文档
* 文档审批
* 费用
* 小时
* 问题
* 注释
* 项目组合
* 项目
* 项目群
* 任务
* 时间表
* 工作项
+++

+++如果在Beta测试期间Reporting Canvas中出现问题，我组织的数据是否会受到影响？

否. 测试版使用填充到报告画布中的贵组织数据的副本。 虽然这意味着您可以在测试期间安全地尝试而不会影响重要数据，但也意味着在正式发布之前，无法在线编辑报告画布中的数据。
+++

+++我加入后是否可以选择退出Beta版？

Workfront管理员无法选择退出测试版；但是，可以通过执行以下操作删除非系统管理员：

1. 以系统管理员身份登录。
1. 导航到报告画布。
1. 单击报告画布 **权限**.
1. 从已选择加入的列表中删除您要选择退出Beta版的用户。
1. 单击&#x200B;**保存**。
+++