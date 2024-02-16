---
content-type: release-notes
navigation-topic: 2019-2-release-activity
title: 2019.2项目增强功能
description: 本页介绍了2019.2版本中包含的所有项目增强功能。 此功能计划于2019年5月20日这一周在“生产”环境中可用。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 76292f90-af1a-4740-9b8e-b02a6303625c
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---

# 2019.2项目增强功能

本页介绍了2019.2版本中包含的所有项目增强功能。 此功能计划于2019年5月20日这一周在“生产”环境中可用。

有关2019.2版中所做所有更改的列表，请参阅 [2019.2发行活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.2-release-activity/2019-2-release-activity-overview.md).

## 自定义状态时更快地查找组

现在，“设置”区域中“状态”选项卡上的下拉菜单是预输入菜单。 这允许您快速搜索和查找系统中的任何组，使其更易于自定义状态。

以前，下拉菜单显示的组数量有限。 如果未显示所需的组，则必须导航到“设置”>“组”并查找特定组，以自定义组的状态。

有关更多信息，请参阅 [创建或编辑状态](../../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## 将默认自定义Forms和批准流程附加到任务

您现在可以配置默认自定义表单和审批流程，以便在将任务添加到项目时附加到任务。 您可以在项目级别配置默认设置。

有关在项目级别为任务配置默认自定义表单和批准流程的信息，请参阅 [编辑项目](../../../../manage-work/projects/manage-projects/edit-projects.md) 文章。

## 在任务列表中以粗体显示父任务的整行

在任务列表中，包含父任务的行以粗体显示。 当列表按工作细分结构或按任务编号升序排序时，此更改可见。

## 撤消对任务列表的更改

任务列表上新增的“自动保存”按钮允许您选择是自动保存所做的更改，还是要在保存更改之前查看更改的效果。 此设置适用于任务列表和甘特图。

在此增强功能之前，所有更改始终自动保存。

有关在任务列表中编辑任务的信息，请参阅 [编辑任务](../../../../manage-work/tasks/manage-tasks/edit-tasks.md).

有关在甘特图中编辑任务的信息，请参阅 [更新任务列表甘特图中的信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## 新列表中的新列宽默认值

现在，Workfront会根据每列中的值格式信息自动调整列的宽度。 例如，显示数字的列比显示说明字段的列宽。

在此改进之前，除非另有指定，否则新项目和任务视图中的列宽设置为100像素。

有关列宽的信息，请参见 [修改列宽和顺序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

## 取消激活未使用的对象

>[!NOTE]
>
>此功能在2019.2预览时间范围内直接发布到生产环境。

如果您有不再使用的对象，现在可以取消激活这些对象以将其从列表中隐藏，以防止用户将它们与其他对象相关联。

现在，当您编辑下面的任何对象时，可以指示它们是否应处于活动状态。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。 未设置为“活动”的对象在下拉菜单和要附加到其他对象的前置键入字段中不可见。

* 审批流程
* 公司
* 自定义表单
* 里程碑路径
* 项目组合
* 项目群
* 模板

您当前使用的任何停用操作都会继续按常常态运行，并且不会被删除或阻止。

>[!IMPORTANT]
>
>通过Workfront API创建这些对象时，“isActive”参数的默认值为true。 这是所有对象的新字段，在API版本11之前不可编辑。 以前对于Portfolio已存在此字段，只是默认值为false；从API版本11开始，此字段将更改为默认值true 。

## 在视图中显示计划工作成本(BCWS)和已执行工作成本(BCWP)

您现在可以在项目和任务视图中显示计划工作预算成本(BCWS)和执行工作预算成本(BCWP)。

虽然这些项目绩效指标以前在Workfront的财务计算中被使用，但在进行此增强之前它们在系统中不可见。

有关计算BCWS的信息，请参见 [计算计划工作的预算成本(BCWS)](../../../../manage-work/projects/project-finances/calculate-bcws.md).

有关计算BCWP的信息，请参见 [计算已执行工作的预算成本(BCWP)](../../../../manage-work/projects/project-finances/calculate-bcwp.md).

