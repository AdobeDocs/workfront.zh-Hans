---
title: 22.1管理员增强功能
description: 22.1管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 22.1管理员增强功能

本页介绍了在22.1版本中对“预览”环境所做的所有“管理员”增强。 这些增强功能将在“生产”环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日这一周。

有关22.1版本可用的所有更改列表，请参阅 [22.1发行版概述](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 文档下载记录在“更新”区域

为帮助用户跟踪他们存储在Workfront中的文档的下载情况，当有人下载文档时，系统现在会在更新区域为文档记录一个条目。

>[!NOTE]
>
>我们建议在新上传文档的预览中测试此功能。

有关Workfront如何记录对象的自动更新的信息，请参阅 [系统跟踪更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## 使用访问级别向团队授予访问权限

访问级别区域的新部分为您提供了更精细的控制来管理用户对团队的访问权限。 现在，您可以确定谁可以创建、编辑和查看团队。

这不会更改用户对团队的现有访问权限。

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Blueprint中现在提供组映射

某些Blueprint现在包含组，您可以在安装Blueprint之前对其进行自定义。 您可以将Blueprint中的组映射到Workfront实例中的现有组，或根据需要创建新组。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 自定义Forms区域中的样式更新

自定义Forms区域具有新外观，该区域与新Workfront Experience中的许多其他区域一起处于最新状态。

有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 创建计算自定义字段的诸多增强功能

现在，通过在新的计算编辑器中添加以下内容，可更轻松地创建计算自定义字段：

* 您可以将鼠标悬停在计算中的任何表达式上，以显示有关该表达式的信息，包括说明、使用方法的示例以及帮助文章中指向更多信息的链接。
* 您添加的每个表达式都进行了颜色编码，具体取决于其类型。 这样更容易识别您的表达式并立即识别其类型。
* 行号有助于在较长的计算中识别和引用函数。
* 当您开始键入表达式或字段名称时，将显示可用项列表，以便您选择所需的项。 而且，当您键入左括号时，右括号会自动添加。
* 您可以使用现有对象预览计算结果，而无需离开计算编辑器。

此外，在可自定义的“说明”中，将计算自定义字段的文本悬停在上，您可以显示或隐藏该字段的公式。 如果您认为填写自定义表单的用户不需要该信息，这将很有用。

有关创建计算自定义字段的更多信息，请参阅 [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 查看有关状态和公司的审核日志信息

现在，您可以通过在“设置”的“审核日志”区域查看有关状态和公司的信息，更轻松地排除涉及它们的事件。

例如：

* 您可以查找已重命名、锁定或隐藏状态的人员及其时间。
* 您可以了解从公司中删除某些成员或职位角色的人及其删除时间。

有关查看审核日志信息的信息，请参见 [查看和导出审核日志](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprint公司映射和其他增强

以下Blueprint增强功能现已可用：

* 某些Blueprint现在包含公司，您可以在安装Blueprint之前对其进行自定义。 您可以将Blueprint中的公司映射到Workfront实例中的现有公司，或者在需要时创建新公司。
* 现已提供新的Blueprint类型“组织结构”。 某些Blueprint包含来自多种类型（例如，项目模板和组织结构）的元素。 您可以在目录页面上按Blueprint类型进行筛选。
* 为简单起见，配置页面上的“安装首选项”和“模板所有权”部分已合并到“模板首选项”中。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 更轻松地管理公司成员资格

在公司区域，通过更新的工具栏，可以轻松将现有Workfront用户添加到公司以及删除公司成员。

以前，这些操作仅在编辑公司框中可用。

更新的工具栏还包含上一个工具栏中可用的所有操作，例如编辑成员的用户配置文件信息以及在系统中停用这些信息。

有关更多信息，请参阅 [管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 在新建计算字段窗口中选择表达式和字段

我们将继续让您更轻松地在自定义表单中创建计算字段。 现在，当您单击“最大化”打开新的计算编辑器时，您可以查找并选择所需的表达式和字段。

有关更多信息，请参阅 [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 组可以配置自己的时间表和小时首选项

>[!NOTE]
>
>此功能最初作为分阶段推出的一部分提供，但仅作为21.4版本的一部分提供给群集4上的客户。 此功能将于2021年11月8日对其余所有生产群集可用。

在大型组织中，某些组可能需要单独配置时间表和小时首选项以适合其独特的工作流，而不是继承由系统级别管理员配置的首选项。 现在，Workfront管理员可以解锁系统中所有组的时间表和小时首选项，以便他们能够自行配置。

最近还增加了用于项目首选项以及任务和问题首选项的功能。

有关Workfront管理员如何解锁时间表和小时首选项的信息，请参阅部分 [解锁组的工时表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置时间表和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有关组管理员如何为组配置解锁的任务和问题首选项的信息，请参见 [配置组的工时表与小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## 选择您要为组解锁或重新锁定的多个通知

现在，解锁或重新锁定群组的电子邮件通知变得更加快速和轻松。 现在，您可以选择多个通知，检查您的选择以确保它们正确，然后单击工具栏中显示的新解锁或锁定按钮。

以前，您必须一次解锁和重新锁定一个通知。 Workfront目前有95条通知，因此如果您必须对所有通知或其中许多通知执行此操作，则需花费一些时间。

有关更多信息，请参阅 [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## 对于组管理员：删除组时更容易选择替换组

在删除组时，“删除组”框中的两项改进使您可以更轻松地选择要保留已删除组的用户、工作项和子组的替换组：

* 您可以开始键入组的名称以快速找到它。 以前，只有一个下拉列表是无法键入的。 对于包含多个组的组织来说，这会造成问题，因为您必须滚动浏览列表才能找到所需的组。 此外，下拉列表具有项目限制，因此可能不显示您想要的组。
* 您可以使用新建信息图标来确保选择所需的替换组。 将鼠标悬停在图标上会显示工具提示，其中列出了有关组的信息，例如组上面的组的层次结构及其管理员的名称。

有关更多信息，请参阅 [删除组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## 用于创建计算字段的较大区域

现在，在自定义表单中构建复杂的计算字段变得更加容易。 单击新的“最大化”按钮，打开一个用于构建计算的大型编辑窗口。 完成后，单击“最小化”以继续处理自定义表单。

有关更多信息，请参阅 [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 将自定义表单添加到组

Group对象现在支持自定义表单。 这使您组织中的组能够更轻松地捕获和共享满足其特定需求和工作流程的信息。 用户可以像对其他Workfront对象一样，对组执行以下操作：

* 创建自定义表单
* 附加自定义表单
* 保存自定义表单数据
* 删除自定义表单
* 编辑列表中的自定义数据，并在新的Workfront Experience中编辑组页面的自定义数据

有关自定义表单的信息，请参阅 [自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## 创建OAuth2应用程序以将应用程序与Workfront集成

现在，您可以将Workfront与Workfront未提供内置集成的其他应用程序集成。 通过为要与之集成的应用程序创建OAuth2应用程序，您可以允许该应用程序访问Workfront，同时确保您的数据受行业标准OAuth2安全身份验证协议的保护。

以前，您只能通过内置集成、Workfront Fusion或Workfront API与其他应用程序集成。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## “公司”区域中的界面文本改进

在设置中的公司区域，新的确认消息和细微的措辞更改使管理公司成员资格更容易。 例如，左侧面板中的部分名称“人员”现在为“公司成员”。

有关管理公司成员资格的信息，请参阅 [管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
