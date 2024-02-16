---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3其他增强功能
description: 本页介绍了20.3版本对生产环境所做的所有其他增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3其他增强功能

本页介绍了20.3版本对生产环境所做的所有其他增强。 这些增强功能在2020年8月10日这一周的生产环境中提供。

有关20.3版本可用的所有更改列表，请参阅 [20.3发行版概述](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## 使用专用链接共享日历

为了减轻在Workfront中共享日历的负担，您可以共享可将用户直接转至日历的专用链接。 该日历必须与该用户共享，并且用户必须登录才能查看该日历。

以前，您可以共享不需要登录即可查看的公共URL。

有关更多信息，请参阅 [共享日历报告](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## 创建请求时的新建草稿区域

为在处理请求时为您提供更大的灵活性，Workfront现在会自动将您创建的每个请求另存为新草稿区域中的草稿。 如果您没有完成新请求所需的全部信息，可以将其保留为草稿，稍后返回并完成。 Workfront会在新的草稿区域中为每个队列主题保存一个请求。 草稿请求可以保存您所需的时间，直到您准备完成并提交为止。 也可以使用“布局模板”在左侧面板中移除或重新放置草稿区域。

有关创建请求的更多信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>对于预览版本，如果您分配了自定义布局模板，则需要通过修改布局模板来添加请求的草稿区域。

## 展开或折叠工时表上的项

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

为了帮助您轻松管理包含多个项目的时间表，您现在可以通过单击按钮来展开或折叠所有项目。

以前，必须分别单击每个项目。

有关更多信息，请参阅 [记录时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 忽略Workfront日历中的实际日期

>[!NOTE]
>
>此功能于2020年6月5日发布到“预览”环境。 该版本将于2020年6月19日在生产环境中提供。

为了让您更好地控制对象在日历报表中的显示方式，您可以选择忽略实际日期，即使它们可用。

以前，日历会在实际日期可用时自动使用这些日期。

有关更多信息，请参阅 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## 在日历报告中使用自定义日期字段

>[!NOTE]
>
>此功能于2020年5月29日发布到“预览”环境。 该版本将于2020年6月12日在生产环境中提供。

为了帮助您更好地可视化和管理日常工作日程表，自定义日期字段现在作为日期选项提供。

以前，在实际日期不可用时，您只能通过计划的预计日期管理日历。

有关更多信息，请参阅 [在日历报告中使用自定义日期字段](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (或者，如果您使用的是Workfront Classic，请参阅 [在日历报告中使用自定义日期字段](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US))。

## 电子邮件更改

**出站电子邮件更改：** Workfront的所有电子邮件将来自notifications@my.workfront.com。 这包括自动警报和用户与用户的通信。

以前，系统管理员可以在电子邮件设置区域添加自定义电子邮件地址。

**入站电子邮件POP回复更改：** 系统管理员将无法再为通知的传入电子邮件回复配置自定义POP电子邮件服务器。

有关更多信息，请参阅 [电子邮件欺骗和POP回复电子邮件更改](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM)现在包含在传出的Workfront电子邮件中

所有传出电子邮件都将包含电子邮件身份验证技术(DKIM)。 最终用户看不到此DKIM签名，但允许在服务器级别进行验证，并强化我们现有的身份验证框架。

## 更新了新版Workfront Experience的注册内容

为了使新Workfront体验中的用户注册更易于管理，组管理员现在有权注册和取消注册属于他们管理的组的用户。

现在还有一个用户详细信息链接，它显示以下用户信息：

* 名称
* 工作角色
* 电子邮件地址
* 个人资料图片

## 管理员的新增功能：适用于特定组、团队、工作角色和用户的Brand Workfront

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

现在，您可以使用布局模板更改顶部导航区域和“主”菜单上的徽标，以放置具有自己的品牌的特定组、团队、工作角色和用户。

有关更多信息，请参阅 [打造您的Adobe Workfront实例](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## 组管理员可以创建和管理审批流程

为了允许对其组的工作流拥有更多自主性和控制权，组管理员现在可以访问“设置”中的“审批流程”区域，并为他或她管理的组创建和编辑审批流程。 这些批准流程基于该组的状态。

为了确保组管理员不会无意中编辑在整个系统中使用的或由其他组创建的批准流程，他们只能访问与其管理的组关联的批准流程。

有关更多信息，请参阅 [创建工作项的审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 对于管理员：使用“新建组”页面可更轻松地创建和管理组

现在，组管理员可以更轻松地管理组，因为他们所需的一切信息都可以在新的组页面上找到。 不再需要在各种叠加框和设置页面之间导航来创建和修改组。

以下是主要亮点：

* 组详细信息：查看和编辑有关组的基本信息，如组名称、说明、组管理员姓名以及组是公用还是专用。
* 组成员列表：查看所有组成员并使用新工具栏快速添加、删除、导出、激活和停用成员资格。 您还可以编辑成员的用户档案，并向他们发送更新注释。
* 标题中的“组管理员”字段：查看您管理的组时，快速分配或取消分配作为组管理员的组成员。 您也可以使用新的“组角色”列在组成员列表中执行此操作。
* 子组列表：查看、编辑、复制、导出和删除您管理的组中的子组。
* 状态列表：查看和管理组的状态。

有关更多信息，请参阅 [创建组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 管理员的新增功能：创建最多14级的子组

为了更便于组织您的Workfront组以匹配您的组织层次结构，我们已将您可以在组中创建的子组级别从3提高到14。

有关更多信息，请参阅 [组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 管理员的新增功能：新增设置侧栏

>[!NOTE]
>
>此功能仅在新的Adobe Workfront Experience中可用

现在，“设置”中的左侧边栏变得更快、更易于使用，并利用了您已了解的基本布局和功能。 除了更现代的外观和感觉，还有新增功能：

* 侧边栏中新的非白色背景可让您更轻松地与“设置”区域的其余部分区分开来。
* 侧栏中的图标稍微大了一些，有些图标经过重新设计，以更清楚地说明该选项的作用。
* 侧栏项目之间的垂直间距越大，阅读起来越轻松。
* 当在主区域需要空间来查看和执行更多操作（如查看其他列）时，可以折叠侧栏。 当您需要查看特征名称时，可以再次展开侧栏。
* 当侧栏处于折叠状态时，您只会看到每个功能的图标。 要查看主侧栏项目下的子项目，请将鼠标悬停在其图标上，以弹出菜单显示它们。 例如，将鼠标悬停在流程图标上可显示包含批准和里程碑路径的菜单。
* 只需单击一下即可访问两个Kick-Start选项（导入数据和导出数据）。 它们已从系统下移出以在侧栏的主级别上显示。

有关如何使用“设置”区域的信息，请参阅 [管理和设置](../../../administration-and-setup/administration-and-setup.md).

## 在客户信息区域包含群集编号

作为Workfront管理员，您现在可以在Workfront中轻松找到群集编号，而无需花费额外的时间和精力从我们的支持团队获得该编号。 我们在“Setup（设置）”的“Customer Info（客户信息）”区域添加了“Cluster Setup（群集设置）”字段。

有关“客户信息”区域的信息，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## 事件订阅的Base64编码

base64Encoding字段是一个可选字段，用于启用事件订阅负载的Base64编码。 如果使用设置为true的base64Encoding字段发出请求，则有效负载中的newState和oldState对象将作为Base64编码字符串交付。 如果您的网络配置不允许在事件订阅中使用特殊字符，则此功能会很有用。

有关详细信息，请参阅 [事件订阅API](../../../wf-api/general/event-subs-api.md).

## 删除了创建重复事件订阅的功能

为了防止投放重复消息，您不能再创建重复订阅。 此外，以前创建的任何重复订阅已被删除。

有关更多信息，请参阅 [常见问题解答 — 活动订阅](../../../wf-api/general/event-subs-faq.md).
