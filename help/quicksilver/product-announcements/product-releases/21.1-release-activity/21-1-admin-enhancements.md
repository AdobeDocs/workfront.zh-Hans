---
content-type: release-notes
keywords: 注释，季度，更新
navigation-topic: product-releases
title: 21.1管理员增强功能
description: 本页介绍在“预览”环境的21.1版本中对管理员所做的所有增强。 这些增强功能将于2021年2月15日这一周的生产环境中提供。
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1管理员增强功能

本页介绍在“预览”环境的21.1版本中对管理员所做的所有增强。 这些增强功能将于2021年2月15日这一周的生产环境中提供。

有关21.1版本中可用的所有更改的列表，请参阅 [21.1版本概述](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## 为复制项目引入新的访问级别设置

为了以系统管理员的身份更好地控制计划员对项目的操作，我们通过引入新设置来允许或禁止计划员复制项目的功能，使访问级别中项目的“编辑”访问权限更加精细。 在进行此项更改之前，当您允许用户访问“编辑”项目时，他们将自动拥有复制这些项目的权限。 通过使用新功能，您可以通过禁用新的“复制”设置，为某人授予编辑项目的权限，而不必拥有复制项目的权限。

如果用户在进行此项更改之前有权访问其访问级别的“编辑项目”，则在发布此功能后，他们将自动启用此设置。

有关计划访问级别的信息，请参阅 [授予对项目的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

有关复制项目的信息，请参阅 [复制项目](../../../manage-work/projects/manage-projects/copy-project.md).

此功能现在包含在 [新Workfront体验中的管理员基础知识，第1部分：用户组织](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) 学习Workfront一号。

## 在对象的自定义表单中，在多选下拉字段中选择所有项目

>[!NOTE]
>
>当您提交新请求时，此功能当前不可用。

在对象的“详细信息”(Details)页面上，当您在自定义表单上填写多选下拉字段时，如果需要选择所有可用选项，可以单击全选。

有关编辑自定义表单上数据的信息，请参阅 [编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 为对象重新计算所有自定义表单字段

现在更容易确保计算自定义字段中的所有数据都是对象的最新数据。 通过新的“重新计算表达式”菜单选项，您可以快速重新计算这些字段中的所有数据。

当某人在对象中的计算自定义字段所引用的另一个对象中编辑数据时，此功能特别有用。

以前，用户必须使用解决方法来确保计算自定义字段中的所有数据都是最新的。 例如，他们编辑了对象以及其他对象，以使用可批量编辑的重新计算选项。

有关更多信息，请参阅 [编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 解锁组管理员的任务和问题首选项

>[!NOTE]
>
>在2021年6月24日之前，该功能一直作为分阶段推出的一部分提供，仅适用于能够解锁群组项目首选项的客户。 现在，它可供所有客户使用。

Adobe Workfront管理员现在可以通过解锁单个任务和问题首选项来为组管理员提供更多自治权。 解锁首选项后，组管理员可以将其配置为其组，以提供每个组的独特需求和内部进程。

有关更多信息，请参阅 [为组配置任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

此功能现在包含在 [新Workfront体验中的管理员基础知识，第2部分：项目设置](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) 学习Workfront一号。

## 分别为项目组合和项目群配置访问级别设置

现在，管理用户对项目组合和项目的访问权限变得更加简单，因为您可以单独配置其访问级别设置。

以前，组合和项目群的访问级别设置会被合并。 这意味着，如果不为程序配置访问设置，就无法像为项目组合配置这些设置一样，反之亦然。

有关配置访问级别的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

有关可以为项目和项目组合配置的访问设置的信息，请参阅 [可配置地访问每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

此功能现在包含在 [新Workfront体验中的管理员基础知识，第1部分：用户组织](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) 学习Workfront一号。

## 在自定义表单中编辑信息时，选中系列中的所有复选框

>[!NOTE]
>
>当您提交新请求时，此功能当前不可用。

在对象的“详细信息”(Details)页面上，在填写包含复选框的“自定义表单”(Custom Form)字段时，如果需要选择所有可用的复选框，则可以单击“全选”(Select All)。

仅当字段包含的复选框数超过2时，才会显示此选项。

有关更多信息，请参阅 [编辑自定义表单字段中的信息](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## 配置Workfront电子邮件允许列表

为了更好地保护您的数据，您现在可以使用电子邮件域允许列表:

* 如果Workfront电子邮件包含存储在Workfront中的报表或文档，则可以控制其转到何处
* 控制电子邮件域可以位于用户在其用户配置文件中指定的电子邮件地址中

例如，如果要保护敏感数据（例如列出风险客户的报表），则只能在电子邮件中包含内部电子邮件域或允许列表域。 这样，用户便无法将该报表(或任何其他Workfront报表)发送到外部电子邮件地址。

有关更多信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) 在文章中 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 为子组分配组管理员

为了更便于贵组织的级别独立运行，我们添加了将组管理员分配给子组的功能。 现在，您可以确保将子组管理委派给适当的人员。

以前，只有顶级组才能具有组管理员，这些管理员管理了顶级组下的所有子组。

有关更多信息，请参阅 [子组的组管理员](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) 在文章中 [子组概述](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

此功能现在包含在 [新Workfront体验中的管理员基础知识，第1部分：用户组织](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) 学习Workfront一号。

## 为组配置事件通知

>[!NOTE]
>
>在分阶段推出中，仅适用于能够解锁群组项目首选项的客户。 这包括群集4和6上的所有客户以及其他群集上的少量客户。 此注释将随着功能对更多群集可用而更新。

Workfront管理员现在可以为组管理员配置顶级组的事件通知，从而赋予组管理员更多的自主权。 子组从其顶部父组继承事件通知配置。

以前，事件通知只能由Workfront管理员在系统级别进行配置，这意味着所有组都必须使用同一组事件通知。

有关更多信息，请参阅以下文章：

* [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [查看和配置群组的事件通知](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

此功能现在包含在 [新Workfront体验中的管理员基础知识，第1部分：用户组织](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) 学习Workfront一号。

此功能现在包含在 [新Workfront体验中的电子邮件和应用程序内通知](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) 学习Workfront一号。

## 在“组”区域中使用组项目和审批流程

如果您是组管理员，那么当您的组项目和审批流程列在“组”区域中时，查看和处理这些项目和审批流程会非常方便。 在群组的主页中，您可以：

* 单击左侧菜单中的项目可查看群组的项目，并为群组创建新项目。 如果已与您共享选定的项目，则可以使用工具栏中的按钮来编辑、导出、复制或删除该项目。

   有关更多信息，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* 单击左侧菜单中的批准可查看和管理与群组关联的所有批准流程。

   有关更多信息，请参阅 [组级别的审批流程](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Workfront管理员也可以使用此功能。

## 查看组中使用和分配的许可证数

要确定许可证的分配情况，您现在可以查看组及其下任何子组中使用的许可证数量。

如果您管理顶级组，则可以查看组（及其子组）中使用的许可证数量以及为组分配的许可证数量上限。

有关更多信息，请参阅 [在新的Adobe Workfront体验中查看群组中分配和使用的许可证数量](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

