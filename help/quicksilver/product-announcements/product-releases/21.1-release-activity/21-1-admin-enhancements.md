---
content-type: release-notes
keywords: 注释，每季，更新
navigation-topic: product-releases
title: 21.1管理员增强功能
description: 本页介绍了在21.1版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1管理员增强功能

本页介绍了在21.1版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在2021年2月15日这一周的“生产”环境中提供。

有关21.1版本的所有可用更改列表，请参阅[21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md)。

## 引入用于复制项目的新访问级别设置

为了让您作为系统管理员更好地控制规划人员可以对项目执行的操作，我们通过引入新设置，使访问级别中的项目编辑访问权限更精确，您可以启用或禁用他们复制项目的功能。 在此更改之前，当您启用用户对编辑项目的访问权限时，他们自动拥有复制项目的权限。 使用新功能，您可以通过禁用新的复制设置来授予某人编辑项目的权限，而无需授予他们复制项目的权限。

在此更改之前，如果您的用户有权在他们的访问级别编辑项目，那么在发布此功能时，他们将自动启用此设置。

有关计划访问级别的信息，请参阅[授予项目访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

有关复制项目的信息，请参阅[复制项目](../../../manage-work/projects/manage-projects/copy-project.md)。

此功能现已包含在新Workfront Experience第1部分：用户组织](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径的[管理员基础知识中Workfront One。

## 在对象的自定义表单中，选择多选下拉字段中的所有项目

>[!NOTE]
>
>目前，当您提交新请求时，此功能不可用。

在对象的“详细信息”页面上，当您在自定义表单中填写多选下拉字段时，如果需要选择所有可用选项，可以单击全选。

有关编辑自定义表单上的数据的信息，请参阅[编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 重新计算对象的所有自定义表单字段

现在，可以更轻松地确保计算自定义字段中的所有数据都是对象的当前数据。 新的“重新计算表达式”菜单选项允许您快速重新计算这些字段中的所有数据。

当有人编辑对象中计算自定义字段引用的另一个对象中的数据后，此功能特别有用。

以前，用户必须使用变通方法确保计算的自定义字段中的所有数据都是最新的。 例如，他们编辑对象以及其他对象以使用可用于批量编辑的重新计算选项。

有关详细信息，请参阅[编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 解锁组管理员的任务和问题偏好设置

>[!NOTE]
>
>在2021年6月24日之前，这仅作为分阶段推出的一部分提供，适用于能够解锁组的项目偏好设置的客户。 现在，所有客户均可使用该功能。

Adobe Workfront管理员现在可以通过解锁各个任务和问题偏好设置来赋予组管理员更大的自主权。 解锁某个首选项后，组管理员可以为其组配置该首选项，以满足每个组的独特需求和内部流程。

有关详细信息，请参阅[为组配置任务和问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

此功能现已包含在新Workfront Experience第2部分：项目设置的[管理员基础知识中](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) Workfront One学习路径中。

## 分别配置项目组合和程序的访问级别设置

现在，可以更轻松地管理用户对项目组合和程序的访问，因为您可以单独配置其访问级别设置。

以前，组合和程序的访问级别设置是组合在一起的。 这意味着如果没有对项目组合进行相同配置，就无法对程序配置访问设置，反之亦然。

有关配置访问级别的信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

有关可以为程序和项目组合配置的访问设置的信息，请参阅[可配置的每个对象类型对功能的访问](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md)。

此功能现已包含在新Workfront Experience第1部分：用户组织](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径的[管理员基础知识中Workfront One。

## 在自定义表单中编辑信息时，选中系列中的所有复选框

>[!NOTE]
>
>目前，当您提交新请求时，此功能不可用。

在对象的“详细信息”页面上，当您填写包含复选框的自定义表单字段时，如果需要选择所有可用的复选框，可以单击全选。

仅当字段包含2个以上的复选框时，才会显示此选项。

有关详细信息，请参阅[编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)。

## 配置Workfront电子邮件允许列表

为了更好地保护您的数据，您现在可以使用电子邮件域允许列表来：

* 控制Workfront电子邮件在包含Workfront中存储的报告或文档时可以转到的位置
* 控制电子邮件域可以使用用户在其用户配置文件中指定的电子邮件地址

例如，如果要保护敏感数据（如列出高风险客户的报表），则只能在电子邮件允许列表中包含内部电子邮件域或域。 这样，用户便无法将该报表(或任何其他Workfront报表)发送到外部电子邮件地址。

有关详细信息，请参阅[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)一文中的[配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur)部分。

## 为子组分配组管理员

为了更便于组织的级别独立运行，我们增加了将组管理员分配给子组的功能。 现在，您可以确保将子组管理委派给合适的用户。

以前，只有顶级组才有组管理员，这些管理员管理顶级组下的所有子组。

有关详细信息，请参阅[子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)一文中的[子组的组管理员](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for)部分。

此功能现已包含在新Workfront Experience第1部分：用户组织](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径的[管理员基础知识中Workfront One。

## 为组配置事件通知

>[!NOTE]
>
>仅对于能够解锁组的项目偏好设置的客户，作为分阶段推出的一部分提供。 这包括群集4和6上的所有客户，以及其他群集上的少数客户。 当功能对更多群集可用时，将更新此注释。

Workfront管理员现在可以赋予组管理员更大的自主权，允许他们为自己的顶级组配置事件通知。 子组从其顶级父组继承事件通知配置。

以前，事件通知只能由Workfront管理员在系统级别配置，这意味着所有组都必须使用同一组事件通知。

有关更多信息，请参阅以下文章：

* [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [查看和配置组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

此功能现已包含在新Workfront Experience第1部分：用户组织](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home)学习路径的[管理员基础知识中Workfront One。

此功能现已包含在Workfront One上的新Workfront Experience](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U)学习路径的[电子邮件和应用程序内通知中。

## 在组区域使用组项目和审批流程

如果您是组管理员，则可以轻松地查看和处理组的项目和审批流程，因为这些项目和审批流程已列在组区域。 从组的主页中，您可以：

* 单击左侧菜单中的项目可查看组的项目并为组创建新项目。 如果选定的项目已与您共享，则可以使用工具栏中的按钮来编辑、导出、复制或删除该项目。

  有关详细信息，请参阅[创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)。

* 单击左侧菜单中的批准，查看和管理与组关联的所有批准流程。

  有关详细信息，请参阅[组级审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)。

此功能也适用于Workfront管理员。

## 查看组中已使用和分配的许可证数量

要确定许可证的分配情况，您现在可以查看组及其下任何子组中使用的许可证数量。

如果管理顶级组，则可以查看组（及其子组）中使用的许可证数量和为该组分配的最大许可证数量。

有关详细信息，请参阅[查看新Adobe Workfront体验中组内分配和使用许可证的数量](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md)。

