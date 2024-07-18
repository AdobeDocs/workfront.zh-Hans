---
title: 22.4项目增强功能
description: 22.4项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4项目增强功能

本页介绍了22.4版本对“预览”环境所做的所有项目增强。 这些增强功能将在2022年10月3日这一周提供。

有关22.4版本的所有可用更改列表，请参阅[22.4版本概述](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md)。

## 前置任务详细信息现已可用

要查看任务的前置任务的详细信息，您现在可以将鼠标悬停在“前置任务”列中的前置任务编号上。 详细信息框显示被引用的前置任务和项目、前置任务的计划开始和结束日期以及前置任务的前置任务和后续任务的数量。 您可以展开项目详细信息以查看有关项目的更多信息。 此外，还将为跨项目前置任务提供其他信息。

有关详细信息，请参阅[在任务列表](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)上创建前置任务关系。

## 将多个团队分配给一个任务或问题

为了给您管理任务和问题的方式提供更大的灵活性，我们实现了将多个团队分配给一个任务或问题。 以前，只能将一个团队分配给任务或问题。

>[!NOTE]
>
>此功能当前在团队区域的工作负载均衡器中不可用。

有关详细信息，请参阅[分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md)和[分配问题](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md)。

## 在“编辑”和“详细信息”区域为项目角色选择智能用户

当您将用户从项目的编辑框和详细信息部分添加到以下项目字段时，我们改进了用户的显示方式：

* 项目所有者

* 项目赞助者

* 资源管理器

现在，当您将用户添加到编辑或详细信息区域中的任意这些字段时，除了其姓名和头像外，也会显示其主要角色和电子邮件。 这有助于区分具有相似或相同名称的多个用户。

有关详细信息，请参阅[编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

注意：项目、任务和问题的其他用户字段将在未来版本中更新此功能。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 计算出的日期字段始终根据协调世界时(UTC)进行保存

现在，您可以确保计算字段中的所有日期函数都始终如一地工作并为每个人产生相同的结果，而不管自定义数据表达式的更新方式，也不管用户在何处在世界各地协作处理对象。

现在，所有计算都通过一个标准时间(协调世界时(UTC))进行计算和保存，而不是按为您的组织实例和单个用户配置文件设置的时区配置进行计算和保存。 但是，计算会根据每个用户在浏览器中设置的各个时区，以自定义表单显示。

以前，计算中的时间设置在这些情况下变化时会导致混淆：

* 如果有人在表单生成器上使用“更新以前的计算”重新计算已计算的字段表达式，则日期函数结果由组织的UTC时区确定。

* 如果有人编辑了对象并且导致计算字段表达式重新计算，则日期函数结果由用户的本地时区决定。 此方案中的计算日期字段结果也将基于UTC进行计算。

有关详细信息，请参阅[跨时区工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)。

## 自定义表单增强功能：Adobe XD和快速过滤器

根据您的反馈，我们引入了以下增强功能，以改进您在管理自定义表单时的体验：

* 添加Adobe XD文件，使自定义表单更直观且信息更丰富。 将表单附加到对象后，使用该对象的用户可以从表单中查看和交互XD文件。

  有关详细信息，请参阅[在自定义表单中添加或编辑图像或其他资源小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)。

* 使用快速筛选器轻松地在现代化自定义表单和字段列表中找到项目。 此外，在管理表单和字段时还可体验更佳的外观。

  有关快速筛选器的详细信息，请参阅[将快速筛选器应用到列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 公共Beta — 项目、任务和问题的新过滤器体验

重新设计了项目、任务和问题列表中的筛选功能，以帮助您快速创建和共享筛选器。 功能包括：

* 用于创建新过滤器的直观“测试版生成器”界面

* 将过滤器标记为收藏的功能

* 筛选器栈叠（应用多个已保存的筛选器）

* 复制筛选器

* 共享筛选器

* 删除与您共享的过滤器


新的过滤器体验还可在时间表列表和Scenario Planner中找到。

文本模式仍可用于高级筛选器编辑，系统管理员仍可通过版面模板为所有用户分配默认筛选器。

### 在哪里可以找到它？

* 项目/任务/问题列表

* 场景计划器

* 工时表


### 我们需要您的反馈！

借助此公共Beta，用户可以通过单击反馈按钮，直接向处理过滤器体验的团队提交反馈。 我们期待您和您的用户在公共测试版中了解新的过滤器体验。 如果您的团队希望直接与产品会面以提供其他反馈，请随时在此处安排会议： https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### 接下来呢？

* 新的分组和视图（也称为列）体验

  我们将开始设计新的分组和视图（也称为列）体验，以便与新的筛选器体验保持一致，并具有一些与新的筛选器体验相同的重要功能。

* 在Adobe Workfront的其他区域中实施新过滤器

  我们将与整个产品的团队合作，在Workfront中的其他区域实施新的过滤器体验。


我们希望通过迭代的方式为您带来价值，因此，随着新的体验和其他领域的准备就绪，我们将继续为您提供价值。 请继续关注更多令人振奋的更新。

有关详细信息，请参阅[筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)和[在Adobe Workfront中创建或编辑筛选器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412391/)
