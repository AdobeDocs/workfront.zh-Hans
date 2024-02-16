---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 5发布活动
description: 本页介绍了2018.3 Beta 5版本预览环境中最近提供的所有更改。 该功能将于2018年9月21日在预览环境中可用。 该版本将于2018年11月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f208b566-2529-4c4d-aa66-0c8756e55a5a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 0%

---

# 2018.3 Beta 5发布活动

本页介绍了2018.3 Beta 5版本预览环境中最近提供的所有更改。 该功能将于2018年9月21日在预览环境中可用。 该版本将于2018年11月在生产环境中提供。

有关2018.3版中所做所有更改的列表，请参阅  [2018.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

2018.3测试版5包含面向所有用户的增强功能：

* [跟踪您在主页区域提交的审批](#track-approvals-you-ve-submitted-in-the-home-area)
* [Workfront中基于Flash的工具的替换](#replacement-of-flash-based-tools-in-workfront)
* [允许工作许可证用户访问项目的“计划”子选项卡](#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project)
* [改进了资源规划者中的筛选器](#improved-filters-in-the-resource-planner)
* [在资源规划者中查看实际小时数](#view-actual-hours-in-the-resource-planner)
* [业务案例导出中的资源规划者数据](#resource-planner-data-in-the-business-case-export)
* [启用公司级别记帐费率覆盖](#enable-company-level-billing-rate-override)
* [简化的基于角色的批准](#simplified-role-based-approvals)
* [利用率报表：从新资源预算区域填充预算小时数](#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area)
* [利用率报表：按用户在项目上查看预算小时数](#utilization-report-view-budgeted-hours-by-user-on-a-project)
* [验证查看器中不再支持SWF文件](#swf-files-no-longer-supported-in-the-proofing-viewer)
* [在验证查看器的评论列表中更快速地访问操作](#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer)
* [验证查看者中的验证共享改进](#proof-sharing-improvement-in-the-proofing-viewer)
* [验证查看者中的注释列表增强功能](#comments-list-enhancements-in-the-proofing-viewer)
* [在校对查看器中缩放和平移视频校对](#zoom-and-pan-video-proofs-in-the-proofing-viewer)
* [验证查看器中的背景变亮](#lighter-background-in-the-proofing-viewer)
* [在校对查看器中编辑评论时提高可见性](#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer)
* [在验证查看器的注释列表中查看与操作关联的注释数](#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer)
* [在验证查看器中指定将用户添加到验证时的阶段](#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer)
* [从交互式或静态网站验证打开关联的网站](#opening-the-associated-website-from-an-interactive-or-static-website-proof)
* [打印摘要增强功能](#print-summary-enhancements)
* [缩短了校对加载时间](#improved-proof-loading-time)
* [Workfront移动设备应用程序中“更新”选项卡的新外观](#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app)

## 跟踪您在主页区域提交的审批 {#track-approvals-you-ve-submitted-in-the-home-area}

您现在可以使用“主页”区域与已提交给其他用户的审批进行交互。

从主页，您可以：

* 撤回批准
* 提醒用户审批
* 将用户添加到文档审批
* 查看验证审批

  以前，您只能在“我的工作”区域与已提交的审批交互。 

有关更多信息，请参阅 [管理审批](../../../../review-and-approve-work/manage-approvals/manage-approvals.md). 

## Workfront中基于Flash的工具的替换 {#replacement-of-flash-based-tools-in-workfront}

计划在2018.3版本中从Workfront删除所有依赖于Flash技术的功能，这些功能将被新的解决方案取代。

有关受移除这些功能影响的所有区域以及了解哪些工具将替换这些功能的更多信息，请参阅 [Adobe Workfront中基于Flash的工具的替换](../../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

## 允许工作许可证用户访问项目的“计划”子选项卡 {#allowing-work-license-users-to-access-the-scheduling-subtab-of-a-project}

拥有工作许可证的用户现在可以访问项目的“计划”子选项卡，位于“人员配备”选项卡下。

在此增强功能之前，只有拥有计划许可证的用户才能访问此子选项卡。

有关访问项目的“计划”子选项卡所需的访问权限的信息，请参阅“开始使用资源计划”。

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器调度资源的信息，请参阅 [工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## 改进了资源规划者中的筛选器 {#improved-filters-in-the-resource-planner}

您现在可以在资源规划者中过滤信息以包括特定于项目和用户字段，包括自定义字段。

在此改进之前，您只能在资源规划者中筛选有限数量的内置字段和标准。

有关在资源规划者中过滤信息的信息，请参阅 [资源规划者中的筛选信息](../../../../resource-mgmt/resource-planning/filter-resource-planner.md).

## 在资源规划者中查看实际小时数 {#view-actual-hours-in-the-resource-planner}

您可以在资源规划者的用户视图中查看实际小时数。

在此改进之前，实际小时数在资源规划者中不可见。

有关在资源规划者中查看小时数信息的信息，请参阅 [资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## 业务案例导出中的资源规划者数据 {#resource-planner-data-in-the-business-case-export}

在将业务案例导出到PDF时，导出文件中的财务信息现在反映了“资源预算”区域和资源规划者中的信息。 

以前，导出的文件反映旧版资源估算区域和Capacity Planner中的信息。 

有关导出业务案例的信息，请参见 [为项目创建业务案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md) 中的部分 [为项目创建业务案例](../../../../manage-work/projects/define-a-business-case/create-business-case.md).

## 启用公司级别记帐费率覆盖 {#enable-company-level-billing-rate-override}

您现在可以启用一个选项，以允许公司级别的记帐费率覆盖项目级别的记帐费率。 在公司级别更新记帐费率后，您可以手动重新计算项目财务以反映这些更改。

如果启用此设置，则公司级别的记帐费率将覆盖项目上的历史工作角色费率。

以前，除非从项目中删除公司，然后重新附加公司，否则无法将公司级别的记帐费率更改应用于项目。

有关更多信息，请参阅 [用公司级别的记帐费率覆盖项目级别的记帐费率](../../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md). 

## 简化的基于角色的批准 {#simplified-role-based-approvals}

现在，基于角色的批准可更简单地用于项目。 现在，必须将用户分配给项目团队并在其用户配置文件中分配角色，才能看到分配给其主要或次要角色的批准。

以前，您必须将用户分配给项目团队，确保他们在用户配置文件中具有正确的角色，并在旧版团队生成器中选择该角色。

有关更多信息，请参阅部分 [项目团队概述](../../../../manage-work/projects/planning-a-project/project-team-overview.md) 在文章中 [项目团队概述](../../../../manage-work/projects/planning-a-project/project-team-overview.md).

## 利用率报表：从新资源预算区域填充预算小时数 {#utilization-report-populates-budgeted-hours-from-new-resource-budgeting-area}

>[!NOTE]
>
> 此功能首次引入到2018.2版本的预览环境中。 它将在2018.3版本中发布到生产环境。 

利用率报表中的预算小时数现在由业务案例的新资源预算编制区域中的可用信息填充。

在此更改之前，使用旧版资源估算区域中的信息。

有关更多信息，请参阅  [资源利用率报表概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) 在文章中  [资源利用率报表概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 利用率报表：按用户在项目上查看预算小时数 {#utilization-report-view-budgeted-hours-by-user-on-a-project}

>[!NOTE]
>
>此功能首次引入到2018.2版本的预览环境中。 它将在2018.3版本中发布到生产环境。 

项目的利用率报告现在按用户显示预算小时数。

在此更改之前，“利用率”报告仅按工作角色显示预算小时数。 

有关更多信息，请参阅  [资源利用率报表概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) 在文章中  [资源利用率报表概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## 验证查看器中不再支持SWF文件 {#swf-files-no-longer-supported-in-the-proofing-viewer}

由于与AdobeFlash相关的安全问题，验证查看器不再支持从SWF文件创建的验证。 如果您打开之前为SWF文件创建的校样，则会显示一条消息，其中校样内容先前显示在校样查看器中。 您可以看到对验证的任何评论。 您还可以下载注释和下载原始SWF文件。

有关更多信息，请参阅 [支持的校对文件类型和大小限制概述](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) 在文章中 [支持的校对文件类型和大小限制概述](../../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md). 

## 在验证查看器的评论列表中更快速地访问操作 {#actions-more-quickly-accessible-in-the-comment-list-in-the-proofing-viewer}

您现在可以更快速地添加或更改验证查看器中评论的操作。 只需单击任意评论上的“更多”图标，然后在下拉菜单中单击所需的操作即可。

以前，您必须打开评论，打开下拉菜单，打开子菜单，然后单击所需的操作。

有关更多信息，请参阅 [对验证评论使用操作](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

## 验证查看者中的验证共享改进 {#proof-sharing-improvement-in-the-proofing-viewer}

现在，当您从验证查看器发送URL时，显示的选项的组织方式与您在文档区域共享URL时看到的选项完全相同。

以前，这些选项提供的功能与现在相同，但其组织方式与“文档”列表中的相应选项不一致。

有关更多信息，请参阅部分  [共享URL](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-the-url) 在文章中  [从验证查看者共享验证](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 验证查看者中的注释列表增强功能 {#comments-list-enhancements-in-the-proofing-viewer}

“注释”列表中现在提供了以下改进功能：

* 现在，评论文本后面会显示浅灰色背景，以便使其与“评论”面板中显示的其它文本明显不同，例如审阅者姓名、审阅时间和验证页码。 这样，当您只想阅读校对反馈时，便可更轻松地阅读校对反馈。

  以前，“评论”面板的整个背景为白色。

  有关更多信息，请参阅。

* 对评论的回复现在缩进到评论下。 这样可以更轻松地区分回复与上面的原始评论。

  以前，评论下的回复与评论左对齐。

  有关更多信息，请参阅中的。

* 在验证查看器中解析注释时，绿色的“已解析”复选标记图标会出现，且注释的右上角没有任何文本。 这使“评论”面板的外观更加清晰，更容易扫描您所需的信息。

  以前，已解决的复选标记图标出现在注释左上角的“已解决”一词旁边 

  有关更多信息，请参阅中的。

## 在校对查看器中缩放和平移视频校对 {#zoom-and-pan-video-proofs-in-the-proofing-viewer}

现在，您可以放大视频校样，并平移到需要更仔细检查的校样区域。

## 验证查看器中的背景变亮 {#lighter-background-in-the-proofing-viewer}

验证查看器中的背景现在稍微变亮了一些。 此更改使区分包含黑色背景和边缘的校对内容变得更容易。

以前，验证查看器背景为黑色。

## 在校对查看器中编辑评论时提高可见性 {#better-visibility-when-a-comment-has-been-edited-in-the-proofing-viewer}

“已编辑”标签现在显示在审阅人更改的任何评论上。 当您将鼠标悬停在此上时，将显示审阅者的名称和更改日期。

## 在验证查看器的注释列表中查看与操作关联的注释数 {#view-the-number-of-comments-associated-with-an-action-in-the-comment-list-in-the-proofing-viewer}

单击“注释”列表中的“过滤器”图标后，您现在可以看到与每个操作关联的注释数量。

仅当为您的组织启用了操作时，“评论”列表中才有这些操作。

## 在验证查看器中指定将用户添加到验证时的阶段 {#specify-the-stage-when-adding-users-to-a-proof-in-the-proofing-viewer}

当您将审阅者添加到在验证查看者中具有自动工作流的验证时，您可以指定希望审阅者处理验证的阶段。 这类似于将用户添加到验证查看者以外的验证时可用的功能。

以前，当您将审阅者添加到验证查看者中的验证时，Workfront会将他们放在当前处于活动状态的阶段中。

有关更多信息，请参阅 [通过添加用户来共享验证](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) 在 [从验证查看者共享验证](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## 从交互式或静态网站验证打开关联的网站 {#opening-the-associated-website-from-an-interactive-or-static-website-proof}

在查看包含交互式或静态Web内容的验证时，您现在可以单击按钮以在验证查看器的新浏览器选项卡中轻松打开关联的网站。 这样，您就可以使用两个不同的选项卡，将您在验证中看到的内容与实际网站进行比较。

以前，您可以将鼠标悬停在URL上并单击工具提示来打开关联的网站。 此方法易于访问且直观。

## 打印摘要增强功能 {#print-summary-enhancements}

“打印摘要”页面现在提供以下改进功能：

* 现在，您可以指定是要在验证中包含所有页面，还是仅包含包含评论的页面。

  以前，只能包含包含注释的页面。

* 如果验证具有阶段，则现在您可以包含一个图表，其中显示验证阶段的顺序以及针对每个阶段作出的决策。

  以前，此图表不可用。

* 现在，当多个标记与一个注释相关联时，该注释的编号将显示在“打印摘要”页面上的每个标记上。

  以前，评论编号只出现在与评论关联的第一标记上。 评论的其他标记显示时没有数字。

* 如果验证是Web捕获，则任何包含注释的页面都会显示捕获网页时的分辨率。 例如，如果验证包含为移动设备捕获的页面以及为笔记本电脑和台式机捕获的相同页面，则此功能非常有用。
* 现在，当您按“操作”、“创作”或“未解决”状态筛选“打印摘要”页面中的注释时，您的筛选器适用于导出为PDF或Excel文件的校样，而不仅仅是打印的校样。

有关更多信息，请参阅 [在Adobe Workfront中打印验证摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## 缩短了校对加载时间 {#improved-proof-loading-time}

我们进行了一些性能改进，这应会缩短打开验证时的加载时间。

有关打开验证的信息，请参阅。

## Workfront移动设备应用程序中“更新”选项卡的新外观 {#new-look-and-feel-of-the-updates-tab-in-the-workfront-mobile-app}

移动应用程序上“更新”选项卡的外观现已更新。 目前，这项改进仅在Android的Workfront Beta版应用程序中可用。

有关在Workfront移动设备应用程序中管理更新和评论的信息，请参阅中的部分。
