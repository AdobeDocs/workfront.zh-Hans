---
title: 22.2&amp；nbsp；项目增强功能
description: 22.2&amp；nbsp；项目增强功能
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# 22.2项目增强功能

本页介绍了22.2版本对“预览”环境所做的所有项目增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日这一周。 有关22.2版本的所有可用更改列表，请参阅[22.2版本概述](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)。

## Adobe Workfront展示板现已可用！

展示板是一种灵活的工具，通过提供对包含列和卡片的共享展示板的访问，允许团队协作。

使用展示板，您可以：

* 快速设置包含多列的任务板
* 配置列以显示状态或类别
* 将其他用户添加到展示板并将他们分配到信息卡
* 快速添加未结卡片和核对清单

请注意，展示板上的信息卡未连接到Adobe Workfront中的对象和工作项。

系统管理员必须在布局模板中启用展示板，以便该选项在主菜单中可供所有用户使用。

有关详细信息，请参阅[讨论区概述](../../../agile/boards-overview.md)。

## 对Workfront展示板的其他改进

Workfront展示板现在提供以下其他改进：

* 展示板上的标记卡

  您现在可以使用颜色编码的标记对展示板上的卡片进行分类。 标记允许您快速识别卡片。 您甚至可以根据应用的标记对展示板进行排序。

* 在展示板上管理信息卡

  我们添加了以下功能来帮助您管理展示板上的信息卡：

   * 复制信息卡：创建展示板上现有信息卡的副本。
   * 移动信息卡：使用新的“列顶部”和“列底部”菜单选项，将信息卡快速移动到展示板的顶部或底部。

* 在讨论区中搜索

  我们添加了搜索栏，以帮助您搜索展示板上的所有信息卡。

* 在展示板中设置卡的到期日期

  您现在可以为展示板上的各个信息卡设置截止日期。

有关详细信息，请参阅[Adobe Workfront中的讨论区入门](../../../agile/get-started-with-boards/get-started-with-boards.md)。

## “更新帖子”的“还原”选项

现在，在发布更新时更容易发现错误。 现在，在对象的“更新”选项卡中完成评论时，会创建一个弹出窗口，持续7秒，允许您在系统为其设置时间戳或发送任何电子邮件和应用程序内通知之前取消帖子并返回编辑。 如果关闭弹出窗口，离开页面，或等待窗口超时7秒，则正常开机自检。

有关详细信息，请参阅[更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 更新了复制和移动问题时的体验

为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们重新设计了用于复制和移动问题的界面。 目前，在复制或移动单个问题，或者从列表或报告批量复制或移动问题时，此功能可用。

此新设计的界面的一些改进包括：

* 移动之前必须更新的所有信息都会显示在一个连续的页面上。
* Workfront会检查您是否有权在选择项目后立即访问目标项目。 在作出此改进之前，Workfront警告您，确认移动后您不再具有正确的访问权限，这会导致额外的步骤，并且不允许移动。
* 能够在不离开“移动任务”框的情况下请求对要移动问题的项目的访问权限。
* 将问题移动到其他位置时，能够从问题中删除项目（分配、进度、文档、权限、更新）。 此功能以前仅可用于复制问题。
* 在复制问题时，除了选择目标项目之外，还能选择目标任务。

有关移动或复制问题的更多信息，请参阅以下文章：

* [复制问题](../../../manage-work/issues/manage-issues/copy-issues.md)
* [移动问题](../../../manage-work/issues/manage-issues/move-issues.md)

## 复制项目时的新体验

为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们重新设计了用于复制项目的界面。 当前在从项目页面复制项目时，或者从列表或报表复制项目时，此功能可用。 在此更新之前，您只能从项目页面复制项目。

有关详细信息，请参阅[复制项目](../../../manage-work/projects/manage-projects/copy-project.md)。

## 能够通过新的“更多”菜单从列表和报告管理项目

我们在项目列表和报告中添加了新的“更多”菜单，允许您从这些区域执行以下操作：

* 对于同时执行多个项目：
* 重新计算时间线
* 重新计算财务
* 重新计算自定义表达式
* 对于单个项目：
* 附加模板
* 导出至 MS 项目
* 订阅

有关更多信息，请参阅以下文章：

* [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [重新计算项目财务](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [将项目导出到Microsoft项目](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [订阅Adobe Workfront中的项目](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## 将问题转化为项目后，将用户保留在功能板、列表或报表上

为了提高效率并消除点击次数，在从列表、报告或仪表板将问题转化为项目时，我们发布了一项改进。

将问题转化为项目后，用户仍保留在列表、报表或功能板中，而不是被重定向到项目的页面。 转换完成后，将显示一个成功通知，其中包含指向项目的链接，以便您根据需要轻松导航到项目。

有关详细信息，请参阅[在Adobe Workfront中将问题转化为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)。

## 对分配进行更改时，不再删除分配小时数

>[!NOTE]
>
>此功能原计划随22.2版一起发布。 它将在2022年4月21日发布到生产环境。

为了确保数据的准确性，我们在更改任务的分配时，进行了相应更改，以保留分配小时数，并保留任务计划小时数不变。

已对具有简单持续时间类型的任务进行了以下更改：

* 删除所有被分配人时，保留计划的小时数。
* 替换用户和角色时，会保留单独的分配分配。
* 删除用户时，会保留角色上的各个分配分配。 (已从版本中删除。 现在，计划小时数在删除所有被分配人后将设置为0。)

有关计划小时数的详细信息，请参阅[计划小时数概述](../../../manage-work/tasks/task-information/planned-hours.md)。

## 仅在文件夹层次结构的前五个级别中共享文件夹

>[!NOTE]
>
>此功能暂时不可用。 当该功能在生产环境中可用时，我们将更新此发行说明。

为确保用户共享文件夹获得最佳性能，我们当前将共享限制为对象上文件夹层次结构中的前五个级别。

第六级或更低级别的每个文件夹都从其正上方的文件夹继承其共享配置。

有关共享文件夹的详细信息，请参阅[共享文档文件夹](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

