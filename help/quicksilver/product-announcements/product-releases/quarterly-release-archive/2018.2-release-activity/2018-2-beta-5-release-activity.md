---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 5发行版活动
description: 本页介绍了2018.2 Beta 5版本在“预览”环境中最近提供的所有更改。 该功能将于2018年6月1日在预览环境中可用。 Beta 5中发布的校对增强功能将于6月4日星期一在“预览”环境中提供。 该版本将于2018年7月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

# 2018.2 Beta 5发行版活动

本页介绍了2018.2 Beta 5版本在“预览”环境中最近提供的所有更改。 该功能将于2018年6月1日在预览环境中可用。 Beta 5中发布的校对增强功能将于6月4日星期一在“预览”环境中提供。 该版本将于2018年7月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.2版中所做所有更改的列表，请参阅  [2018.2发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 5版本包含适用于Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**&#x200B;**

* [使用审核日志查看用户触发的更改](#view-user-triggered-changes-with-audit-logs)
* [以组管理员身份查看许可证信息](#view-license-information-as-a-group-administrator)

所有用户&#x200B;**&#x200B;**

* 主页区域中的[日历视图](#calendar-view-in-the-home-area)
* 主页[&#128279;](#additional-updates-to-the-work-list-left-panel-in-home)中的工作列表（左侧面板）的其他更新
* [为自动资源计划配置工作角色限制](#configure-job-role-limits-for-automated-resource-scheduling)
* 资源规划者中的[项目和角色视图改进](#project-and-role-view-improvements-in-the-resource-planner)
* [调整项目列表的列宽](#resize-column-widths-for-project-lists)
* 对新项目列表的[图标支持](#icon-support-for-the-new-project-lists)
* [在文档视图中添加大缩略图字段](#add-large-thumbnail-field-in-document-views)
* [提高Excel导出限制](#increase-excel-export-limit)
* 项目列表的[快速筛选器](#quick-filters-for-project-lists)
* [项目和任务报告中的引用问题集合](#reference-issue-collections-in-project-and-task-reports)
* 在Workfront中添加新文档版本时，[新增更强大的版本菜单](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* Android Beta移动设备应用程序中的[移动设备改进](#mobile-improvements-in-the-android-beta-mobile-app)
* [验证查看器增强功能(Workfront和Workfront Proof)](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* Workfront中的[校对增强功能](#proofing-enhancements-in-workfront)
* [Workfront Proof中的校对增强功能](#proofing-enhancements-in-workfront-proof)

## 主页区域中的日历视图 {#calendar-view-in-the-home-area}

现在，您可以使用Workfront主页日历视图来管理个人工作任务和计划。 “主页日程表”视图允许您执行以下操作：

* 设置您自己的计划，以完成分配给您的Workfront任务
* 快速查看即将到期或过期的任务
* 查看您一周的总分配小时数
* 更新分配给您的任务

如果在Outlook中使用日历，则可以集成日历，以便在“主页日历”视图中显示您的Outlook事件。

## 主页工作列表（左侧面板）的其他更新 {#additional-updates-to-the-work-list-left-panel-in-home}

“主页”区域的工作列表现在提供以下增强功能：

* 现在，已完成项目的数量显示在“过滤器”下拉菜单中的“已完成”选项旁的括号中。

  以前，已完成项目的数量不会显示在过滤器菜单中。 

* 系统会显示前2周已完成的项目。

  以前，会显示过去3个月的已完成项目。

  有关查看“主页”区域中的已完成工作的信息，请参阅[显示主页中的工作列表中的项目](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)中的文章[显示主页中的工作列表中的项目](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 添加持续时间字段和分配字段，以在主页区域中选择项目时显示。

  以前，任务字段默认可用；但是，如果删除它，则无法重新添加它。 Duration字段之前不可添加。

  有关向主页区域添加字段的信息，请参阅创建和管理布局模板。

有关使用主页区域的详细信息，请参阅[使用主页区域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 使用审核日志查看用户触发的更改 {#view-user-triggered-changes-with-audit-logs}

我们为Workfront管理员创建了以下审核日志，以跟踪用户触发的更改：

* 用户审核日志
* 访问级别审核日志
* 组审核日志
* 登录尝试审核日志

以前，无法跟踪系统内的更改。

有关详细信息，请参阅[查看和导出审核日志](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)。

## 以组管理员身份查看许可证信息 {#view-license-information-as-a-group-administrator}

我们为组管理员创建了一个只读许可证页面，用于查看他们管理的组的许可证计数。

在此更改之前，组管理员无法查看许可证信息。

有关详细信息，请参阅[组管理员](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)。

## 为自动资源计划配置工作角色限制 {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

在自动资源计划设置中，您现在可以为工作角色分配限制。 这样，您就可以用相同的角色控制被分派工作的资源数量。

以前，您无法指定某个工作角色中可以分配工作的用户数量。

有关更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 资源规划者中的项目和角色视图改进 {#project-and-role-view-improvements-in-the-resource-planner}

资源规划者的项目和角色视图现在包含以下改进：

* 改进了从整个数据库提取信息（而不仅仅是屏幕上的信息）的过滤器。
* 全屏模式。
* 性能现在更快、更有效。

   * 可显示的项目、角色和用户数的新限制。
   * 延迟加载，可加快项目和角色的加载。

* 直接从资源规划者快速访问项目和用户。
* 项目视图中更快的拖放功能，可安排项目的优先顺序。

在这些改进之前，您已经报告资源规划者加载缓慢，并且您已经注意到显示的数据中存在不一致的情况。 有了这些改进，这些应该取消。

有关信息并了解资源规划者的新限制，请参阅[资源规划者显示限制](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## 调整项目列表的列宽 {#resize-column-widths-for-project-lists}

由于我们一直在努力改进列表的功能，因此暂时禁用了调整以下项目列表中的列宽的功能：

* 我拥有的项目
* 我在处理的项目
* 所有项目

在此版本中，我们现在可以再次调整所有项目列表中的列的大小。

我们为这项功能添加了其他改进。

现在，当您拖动列的右边框来调整其大小时，右侧的相邻列会保留其大小，从而使列表变宽，而不是同时进行修改。 此外，可以将列的边框拖到相邻列的边框右上方。

在此改进之前，调整大小的列右侧的相邻列也会按比例调整大小以适合屏幕，并且您不能将列的边框拖过相邻列的右边框。  

有关调整列表中列重新排序大小的信息，请参阅[修改列宽和顺序](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)。

要参加我们的测试版测试计划以改进当前列表，请参阅[新列表研究。](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront) （需要登录）

## 图标对新项目列表的支持 {#icon-support-for-the-new-project-lists}

由于我们一直在努力改进列表的功能，因此暂时禁止在以下项目列表中显示状态图标：

* 我拥有的项目
* 我在处理的项目
* 所有项目

在此版本中，状态图标可以再次显示在项目的项目列表中或项目列表中的其他对象中。

有关使用列表的信息，请参阅[Adobe Workfront中的列表入门](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

## 在文档视图中添加大型缩略图字段 {#add-large-thumbnail-field-in-document-views}

我们将向列表或报表中的文档视图中添加一个名为大缩略图的新字段。 在文档视图中选择此字段时，会在列表或报告中显示文档的400像素宽缩略图。

在此更改之前，您只能将“缩略图”字段添加到文档视图，该视图显示文档的宽度为33-66像素的缩略图。

有关列表和报告中的字段的信息，请参阅[Adobe Workfront术语词汇表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## 提高Excel导出限制 {#increase-excel-export-limit}

我们增加了您可以在Excel文件中导出多少行的限制。 您现在可以导出以下内容：

* Excel .xls文件中的65,000行
* Excel .xlsx文件中的100,000行

从Workfront导出以下内容时，将应用这些新限制：

* 来自Web界面的列表或报告
* 使用API的列表或报表
* 已计划和传递的报表

在此改进之前，您只能在任何Excel文件中导出50,000行。

有关从Workfront导出数据的信息，请参阅[导出数据](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 项目列表快速过滤器 {#quick-filters-for-project-lists}

您现在可以将快速过滤器应用于列表。

快速过滤器的用途是帮助您直接导航到大型列表中对您很重要的那些项目，以便您能够快速查看、更新或与他人共享这些项目。

目前，快速筛选器仅适用于以下子选项卡中的项目列表：

* 我在处理的项目
* 我拥有的项目
* 所有项目

有关快速筛选器的信息，请参阅[Adobe Workfront中的列表入门](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)中的“将快速筛选器应用到列表”部分。

## 项目和任务报告中的引用问题集合 {#reference-issue-collections-in-project-and-task-reports}

您现在可以在项目或任务查看和筛选中引用问题集合。 您只能在构建报表时使用文本模式执行此操作。

在此改进之前，您只能在项目视图或筛选器中引用一组任务。

有关如何引用报表中的收藏集的信息，请参阅[引用报表中的收藏集](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)。

有关使用文本模式的信息，请参阅  [文本模式的常见使用概述](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)。

>[!NOTE]
>
>在以下视频中，问题集合的示例文本模式不正确。 报表[&#128279;](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)中的引用收藏集中提供了正确的示例文本模式。

## 在Workfront中添加新文档版本时，新增更强大的版本菜单 {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

现在，向Workfront中的文档添加新版本时，“新版本”菜单包含其他选项，并且现在，在您可以添加新版本的Workfront区域之间保持一致性。

您可以从Workfront的以下区域添加新文档版本：

* 从“文档”选项卡的“更多”下拉菜单中。
* 从文档详细信息页面上的“文档操作”菜单。
* 从文档详细信息页面上的“所有版本”选项卡。

在此更改之前，只有“文档”选项卡中的“更多”下拉菜单包含用于添加新版本的所有选项。

现在，“新版本”菜单中提供了以下选项，可用于所有可添加新版本的区域：

* 校样
* 只是文档
* 链接选项(来自Dropbox、来自Google Drive，等等)
* 从剪贴板粘贴（这是添加版本时的新选项）

有关详细信息，请参阅[将文档从文件系统添加到Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)一文中的[将文档从文件系统添加到Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

## Android Beta移动设备应用程序中的移动设备改进 {#mobile-improvements-in-the-android-beta-mobile-app}

在此版本发布后不久，移动设备应用程序的Android Beta版本将推出以下改进：

* 轻扫操作

  您可以执行各种活动，例如志愿为任务工作、完成任务、将通知标记为“已查看”或“新建”、通过在Workfront移动设备应用程序中滑动各种对象来发送文本或致电联系人。

  此功能对以下方面进行了改进：

   * 我的工作和主页
   * 通知
   * 联系人
   * 审批

* 查看项目的“详细信息”选项卡时的新外观

  在移动设备应用程序的Android Beta版本中查看项目时，界面发生了更改，更便于编辑、填写项目或向项目附加文档。

* 记录时间的新体验

  记录时间比以往更快、更容易，记录时间按钮更易于访问，记录小时数界面更简化。

在此版本中，这些改进仅适用于Workfront移动设备应用程序的Android Beta版本。 它们当前不适用于iOS。

有关如何注册为测试版并下载Android Beta版本的Workfront移动应用程序的更多信息，请参阅。

## 校对查看器增强功能(Workfront和Workfront Proof) {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [已更新打印摘要页](#updated-print-summary-page)
* [直接从验证查看者将用户添加到验证](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [在验证查看器中显示所有标记工具](#display-all-markup-tools-in-the-proofing-viewer)
* [在验证查看器中配置默认排序选项](#configure-default-sorting-options-in-the-proofing-viewer)
* [在桌面验证查看器中查看Workfront文档审批](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [将打开新选项卡和窗口的链接配置为在桌面校对查看器中打开](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* 验证查看器中的[存在指示器](#presence-indicator-in-the-proofing-viewer)
* [筛选注释以在桌面验证查看器中显示交互式URL验证的单个页面](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [静态和视频内容的桌面校对查看器](#desktop-proofing-viewer-for-static-and-video-content)
* [向系统中添加自定义设备](#add-custom-devices-to-your-system)

### 已更新打印摘要页面 {#updated-print-summary-page}

“打印摘要”页面已更新，具有新外观和改进功能。

有关信息，请参阅[在Adobe Workfront中打印校样摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)。

### 直接从验证查看者将用户添加到验证 {#add-users-to-a-proof-directly-from-the-proofing-viewer}

现在，您可以直接从Web验证查看器和桌面验证查看器将用户添加到验证中。 

以前，您无法将个人用户添加到验证中。 您而是只能复制公共URL或嵌入代码。

有关详细信息，请参阅文章中的[通过将用户添加到校对来共享校对](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)  [从验证查看者共享验证](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)。

### 在校对查看器中显示所有标记工具 {#display-all-markup-tools-in-the-proofing-viewer}

现在，可以将标记工具配置为始终显示，而不是显示在必须打开的菜单中。 这使得在工具之间切换的速度更快。 如果以这种方式进行配置，则标记工具水平显示在Web验证查看器和桌面验证查看器的顶部。

以前，标记工具仅在下拉菜单中可用。

有关配置此标记设置的详细信息，请参阅[配置校对查看器设置](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

有关在查看验证时使用标记选项的更多信息，请参阅文章中的。

### 在验证查看器中配置默认排序选项 {#configure-default-sorting-options-in-the-proofing-viewer}

现在，当您更改验证中评论列表中的排序选项时，该选项会在您下次在Web验证查看器或桌面验证查看器中打开任何验证时变成默认排序选项。 

有关更多信息，请参阅文章中的。

### 在桌面验证查看器中查看Workfront文档审批 {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

现在，您可以在桌面验证查看器中作出Workfront文档审批决策。

以前，只有Web验证查看者允许您作出Workfront文档审批决策。 

有关更多信息，请参阅  [在文章的验证查看者中做出校对决定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)  [在校对查看者中做出校对决定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

### 配置打开新选项卡和窗口的链接以在桌面验证查看器中打开 {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

在桌面校对查看器中校对交互式内容时，您现在可以将在新选项卡或新窗口中打开的链接配置为在桌面校对查看器中打开，以便您可以继续校对。

在旧版验证查看器中，无法验证查看器中查看在新选项卡或新窗口中打开的链接。

有关详细信息，请参阅[配置校对查看器设置](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

### 验证查看者中的存在指示器 {#presence-indicator-in-the-proofing-viewer}

现在，在Web验证查看器或桌面验证查看器中查看验证时，您可以查看当前查看验证的每个用户的头像显示在验证查看器的右上角。

有关详细信息，请参阅[与多个审阅人同时审阅校样](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md)。

### 筛选注释以在桌面验证查看器中显示交互式URL验证的单个页面 {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

在桌面验证查看器中查看交互式验证中的URL时，现在可以过滤注释以显示仅在当前页面上所做的注释。 

在此更改之前，此选项仅适用于静态验证。

有关更多信息，请参阅文章中的。

### 用于静态内容和视频内容的桌面校对查看器 {#desktop-proofing-viewer-for-static-and-video-content}

桌面校对查看器现在支持静态和视频内容。

以前，它仅支持交互式内容。

有关配置要在桌面验证查看器中打开的静态和视频验证的信息，请参阅[配置验证查看器设置](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)。

有关桌面校对查看器的详细信息，请参阅[在桌面校对查看器中查看校对。](https://support.workfront.com/hc/en-us/sections/360000686434)

### 向系统中添加自定义设备 {#add-custom-devices-to-your-system}

您现在可以将任何自定义设备添加到系统中，从而允许用户在桌面验证查看器中查看验证时，查看交互式内容并模拟其在特定设备上的显示方式。

在此更改之前，用户只能从预配置的标准设备列表中进行选择。

有关添加自定义设备的信息，请参阅中的

有关用户在查看交互式内容时如何选择设备的信息，请参阅[在验证查看器中更改交互式验证分辨率](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)。

## Workfront中的校对增强功能 {#proofing-enhancements-in-workfront}

* [直接从Workfront共享校对链接](#share-the-proof-link-directly-from-workfront)
* [报告Workfront中的其他校对数据](#report-on-additional-proofing-data-in-workfront)
* [在Workfront中查看验证审批的历史数据](#view-historical-data-for-proof-approvals-in-workfront)

### 直接从Workfront共享验证链接 {#share-the-proof-link-directly-from-workfront}

现在，您可以在Workfront中生成验证链接，并直接从Workfront共享该链接。 或者，您可以复制URL并使用替代方法分发它。

在此更改之前，您只能在Workfront中复制验证链接并使用替代方法分发它。

有关详细信息，请参阅[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)一文中的[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

>[!NOTE]
>
>当前可用的嵌入链接将在未来版本中删除。 嵌入链接仍可通过Workfront API访问。

### 报告Workfront中的其他验证数据 {#report-on-additional-proofing-data-in-workfront}

在包含文档版本对象的报告中（例如文档版本报告和验证审批报告），现在提供了多个字段，允许您查看其他验证信息。

* 校对截止日期

  显示验证截止日期中一周的某天、日期、时间和年份。

* 校对决策

  显示验证的决策状态（待定、需要更改或已批准）。

* 校样名称

  显示校对名称。

* 校样页面

  显示验证中包含的页数。

* 校对进度

  显示验证的进度状态（已发送、已打开、已评论、已决策）。

有关每个字段的更多信息，请参阅  [Adobe Workfront术语词汇表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

### 在Workfront中查看验证审批的历史数据 {#view-historical-data-for-proof-approvals-in-workfront}

在验证审批报告中，您可以添加字段以查看不再有效的验证的验证审批决策。 您可通过将“批准者决策”字段添加到报表来执行此操作。

在此更改之前，在对验证做出决定后，该决定无法再显示在Workfront报表中。

有关更多信息，请参阅  [Adobe Workfront术语词汇表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## Workfront Proof中的校对增强功能 {#proofing-enhancements-in-workfront-proof}

* [直接从验证查看器(Workfront Proof)创建新版本的验证](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [校对查看器和桌面校对查看器中的新校对详细信息链接(Workfront Proof)](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### 直接从验证查看器(Workfront Proof)创建新版本的验证 {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

在Workfront Proof中进行验证时，您现在可以直接从新的验证查看器和桌面验证查看器中创建新版本的验证。

以前，此选项仅在旧版Flash查看器中可用。

有关详细信息，请参阅文章中的[在Workfront Proof中复制校样](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)  [在Workfront Proof中复制校样](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)。

### 校对查看器和桌面校对查看器中的新校对详细信息链接(Workfront Proof) {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

在验证查看器中查看验证时，Workfront Proof用户现在可以快速转到Workfront Proof中的验证详细信息页面。

有关更多信息，请参阅查看校对详细信息。
