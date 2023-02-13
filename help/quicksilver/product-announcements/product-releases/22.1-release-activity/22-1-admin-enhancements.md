---
title: 22.1管理员增强功能
description: 22.1管理员增强功能
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 22.1管理员增强功能

本页介绍在“预览”环境的22.1版本中对管理员所做的所有增强。 这些增强功能将在生产环境中提供

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年1月17日这一周。

有关22.1版本中可用的所有更改的列表，请参阅 [22.1版本概述](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 记录在“更新”区域中的文档下载

为了帮助您的用户跟踪他们存储在Workfront中的文档的下载，现在当有人下载文档时，系统会在“更新”区域中为文档记录一个条目。

>[!NOTE]
>
>我们建议在新上传的文档的“预览”中测试此功能。

有关Workfront如何记录对象自动更新的信息，请参阅 [系统跟踪的更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## 使用访问级别授予团队访问权限

“访问级别”区域中新增了一个部分，通过该部分可以更精细地控制管理用户对团队的访问权限。 现在，您可以确定谁可以创建、编辑和查看团队。

这不会更改用户对团队的现有访问权限。

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Blueprint中现已提供组映射

现在，某些Blueprint包括组，您可以在安装Blueprint之前对其进行自定义。 您可以将Blueprint中的组映射到Workfront实例中的现有组，或根据需要创建新组。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 自定义Forms区域中的样式更新

“自定义Forms”区域具有新的外观，可使其与新Workfront体验中的许多其他区域保持最新。

有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 许多用于创建计算自定义字段的增强功能

现在，通过在新的计算编辑器中添加这些内容，可以更轻松地创建计算自定义字段：

* 您可以将鼠标悬停在计算中的任何表达式上以显示有关该表达式的信息，包括描述、如何使用该表达式的示例，以及指向帮助文章中更多信息的链接。
* 您添加的每个表达式都采用颜色编码，具体取决于其类型。 这样，您就更容易发现表达式并立即识别其类型。
* 行号可帮助您在较长的计算中识别和引用函数。
* 开始键入表达式或字段名称时，将显示可用项目列表，以便您选择所需的项目。 此外，当您键入左圆括号时，将自动添加右圆括号。
* 您可以使用现有对象预览计算结果，而无需离开计算编辑器。

此外，在可自定义的“说明”中将鼠标悬停在计算的自定义字段的文本上，可以显示或隐藏该字段的公式。 如果您认为填写自定义表单的用户不需要该信息，则此功能非常有用。

有关创建计算自定义字段的更多信息，请参阅 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 查看有关状态和公司的审核日志信息

现在，您可以通过在“设置”的“审核日志”区域中查看与状态和公司有关的信息，更轻松地对涉及状态和公司的事件进行故障诊断。

例如：

* 您可以查找谁重命名、锁定或隐藏了状态，以及他们何时重命名、锁定或隐藏状态。
* 您可以了解从公司中删除某些成员或职务角色的人员，以及他们何时删除了这些角色。

有关查看审核日志信息的信息，请参阅 [查看和导出审核日志](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprint公司映射和其他增强功能

以下Blueprint增强功能现已可用：

* 现在，一些蓝图包括公司，在安装蓝图之前，您可以对其进行自定义。 您可以将Blueprint中的公司映射到Workfront实例中的现有公司，或根据需要创建新公司。
* 新的Blueprint类型“组织结构”现已可用。 某些蓝图包括多种类型（例如，项目模板和组织结构）中的元素。 您可以在目录页面上按Blueprint类型进行过滤。
* 为简单起见，配置页面上的“安装首选项”和“模板所有权”部分已合并到“模板首选项”中。

有关更多信息，请参阅 [配置Blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## 更轻松地管理公司成员资格

在“公司”区域中，更新的工具栏可以轻松地向公司添加现有Workfront用户，并删除公司成员。

以前，这些操作仅在“编辑公司”框中可用。

更新后的工具栏还包含之前工具栏中可用的所有操作，例如编辑成员的用户配置文件信息并在系统中取消激活它们。

有关更多信息，请参阅 [管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## 在新的计算字段窗口中选择表达式和字段

我们将继续简化在自定义表单中创建计算字段的过程。 现在，当您单击最大化以打开新的计算编辑器时，您可以找到并选择所需的表达式和字段。

有关更多信息，请参阅 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 组可以配置自己的时间表和小时首选项

>[!NOTE]
>
>此功能最初作为分阶段推出的一部分提供，仅在21.4版本的一部分，面向群集4上的客户。 此功能将于2021年11月8日在生产环境中适用于所有剩余的群集。

在大型组织中，某些组可能需要独立配置工时单和小时首选项以适合其独特工作流，而不是继承由系统级别的管理员配置的首选项。 现在，Workfront管理员可以解锁系统中所有组的工时单和小时首选项，以便他们可以自行配置。

最近还为项目首选项以及任务和问题首选项添加了此功能。

有关Workfront管理员如何解锁工时单和小时首选项的信息，请参阅部分 [解锁组的工时单和小时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) 在文章中 [配置工时单和工时首选项](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

有关组管理员如何配置已解锁任务和发布组首选项的信息，请参阅 [为组配置工时单和小时首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## 选择要解锁或重新锁定组的多个通知

现在，可以更快、更轻松地解锁或重新锁定群组的电子邮件通知。 现在，您可以选择多个通知，检查您的选择以确保它们正确无误，然后单击工具栏中显示的新“解锁”或“锁定”按钮。

以前，您必须一次解锁和重新锁定一个通知。 Workfront目前有95条通知，因此，如果您必须为所有通知或许多通知执行此操作，则需要一段时间。

有关更多信息，请参阅 [解锁或锁定所有组的事件通知配置](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## 对于组管理员：在删除群组时更便于选择替换群组

删除组时，通过“删除组”框中的两项改进，可以更轻松地选择要保留已删除组的用户、工作项和子组的替换组：

* 您可以开始键入组的名称以快速找到它。 以前，只有一个下拉列表无法键入。 对于具有多个组的组织而言，这存在问题，因为您必须滚动浏览列表以找到所需的组。 此外，下拉列表还存在项目限制，因此可能未显示您想要的组。
* 您可以使用新信息图标确保选择所需的替换组。 将鼠标悬停在图标上会显示有关该群组的工具提示列表信息，例如该群组上的群组层次结构及其管理员姓名。

有关更多信息，请参阅 [删除群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## 用于创建计算字段的更大区域

现在，更轻松地在自定义表单中生成复杂的计算字段。 单击新的最大化按钮以打开一个用于生成计算的大型编辑窗口。 完成后，单击最小化以继续处理自定义表单。

有关更多信息，请参阅 [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## 将自定义表单添加到群组

组对象现在支持自定义表单。 这样，贵组织中的群组便于捕获和共享满足其特定需求和工作流程的信息。 用户可以像对其他Workfront对象一样，对组执行以下操作：

* 创建自定义表单
* 附加自定义表单
* 保存自定义表单数据
* 删除自定义表单
* 从列表中编辑自定义数据，在新的Workfront体验中，从群组页面编辑自定义数据

有关自定义表单的信息，请参阅 [自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## 创建OAuth2应用程序以将应用程序与Workfront集成

现在，您可以将Workfront与Workfront未提供内置集成的其他应用程序集成。 通过为要与集成的应用程序创建OAuth2应用程序，您可以允许该应用程序访问Workfront，同时知道您的数据受安全的行业标准OAuth2身份验证协议的保护。

以前，您只能通过内置集成、Workfront Fusion或Workfront API与其他应用程序集成。

有关更多信息，请参阅 [为Workfront集成创建OAuth2应用程序](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## “公司”区域的界面文本改进

在“设置”的“公司”区域中，新的确认消息和细微的措辞更改使管理公司成员资格变得更加容易。 例如，左侧面板中名为“人员”的部分现在为“公司成员”。

有关管理公司成员资格的信息，请参阅 [管理公司成员资格](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
