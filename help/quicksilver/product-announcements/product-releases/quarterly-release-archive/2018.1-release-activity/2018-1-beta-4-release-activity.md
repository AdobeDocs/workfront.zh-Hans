---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 4发行版活动
description: 本页介绍了2018.1 Beta 4版本在“预览”环境中最近提供的所有更改。 2018年1月24日，该功能在“预览”环境中提供。 该版本将于2018年3月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# 2018.1 Beta 4发行版活动

本页介绍了2018.1 Beta 4版本在“预览”环境中最近提供的所有更改。 2018年1月24日，该功能在“预览”环境中提供。 该版本将于2018年3月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.1版中所做所有更改的列表，请参阅  [2018.1版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 4版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [由组管理员管理的计划](#schedules-managed-by-group-administrators)

所有用户&#x200B;****

* Workfront中的[验证改进](#proofing-improvements-within-workfront)
* 在Workfront Proof中创建[验证 — 改进了用户体验和其他功能](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* Workfront和Workfront Proof中的[校对改进](#proofing-improvements-within-workfront-and-workfront-proof)
* [Workfront Proof中的Basecamp集成更新了外观](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [将图片从剪贴板粘贴到Workfront](#paste-images-to-workfront-from-the-clipboard)
* [利用率报告改进](#utilization-report-improvements)
* [从Workfront中删除资源预算小时对象](#remove-the-resource-budgeted-hour-object-from-workfront)
* [报告使用情况统计数据](#report-usage-statistics)
* [甘特图更新](#gantt-chart-updates)
* [新Portfolio优化器](#new-portfolio-optimizer)
* 资源规划者中的[预算日期调整选项](#budget-date-adjustment-option-in-the-resource-planner)
* [资源计划：根据组成员资格限制分配给用户](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [资源计划：允许分配给用户，而不管角色是什么](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Emoji支持](#emoji-support)

## Workfront中的验证改进 {#proofing-improvements-within-workfront}

对Workfront中的文档列表进行了以下改进： 

* [从文档列表查看校对进度](#view-proof-progress-from-the-document-list)
* [从文档列表查看打印摘要的新选项](#new-option-to-view-the-print-summary-from-the-document-list)
* [更新了从文档列表生成或打开验证的外观](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [从文档列表上的文档中删除的各种链接](#various-links-removed-from-documents-on-the-document-list)
* [查看组合验证的文件名](#view-file-names-on-combined-proofs)
* [从文档列表查看验证的当前活动阶段](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### 从文档列表查看验证进度 {#view-proof-progress-from-the-document-list}

现在，查看文档列表时，将为所有验证显示验证进度指示器。 （包括已发送、已打开、已作出评论和已作出决定。）

在此更改之前，您必须在文档列表中选择验证以在右侧面板中查看验证进度。 

有关详细信息，请参阅[校对进度和状态概述](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md)。

### 从文档列表查看打印摘要的新选项 {#new-option-to-view-the-print-summary-from-the-document-list}

您现在可以直接从文档列表查看校样的打印摘要。

在此更改之前，您只能从校对查看器中查看打印摘要。 

有关从文档列表查看打印摘要的详细信息，请参阅[在Adobe Workfront中打印校对摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)。

### 更新了从文档列表生成或打开验证的外观 {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

现在，当鼠标悬停在文档列表中的文档上时，用于生成验证或打开验证的选项已更新。 这些选项现在更加突出，并显示为按钮。

在此更改之前，这些选项可用作文档名称下方的链接。

有关更多信息，请参阅以下部分：

* 。
* 中的。

### 从文档列表上的文档中删除的各种链接 {#various-links-removed-from-documents-on-the-document-list}

以下操作不再作为文档列表中各个文档的链接提供：

* 生成校样
* 校样
* 详细信息
* 共享
* 签出/签入

以下操作现在可作为文档列表内的文档按钮使用：

* 打开验证（在生成验证后可用） 
* 生成校对（在尚未生成校对时可用）

现在，在打开验证或生成验证按钮旁边的下拉菜单中可使用以下操作：

* 校样详细信息
* 文档详细信息
* 打印摘要

有关更多信息，请参阅以下部分：

* 。
* 中的。

### 查看组合验证的文件名 {#view-file-names-on-combined-proofs}

现在，您可以查看组成组合验证的各个文件名。 在文档列表中选择验证时，此信息显示在“详细信息”选项卡中。

有关更多信息，请参阅查看组合验证中包含的所有文件。 

### 从文档列表查看验证的当前活动阶段 {#view-the-current-active-stage-of-a-proof-from-the-document-list}

现在，在文档列表中选择验证时，当前活动阶段显示在详细信息选项卡的右列。 

有关详细信息，请参阅[在校对上查看活动阶段](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md)。  

## 在Workfront Proof中创建验证 — 改进了用户体验和其他功能 {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

除了在Workfront Proof中创建验证时改进的用户体验之外，现在还提供以下附加功能：

* 将多个图像合并到单个验证中。
* 多个分辨率的验证网站（多个分辨率可以作为单个验证创建，或者可以组合到单个验证中）。
* 在上载过程中编辑文件名。
* 在验证创建表单中包含自定义字段。
* 添加自定义消息以验证电子邮件通知。
* 其他校对设置 
* 验证URL时的实时错误验证（以前，显示错误之前必须等待几分钟）

>[!NOTE]
>
>Workfront Proof中的这个新验证创建页面现在与最近在Workfront中创建验证时提供的验证创建页面匹配。 

有关更多信息，请参阅  [在Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证。

## Workfront和Workfront Proof中的验证改进 {#proofing-improvements-within-workfront-and-workfront-proof}

将文档添加到Workfront和Workfront Proof时，以下更改适用：

* [查看验证时调整评论列表大小](#resize-the-comment-list-when-reviewing-proofs)
* 审阅静态校样时，[超链接处于活动状态](#hyperlinks-are-active-when-reviewing-static-proofs)
* [添加验证时的改进](#improvements-when-adding-proofs)

### 查看验证时调整评论列表大小 {#resize-the-comment-list-when-reviewing-proofs}

现在，您可以在验证查看器中查看验证时调整评论列表的大小。

有关更多信息，请参阅中的。

### 查看静态验证时，超链接处于活动状态 {#hyperlinks-are-active-when-reviewing-static-proofs}

现在，查看验证查看者中的静态验证时，超链接处于活动状态。 单击超链接可转到链接的页面。

任何包含文本的文件类型(如PDF、DOC等)都支持此功能。 不支持图像文件。

### 添加验证时的改进 {#improvements-when-adding-proofs}

在添加要校对的文档时，可以使用以下增强功能。 

* 收件人列表中的信息现在以3列视图的形式提供，使得该信息更易于查看和修改。 

  以前，信息以单列视图显示，当需要进行更改时，需要多次单击。 

  有关更多信息，请参阅中的。

* 使用自动工作流时，将一个或多个收件人从一个工作流阶段拖到另一个工作流阶段。 您可以直接拖动到舞台，也可以拖动到位于页面顶部的图表上的舞台。

  有关更多信息，请参阅中的。

* 即使在滚动时，工作流程图表在页面顶部仍然可见。 默认情况下，该图处于折叠状态；展开该图以查看完整图。

  有关更多信息，请参阅中的。

* 将模板添加到验证中的自动工作流时，会显示加载动画，指示正在加载模板。

  有关更多信息，请参阅中的。

* 以下设置已从“校对设置”部分移至“新校对”页面上的“工作流”部分：

   * 主要决策者
   * 只需要一个决策

## 通过Workfront Proof中的Basecamp集成更新了外观 {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Basecamp与Workfront Proof集成的外观现已更新。 功能保持不变。

## 将图片从剪贴板粘贴到Workfront {#paste-images-to-workfront-from-the-clipboard}

您现在可以通过从系统剪贴板粘贴图像来将图像文件添加到Workfront。

从剪贴板粘贴的功能已在以前的版本中从Workfront中删除；此版本正在重新引入此功能。 新方法更加简洁直观。

有关详细信息，请参阅[从剪贴板粘贴图像](../../../../documents/managing-documents/paste-image-clipboard.md)。 

## 利用率报告改进 {#utilization-report-improvements}

“Utilization”报告包含以下改进：

* 在项目的利用率报告中查看收入

  用于查看预算收入、计划收入、实际收入、预算差异和计划差异。

* 将收入与计划成本和实际成本进行比较

  允许您查看计划或实际成本以及计划收入。 系统还会显示毛利(%)（毛利的计算方法为收入 — 成本/收入）。

* 查看图表时会显示收入。
* 滚动时，标题保持可见。

  现在，滚动利用率报告中的信息时，利用率报告顶部的标题始终可见，这使您能够更轻松地了解报告中的数据。

  以前，在滚动时，利用率报告顶部的标题将移出视图。

* 单个项目的利用率报告会自动加载

  查看项目的利用率报告时，报告会自动加载。

  在此更改之前，您必须在报表运行之前单击“运行”。

* 改进的性能

有关利用率报告的详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 从Workfront中删除资源预算小时对象 {#remove-the-resource-budgeted-hour-object-from-workfront}

为了解决性能问题，已从Workfront中临时删除资源预算小时数字段。

提醒一下，资源预算小时数是您在资源规划者中为资源或项目预算的小时数。 目前，您无法再在Web应用程序中或通过API报告此字段。 当性能问题得到解决后，该字段将在未来版本中恢复。

有关资源规划者中预算小时数的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。 

## 报告使用情况统计数据 {#report-usage-statistics}

现在，您可以在报表列表中显示Workfront报表的以下使用情况信息：

* 上次查看者
* 上次查看日期
* 最近 10 个查看者
* 本月/季度/年查看次数
* 查看上个月/季度/年
* 所有视图

在此更新之前，您在报表中看到的使用信息有限。

有关报告使用情况的详细信息，请参阅[查看报告使用情况](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## 由组管理员管理的计划 {#schedules-managed-by-group-administrators}

作为组管理员，您可以创建和编辑与所管理组及其子组相关联的计划。 在此更改之前，只有Workfront管理员才能创建和编辑计划。

有关管理计划的详细信息，请参阅[创建计划](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## 甘特图更新 {#gantt-chart-updates}

甘特图现在可编辑。 使用甘特图，您可以对任务进行以下更新：

* 创建前置任务关系
* 编辑任务持续时间
* 更新任务完成百分比
* 应用资源均衡

在此更改之前，您只能在甘特图中删除前置任务关系，并且只能在任务列表中编辑任务。

有关甘特图的详细信息，请参阅任务列表甘特图中的[更新信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## 新的Portfolio优化器 {#new-portfolio-optimizer}

Workfront的Portfolio优化器区域现在更新了新外观。 功能没有改变。

有关Portfolio优化程序的详细信息，请参阅[Portfolio优化程序概述](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## 资源规划者中的预算日期调整选项 {#budget-date-adjustment-option-in-the-resource-planner}

我们新增了一个选项，可让您快速查看时间范围，而不会出现预算冲突。 查看时间范围发生无预算冲突的时间范围后，您可以手动将预算小时数移动到这些时间。 这还将调整小时的预算日期。 在此更新之前，无法一览项目的预算冲突。

有关资源规划者中调整预算日期的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的“调整预算日期”部分

## 资源计划：根据组成员资格限制分配给用户 {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

在“计划”区域中进行用户分配（如“在计划区域中手动分配未分配的任务和问题”中所述）时，您现在可以配置Workfront，以仅将任务和问题的分配限制为那些属于在任务或问题源自的项目上定义的组的成员的用户。 

这适用于以下列方式分配工作：

* 将用户分配给特定角色的所有任务和问题时，如“在计划区域中手动分配未分配的任务和问题”中所述。

  在此更改之前，任务或问题始终可以分配给任何用户，而不管该用户的组成员资格如何。 

* 与其他用户交换分配时，如“在计划区域中手动分配未分配任务和问题”中所述。

  在此更改之前，任务或问题始终可以分配给任何用户，而不管该用户的组成员资格如何。 

* 从计划时间线手动分配任务或问题时，如“在计划区域中手动分配未分配的任务和问题”中所述。

  在此更改之前，任务或问题始终可以分配给任何用户，而不管该用户的组成员资格如何。 

* 当允许Workfront自动分配用户时，如“在计划区域中手动分配未分配的任务和问题”中所述。

  在此更改之前，无论组成员身份如何，Workfront都会向用户分配任务和问题。

有关配置此选项的更多信息，请参阅“开始使用资源计划”。

## 资源计划：允许分配给用户，而不管角色如何 {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

在计划区域中进行用户分配时（如“在计划区域中手动分配未分配的任务和问题”中所述），您现在可以将Workfront配置为允许将任务和问题分配给任何用户，无论该用户的用户配置文件中定义的角色是否与分配给他们的任务或问题的角色分配相匹配。

这适用于以下列方式分配工作：

* 将用户分配给特定角色的所有任务和问题时，如“在计划区域中手动分配未分配任务和问题”中的“在计划区域中手动分配未分配任务和问题”中所述。

  在此更改之前，要分配的用户的主要角色必须与选择角色字段中已定义的角色匹配。

* 与其他用户交换分配时，如“在计划区域中手动分配未分配任务和问题”中所述。

  在此更改之前，要分配的用户的主要角色必须与选择角色字段中已定义的角色匹配。

* 从计划时间线手动分配任务或问题时，如“在计划区域中手动分配未分配的任务和问题”中所述。

  在此更改之前，只有其角色与您分配的任务或问题的角色相匹配的用户才会显示在计划时间线上。

>[!NOTE]
>
>当允许Workfront自动分配用户时，这不适用，如“在计划区域中手动分配未分配的任务和问题”中所述。 在自动分配用户时，只能将任务和问题分配给具有匹配角色的用户。

有关配置此选项的更多信息，请参阅“开始使用资源计划”。

## Emoji支持 {#emoji-support}

现在，您可以通过插入表情符号来为Workfront中的注释和更新设置基调。 在“更新”选项卡上发表的评论中添加的任何表情符号也会显示在更新电子邮件通知中。 

有关详细信息，请参阅[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。
