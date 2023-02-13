---
title: 22.4项目增强功能
description: 22.4项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 22.4项目增强功能

本页介绍了在“预览”环境中22.4版本所做的所有项目增强功能。 这些增强功能将于2022年10月3日这一周发布。

有关22.4版本中可用的所有更改的列表，请参阅 [22.4版本概述](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## 前置任务详细信息现已可用

要查看任务的前置任务的详细信息，您现在可以将鼠标悬停在“前置任务”列中的前置任务编号上。 “详细信息”(Details)框显示被引用的前置任务和项目、前置任务的计划起始日期和结束日期，以及前置任务的前置任务和后置任务的数量。 您可以展开项目详细信息，以查看有关项目的更多信息。 跨项目前置任务还包含其他信息。

有关更多信息，请参阅 [在任务列表上创建前置任务关系](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## 为任务或问题分配多个团队

为了在管理任务和问题的方式上提供更大的灵活性，我们为任务或问题分配了多个团队。 以前，只能为任务或问题分配一个团队。

>[!NOTE]
>
>此功能当前在“团队”区域的工作负载平衡器中不可用。

有关更多信息，请参阅 [分配任务](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) 和 [分配问题](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## 在“编辑”和“详细信息”区域为项目角色选择智能用户

我们改进了在您将用户添加到以下项目字段（从项目的“编辑”框和“详细信息”部分）时，用户的显示方式：

* 项目所有者

* 项目赞助者

* 资源管理器

现在，当您将用户添加到“编辑”或“详细信息”区域中的任意这些字段时，除了其名称和头像外，还会显示其“主要角色”和电子邮件。 这有助于区分具有相似或相同名称的多个用户。

有关更多信息，请参阅 [编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

注意：有关项目、任务和问题的其他用户字段将在未来版本中使用此功能进行更新。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412390/){target=_blank}

## 计算日期字段始终基于协调的通用时间(UTC)进行保存

现在，您可以确保计算字段中的所有日期函数都保持一致，并且为每个人生成相同的结果，无论自定义数据表达式如何更新，或用户在全球范围内对对象进行协作的位置如何。

现在，所有计算都由一个标准(协调通用时间(UTC))来计算和保存，而不是由为组织实例和单个用户配置文件设置的时区配置来计算和保存。 但是，计算会根据每个用户在其浏览器中设置的各个时区，以自定义形式显示。

以前，计算中的时间设置在以下情况下会有所不同时会造成混淆：

* 如果有人在表单生成器中使用“更新以前的计算”重新计算了计算字段表达式，则日期函数结果由贵组织的UTC时区决定。

* 如果有人编辑了对象，并且导致计算的字段表达式重新计算，则日期函数结果由用户的本地时区决定。 此方案中的计算日期字段结果也将根据UTC进行计算。

有关更多信息，请参阅 [跨时区工作](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## 自定义表单增强功能：Adobe XD和快速过滤器

根据您的反馈，我们引入了以下增强功能，以改进您在管理自定义表单时的体验：

* 添加Adobe XD文件，使自定义表单更加直观和信息丰富。 将表单附加到对象后，使用该对象的用户可以从表单内查看XD文件并与之交互。

   有关更多信息，请参阅 [在自定义表单中添加或编辑图像或其他资产小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* 使用快速过滤器可轻松找到现代化自定义表单和字段列表中的项目。 在管理表单和字段时，还可以享受更好的外观。

   有关快速过滤器的更多信息，请参阅 [将快速过滤器应用到列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412469/){target=_blank}

## 公共测试版 — 针对项目、任务和问题的新过滤体验

项目、任务和问题列表中的过滤已经过重新设计，可帮助您快速创建和共享过滤器。 功能包括：

* 直观的“测试版生成器”界面，用于创建新过滤器

* 将过滤器标记为收藏的功能

* 过滤器堆叠（应用多个保存的过滤器）

* 复制过滤器

* 共享过滤器

* 删除与您共享的过滤器


时间表列表和方案计划员中也提供了新的过滤器体验。

文本模式仍可用于高级过滤器编辑，系统管理员仍可以通过布局模板为所有用户分配默认过滤器。

### 该功能将在何处提供？

* 项目/任务/问题列表

* 场景计划器

* 时间表


### 我们要您的反馈！

通过此公共测试版用户，可以通过单击反馈按钮，直接向处理过滤器体验的团队提交反馈。 我们期待您和您的用户就公共测试版中的新过滤器体验发表意见。 如果您的团队希望直接与产品会面以提供其他反馈，请随时安排在此举行会议：https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### 接下来会是什么？

* 新的分组和视图（也称为列）体验

   我们将开始为分组和视图（也称为列）处理新体验，以使其与新过滤器体验保持一致，并具有与新过滤器体验相同的一些出色功能。

* 在Adobe Workfront的其他区域实施新过滤器

   我们将与产品各个团队合作，在Workfront的其他区域实施新的过滤器体验。


我们希望反复地为您提供价值，因此在新体验和其他领域准备就绪后，我们将继续提供。 请继续观看更激动人心的更新。

有关更多信息，请参阅 [过滤器Adobe Workfront概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) 和 [在Adobe Workfront中创建或编辑过滤器](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3412391/)
