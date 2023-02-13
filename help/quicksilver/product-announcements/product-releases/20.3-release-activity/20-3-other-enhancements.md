---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3其他增强功能
description: 本页介绍20.3版本到生产环境的所有其他增强功能。 这些增强功能已于2020年8月10日这一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# 20.3其他增强功能

本页介绍20.3版本到生产环境的所有其他增强功能。 这些增强功能已于2020年8月10日这一周的生产环境中提供。

有关20.3版本中可用的所有更改的列表，请参阅 [20.3版本概述](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## 使用专用链接共享日历

要减轻在Workfront中共享日历的负担，您可以共享将用户直接转到日历的专用链接。 必须与用户共享日历，用户必须登录才能查看日历。

以前，您可以共享不需要登录即可查看的公共URL。

有关更多信息，请参阅 [共享日历报表](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## 创建请求时的新草稿区域

为了在处理请求时提供更大的灵活性，Workfront现在会自动将您创建的每个请求作为草稿保存在新的“草稿”区域中。 如果您没有完成新请求所需的所有信息，则可以将其保留为草稿，返回并稍后完成。 Workfront在新的“草稿”区域中为每个队列保存一个请求主题。 在您准备好完成并提交草稿请求之前，您可以根据需要一直保存草稿请求。 您还可以使用布局模板删除或重新定位左侧面板中的“草稿”区域。

有关创建请求的更多信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>对于预览版本，如果您为自己分配了自定义布局模板，则需要通过修改布局模板来添加请求的草稿区域。

## 展开或折叠工时单上的项目

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

为帮助您轻松管理包含多个项目的工时单，您现在可以通过单击按钮展开或折叠所有项目。

以前，必须逐个单击每个项目。

有关更多信息，请参阅 [日志时间](../../../timesheets/create-and-manage-timesheets/log-time.md).

## 忽略Workfront日历中的实际日期

>[!NOTE]
>
>此功能于2020年6月5日发布到预览环境。 它将于2020年6月19日在生产环境中提供。

为了更好地控制对象在日历报表中的显示方式，您可以选择忽略实际日期（即使这些日期可用）。

以前，日历会在日期可用后自动使用实际日期。

有关更多信息，请参阅 [日历报表概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## 在日历报表中使用自定义日期字段

>[!NOTE]
>
>此功能于2020年5月29日发布到预览环境。 它将于2020年6月12日在生产环境中提供。

为了帮助您更好地使用日历可视化和管理日常工作，自定义日期字段现在作为日期选项提供。

以前，您只能在实际日期不可用时，通过预计的计划来管理日历。

有关更多信息，请参阅 [在日历报表中使用自定义日期字段](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (或者，如果您使用的是Workfront Classic，请参阅 [在日历报表中使用自定义日期字段](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US))。

## 电子邮件更改

**出站电子邮件更改：** 所有来自Workfront的电子邮件都将来自notifications@my.workfront.com。 这包括自动警报和用户与用户的通信。

以前，系统管理员可以在“电子邮件设置”区域添加自定义电子邮件地址。

**入站电子邮件POP回复更改：** 系统管理员将无法再为传入电子邮件回复通知配置自定义POP电子邮件服务器。

有关更多信息，请参阅 [电子邮件欺骗和POP回复电子邮件更改](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## 域名键识别邮件(DKIM)现在包含在传出的Workfront电子邮件中

所有传出电子邮件中都将包含电子邮件身份验证技术(DKIM)。 此DKIM签名对最终用户不可见，但允许在服务器级别进行验证，并增强我们现有的身份验证框架。

## 更新了新Workfront体验中的注册

为了使新Workfront体验中的用户注册更易于管理，群组管理员现在有权注册和取消注册属于他们管理的群组的用户。

现在还有一个用户详细信息链接，可显示以下用户信息：

* 名称
* 作业角色
* 电子邮件地址
* 个人资料图片

## 管理员的新增功能：适用于特定组、团队、工作角色和用户的Brand Workfront

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

现在，您可以使用布局模板更改顶部导航区域和主菜单中具有自己品牌的特定组、团队、工作角色和用户的徽标。

有关更多信息，请参阅 [品牌化Adobe Workfront实例](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## 群组管理员可以创建和管理审批流程

为了允许对其组的工作流拥有更多自主权和控制，组管理员现在可以访问“设置”中的“审批流程”区域，并为其管理的组创建和编辑审批流程。 这些审批流程基于该群组的状态。

为确保群组管理员不会无意中编辑整个系统中使用的或由其他群组创建的审批流程，他们只能访问与其管理的群组关联的审批流程。

有关更多信息，请参阅 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 对于管理员：“新建群组”页面可更轻松地创建和管理群组

由于组管理员需要的所有内容都位于新的组页面上，因此可以更轻松地管理组。 不再需要在各种叠加框和设置页面之间导航来创建和修改群组。

以下是主要亮点：

* 组详细信息：查看和编辑有关群组的基本信息，如群组名称、描述、群组管理员姓名，以及群组是公用还是专用。
* 组成员列表：查看所有组成员，并使用新工具栏可快速添加、删除、导出、激活和停用成员关系。 您还可以编辑成员的用户档案并向他们发送更新评论。
* 标题中的“组管理员”字段：查看您管理的组时，可以快速将组成员分配或取消分配为该组的管理员。 您还可以使用新的“组角色”列在组成员列表中执行此操作。
* 子组列表：查看、编辑、复制、导出和删除您管理的群组中的子组。
* 状态列表：查看并管理组的状态。

有关更多信息，请参阅 [创建群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## 管理员的新增功能：创建多达14个级别的子组

为了更便于组织Workfront组以匹配您的组织层次结构，我们将您可以在组中创建的子组级别从3个增加到14个。

有关更多信息，请参阅 [群组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## 管理员的新增功能：新建设置侧栏

>[!NOTE]
>
>此功能仅在新的Adobe Workfront体验中可用

现在，设置中的左侧边栏变得更快、更易于使用，并且利用了您已经知道的基本布局和功能。 除了更现代的外观外，还有以下新鲜事：

* 侧栏中新增的非白色背景，可更轻松地与“设置”区域的其余部分区分开来。
* 侧栏中的图标会稍大一些，有些图标会经过重新设计，以便更清楚地说明选项的用途。
* 侧栏项目之间的垂直间距越大，它们的阅读越容易。
* 当您需要在主区域有空间来查看和执行更多操作（如查看其他列）时，可以折叠侧栏。 此外，当您需要查看功能名称时，还可以再次展开侧栏。
* 在侧栏折叠时，您只会看到每个功能的图标。 要查看主侧栏项目下的子项目，请将鼠标悬停在其图标上以在弹出菜单中显示它们。 例如，将鼠标悬停在“流程”图标上，可显示包含“批准”和“里程碑路径”的菜单。
* 您可以更快地单击两个“启动”选项（“导入数据”和“导出数据”）。 它们已从“系统”下移出来，以在侧栏的主级别显示。

有关如何使用“设置”区域的信息，请参阅 [管理和设置](../../../administration-and-setup/administration-and-setup.md).

## 在“客户信息”区域中包括群集编号

作为Workfront管理员，您现在可以轻松地在Workfront中找到群集编号，而无需花费额外的时间和精力从我们的支持团队获取该编号。 我们在“设置”的“客户信息”区域添加了“群集设置”字段。

有关“客户信息”区域的信息，请参阅 [配置系统的基本信息](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## 用于事件订阅的Base64编码

base64Encoding字段是用于启用事件订阅负载的Base64编码的可选字段。 如果使用将base64Encoding字段设置为true发出请求，则有效负载中的newState和oldState对象将作为Base64编码字符串进行传递。 如果您的网络配置方式为在事件订阅中不允许使用特殊字符，则此功能将非常有用。

有关详细信息，请参阅 [事件订阅API](../../../wf-api/general/event-subs-api.md).

## 删除了创建重复事件订阅的功能

为防止发送重复的消息，您无法再创建重复的订阅。 此外，之前创建的任何重复订阅都已删除。

有关更多信息，请参阅 [常见问题解答 — 事件订阅](../../../wf-api/general/event-subs-faq.md).
