---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2Beta决赛
description: 本页介绍了2017.2版的“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年6月28日在预览环境中提供。 该版本将于2017年7月26日在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 0%

---

# 2017.2Beta决赛

本页介绍了2017.2版的“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年6月28日在预览环境中提供。 该版本将于2017年7月26日在生产环境中提供。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.2版中所做所有更改的列表，请参阅[2017.2版活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md)。

2017.2 Beta最终版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**：**

* [确定HTML5视频校对查看器(ProofHQ和Workfront)的可用性](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [支持SAML 2.0的SHA-256证书](#support-sha-256-certificates-for-saml-2-0)
* [提前键入映射属性](#type-ahead-for-mapping-attributes)
* [API增强：访问用户分配](#api-enhancement-access-user-allocations)

所有用户&#x200B;**：**

* [资源规划程序](#resource-planner)
* [项目中的新计划区域（团队生成器）](#new-scheduling-area-in-a-project-team-builder)
* [资源计划：默认显示较少项目](#resource-scheduling-show-fewer-items-by-default)
* [资源计划：拖动任务和问题时显示放置指示器和过度分配](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [资源计划：用户分配不再四舍五入到最接近的半小时](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [以TSV和PDF格式导出利用率报告](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 Beta决赛](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 Beta决赛](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* 我的工作区域(Workfront)中显示[验证决定](#proof-decision-displays-in-the-my-work-area-workfront)
* [以预设分辨率查看富媒体校样(ProofHQ和Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [在富媒体校样(ProofHQ和Workfront)的评论中查看子页面的URL](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [根据现有的标准视图(ProofHQ)创建自定义视图](#create-custom-views-based-on-existing-standard-views-proofhq)
* [筛选报告区域(ProofHQ)](#filter-the-reporting-area-proofhq)
* [在报告(ProofHQ)中显示最小值和最大值](#display-minimum-and-maximum-values-in-reports-proofhq)
* [用于验证审批的应用程序内通知](#in-app-notification-for-proof-approval)
* [移动改进](#mobile-improvements)
* [Slash已添加到包含逗号的字段值的筛选语句中](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [多个记帐费率](#multiple-billing-rates)
* [新资源预算小时字段](#new-resource-budgeted-hour-field)
* [在任务和问题的详细信息页面的“分配给”区域显示用户工作角色](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>在23.1版本中，资源计划工具已弃用并从Workfront中删除。 有关使用工作负载均衡器计划资源的信息，请参阅[工作负载均衡器概述](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)。

## 项目中的新计划区域(Team Builder) {#new-scheduling-area-in-a-project-team-builder}

项目（以前称为Team Builder）中的“计划”区域已使用更新后更直观的用户界面进行了重新设计。 现在，新的计划功能与Workfront其他区域中当前可用的资源计划功能更加匹配。

改进包括：

* 查看项目团队成员的当前资源分配，使您能够在进行分配时做出更明智的决策
* 任务持续时间在计划时间线上的可视化表示形式
* 筛选在计划时间轴上显示的信息
* 直接在时间表上轻松地在项目团队中添加和删除用户

在计划资源时，以下功能在工具的其他区域可用，但在计划团队计划区域中的资源时不可用：

* 配置要在计划时间线上显示的父任务
* 配置要在计划时间线上显示的项目名称
* 使用交换工具修改用户分配
* 按项目组合、项目和项目过滤

有关“团队计划”区域中可用功能的详细信息，请参阅“开始使用资源计划”。

## 资源计划：默认显示更少的物料 {#resource-scheduling-show-fewer-items-by-default}

默认情况下，给定用户的计划时间线中现在每天最多显示10个工作项。 您可以展开列表以查看当前分配给该用户的所有任务和问题。

这样，当用户被分配了许多任务和问题时，您就可以更轻松地浏览计划时间线。

在此更改之前，将始终为所有用户显示所有任务和问题。

有关在计划时间线上将任务和问题分配给用户的更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 资源计划：在拖动任务和问题时显示放置指示器和过度分配 {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

现在，当通过拖放方式将任务或问题分配给计划时间线上的用户时，在释放任务或问题并完成分配之前会显示以下信息：

* 放置指示符显示在用户的行中。 这使您能够在进行分配之前查看在何处分配项目。
* 如果在计划时间线上启用了用户分配，则在完成分配将导致用户过度分配时，将显示红色过度分配指示符。

在这些更改之前，在发布任务或问题之前不显示任何信息。

有关在计划时间线上将任务和问题分配给用户的更多信息，请参阅“在计划区域中手动分配未分配的任务和问题”。

## 资源计划：用户分配不再四舍五入到最接近的半小时 {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

当多个用户被分配到任务或问题，或者任务或问题跨多天时，Workfront会尝试在分配的用户和天数之间平均分配计划小时数。 默认情况下，小时数会四舍五入到最接近的百分之一（例如，1.33）。

以前，当您手动修改分布式小时数时，小时数会进行调整并四舍五入到最接近的半小时（例如，1.33四舍五入到1.5）。

现在，不再调整小时数，并且四舍五入到最接近的半小时（例如，1.33仍为1.33）。

## API增强：访问用户分配 {#api-enhancement-access-user-allocations}

您现在可以通过Workfront API访问用户分配底纹。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## 以TSV和PDF格式导出利用率报告 {#export-the-utilization-report-in-tsv-and-pdf-formats}

除XLSX格式外，您现在还可以以TSV和PDF格式导出项目的利用率报告。

在此更改之前，您只能以XLSX格式导出“利用率”报告。

有关导出利用率报告的详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 验证决策显示在我的工作区域(Workfront)中 {#proof-decision-displays-in-the-my-work-area-workfront}

现在，在“我的工作”区域的“我的审批”选项卡中查看验证审批时，验证决策将显示在“我的工作”区域中，并且一直保留，直到您单击Workfront中的新“刷新”按钮或下次刷新浏览器页面为止。

在此更改之前，没有迹象表明已对验证做出决定，并且在刷新浏览器之前，验证仍保留在“我的审批”选项卡中。

有关详细信息，请参阅[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中的[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。

## 以预设分辨率查看富媒体校对(ProofHQ和Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

在以前的“预览”环境版本中，我们引入了一项功能，即通过指定自定义分辨率或将图像拖动到所需分辨率来调整富媒体验证的分辨率。

您现在可以从各种手机、平板电脑、笔记本电脑和台式机的预设分辨率选项中进行选择。

有关详细信息，请参阅[在验证查看器中更改交互式验证分辨率](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)中的“查看预设分辨率”。

## 查看富媒体校样(ProofHQ和Workfront)评论中的子页面URL {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>此功能当前在生产环境中可用。

现在，当您对富媒体验证中的子页面进行评论时，该子页面的URL会显示在评论中。

在此更改之前，不清楚该评论指的是哪个子页面。

有关更多信息，请参阅

## 确定HTML5视频校对查看器(ProofHQ和Workfront)的可用性 {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

作为ProofHQ中的Workfront管理员，您可以确定贵组织中的用户是否有权访问新的HTML5验证查看器以查看视频验证。

有关在Workfront中配置此选项的更多信息，请参阅中的。

## 基于现有标准视图创建自定义视图(ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

现在，您可以基于标准视图创建自定义视图。 默认情况下，新视图中包含标准视图中的列、排序和筛选器选项。

在此更改之前，要创建自定义视图，您必须从头开始创建视图。 

有关详细信息，请参阅[在Workfront Proof Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)中创建和管理自定义视图[中创建自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating)。

## 筛选报告区域(ProofHQ) {#filter-the-reporting-area-proofhq}

默认情况下，“报告”选项卡上显示的数据包含来自ProofHQ系统的所有信息。 您现在可以使用过滤器仅显示与您的需求相关的信息。 

有关详细信息，请参阅[过滤报表](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports)，位于  [在Workfront Proof中运行报告](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md)。

## 在报告中显示最小值和最大值(ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

您现在可以配置在查看报表时是否在图形中显示最小值和最大值。

有关详细信息，请参阅中的[查看报表](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports)  [在Workfront Proof中运行报告](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md)。

## 支持SAML 2.0的SHA-256证书 {#support-sha-256-certificates-for-saml-2-0}

在使用SAML 2.0为Workfront配置SSO时，我们现在支持安全哈希算法256 (SHA-256)。在此版本之前，我们仅支持安全哈希算法1 (SHA-1)。

有关使用SAML 2.0配置Workfront的更多信息，请参阅[使用SAML 2.0配置Adobe Workfront](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## 预输入映射属性 {#type-ahead-for-mapping-attributes}

“属性映射”对话框中的“默认值”字段类型已更新为预先输入字段。 在此更改之前，默认值字段的类型是下拉列表。

此更改适用于以下SSO协议：

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1不支持属性映射。

## 移动改进 {#mobile-improvements}

>[!NOTE]
>
> 移动设备应用程序独立于主Workfront应用程序进行发布。 此部分描述的功能将于8月初发布。

您将看到在移动应用程序上为Android和iOS平台添加了以下功能：

* 从移动设备应用程序提交请求
* 移动应用程序上的工时表新条目
* 从移动应用程序编辑自定义表单
* 移动应用程序上的验证审批请求

Android平台的其中一些功能将有一个公开测试版计划。

有关即将推出的移动设备测试版计划的更多信息，请参阅  [“Betas”](https://support.workfront.com/hc/en-us/sections/115000743248)页。

有关使用Workfront移动设备应用程序的更多信息，请参阅。  

## 为包含逗号的字段值的筛选语句添加了斜杠 {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

在文本模式下构建过滤器并筛选包含逗号的字段值时，必须在分隔值的逗号之前添加斜杠(“/”)，以确保将该值作为一个过滤器选项读取。 这仅适用于以下字段类型：

* 下拉列表
* 单选按钮
* 复选框

在此更改之前，您无法筛选选项中包含逗号的字段。

有关此更改的详细信息，请参阅[筛选器概述](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

## 多个记帐费率 {#multiple-billing-rates}

您现在可以在项目级别为同一工作角色添加多个记帐费率覆盖。 利用这项新功能，您可以为每个记帐费率覆盖定义日期范围。 在指定的日期范围内，对分配给项目任务的工作角色应用不同的记帐费率。 记帐费率乘以项目的小时数来计算收入。 在计费费率的日期范围内计算的收入仍以该费率锁定，并且不会作为项目更新时工作角色的费率进行更新。 在实际收入中，覆盖记帐费率之前记录的小时数将不会重新计算以反映当前记帐费率。 将记帐费率覆盖添加到项目之前记录的小时数将与当时工作角色的记帐费率关联。

在此更改之前，您只能覆盖工作角色的记帐费率一次，并且实际收入将重新计算以反映在记帐费率更改之前记录的所有小时的当前记帐费率。

有关记帐费率和收入的更多信息，请参阅[记帐和收入概览](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)。

有关在项目级别覆盖工作角色的记帐费率的详细信息，请参阅[有关覆盖工作角色记帐费率和计算项目收入的概述](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

## 资源规划程序 {#resource-planner}

在此版本中，我们将介绍资源规划者的第一阶段，它是人员区域中新“规划”选项卡重新设计的一部分。 通过使用资源规划者，您可以预算您的资源池中的用户在您是其资源管理员的所有当前项目中分配的小时数。 您可以在资源计划程序中按项目、工作角色和用户查看以下分配编号：

* 可用小时数
* 规划小时数
* 预算小时
* 小时差异（预算和计划小时数之间）
* 净小时差异（可用小时数和预算小时数之间）

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 新资源预算小时数字段 {#new-resource-budgeted-hour-field}

为了支持新的计划功能和资源规划者，已在Report Builder中添加了一个新字段，用于报告资源预算小时数。 此字段捕获在项目中为资源预算的小时数。 在使用旧版资源计划功能对资源进行预算时，此字段不可用。

有关在资源规划者中使用预算小时数的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 用于验证审批的应用程序内通知 {#in-app-notification-for-proof-approval}

当您被指定为校样的审批者时，您将收到有关等待您决策的校样审批的应用程序内通知。 通知显示以下文本：`<User name>`希望您批准此校对”。 如果用户信息不可用，通知将更改为“此验证需要您的审批”。

在此增强功能之前，您被指定为验证审批者的唯一视觉指示是“我的工作”区域中的新验证请求。

有关应用程序内通知的详细信息，请参阅[查看和管理应用程序内通知](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)。

## 在任务和问题的详细信息页面的“分配给”区域显示用户工作角色 {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

现在，查看任务或问题的详细信息页面时，工作角色显示在任务接受者姓名下方的“分配给”区域中。 此工作角色表示与任务或问题的工作角色分配匹配的用户的工作角色。 如果任务或问题未分配给工作角色，则会显示已分配用户的主要工作角色。

在此更改之前，仅用户标题显示在分配给区域的用户名下方。 
