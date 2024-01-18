---
content-type: release-notes
navigation-topic: product-releases
title: 20.4版本概述
description: 20.4版本在2020年11月9日当周的生产环境中提供。 有关每个群集的特定发行日期和时间，请参阅Workfront状态站点。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7cf7f6ed-fe85-4c86-bb4b-dd93197338cf
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3694'
ht-degree: 0%

---

# 20.4版本概述

20.4版本在2020年11月9日当周的生产环境中提供。

本页介绍了Adobe Workfront Classic的功能以及20.4版本中包含的新Adobe Workfront Experience。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 20.4 release nears its planned Production release, this page will be updated with all functionality included with 20.4.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of November 9, 2020. For specific release dates and times for each cluster, see the <a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>. </p>
-->

## Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [资源管理增强功能](#resource-management-enhancements)
* [项目管理增强功能](#project-management-enhancements)
* [增强的分析](#enhanced-analytics)
* [校对增强功能](#proofing-enhancements)
* [移动和集成增强功能](#mobile-and-integration-enhancements)
* [其他增强功能](#other-enhancements)

### 管理员增强功能 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">管理员的新增功能：控制自定义字段的共享方式</a> </p> <p>为了让您更好地控制谁可以编辑、删除和使用您创建的自定义字段，我们添加了准确配置您希望如何共享这些字段的功能。</p> <p>此前，当您创建自定义字段时，系统中的每个人都可以编辑它。 这仍然是自定义字段的默认状态，但现在您可以将自定义字段共享限制为仅共享某些用户、角色、团队、组和公司。 并且您可以确定收件人是否可以管理或仅查看自定义字段。</p> <p>此外，为了让您熟悉这种体验，我们设计了用户界面，以便该功能与在Workfront中共享的其他对象区域类似。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">管理员的新增功能：标准化的自定义表单共享</a> </p> <p>我们为自定义Forms实现了标准化共享，以便您可以使用已知的Workfront对象共享流程。 新的共享体验使您能够更好地控制谁可以编辑、删除和使用您创建的自定义Forms。 您可以将自定义表单的共享限制为某些用户、角色、团队、组和公司。 您还可以确定这些收件人是否可以查看或管理自定义表单。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">管理员的新增功能：切换Workfront环境选项可用</a> </p> <p>为了获得更高效且更便捷的体验，组管理员和Workfront管理员现在可以从Workfront中的任何页面快速在不同的Workfront环境之间切换，而无需注销。</p> <p>在新的Workfront Experience中，主菜单中会显示切换到经典选项。</p> <p>在Workfront Classic中，切换到新体验选项显示在单击全局导航栏右上角的配置文件图片时显示的菜单中。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">管理员的新增功能：分配给公司的组的管理员可以管理公司</a> </p> <p>我们让组管理员可以轻松管理在Workfront中与其组关联的公司。 建立关联后，将自动提供管理公司的权限。 当组管理员对公司没有管理权限时，这一点尤其重要。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">管理员的新增功能：电子邮件通知增强功能</a> </p> <p>现在，只需单击一下，即可在“设置”中启用或禁用事件电子邮件通知。 只需单击通知名称旁边的打开/关闭开关。</p> <p>此外，请注意我们的现代样式现在改进了电子邮件通知区域中配置事件通知的体验。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">管理员的新增功能：将项目组合、项目和公司与组关联</a> </p> <p>当Workfront管理员创建或编辑项目组合、项目或公司时，可以将其分配给组。 通过将组分配给这些对象，可以轻松确定您的组对这些对象的责任。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月25日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">将组分配给团队</a> </p> <p>为了更便于管理和报告与组关联的团队，您现在可以将任何组分配给有权编辑的团队。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月29日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">管理员的新增功能：将业务负责人分配给组</a> </p> <p>为了帮助您更好地组织和定义组，我们添加了将用户指定为组（或子组）的业务负责人的功能。 业务领导是为组制定业务决策的Workfront用户。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月21日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">适用于MobileIron的Workfront简介</a> </p> <p>Workfront与移动设备管理(MDM)平台MobileIron合作，为组织提供更加安全和可控的移动体验。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版：不适用</p> <p>生产版本： 2020年8月21日</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 资源管理增强功能 {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#plan" class="MCXref xref" xrefformat="{para}">使用工作投入而不是计划小时数计划工作</a> </p> <p>为了让您在计划项目工作时具有灵活性，我们为任务引入了“工作投入”的新概念。 您可以估计任务的工作投入是小型、中型还是大型，而无需手动估计任务的已计划小时数。 每个级别的工作量都是根据实例中配置的典型每天小时数占时间的百分比来计算的。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#project" class="MCXref xref" xrefformat="{para}">工作负载均衡器中工作项的基于项目状态的颜色</a> </p> <p>为了在工作负载均衡器中更好地显示和增强体验的自定义，您现在可以更改项目及其工作项的颜色，以匹配项目状态的状态。 颜色对应于组级别或系统级别的项目状态。 显示的颜色既可以对应于系统状态，也可以对应于自定义项目状态。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#adjust" class="MCXref xref" xrefformat="{para}">在工作负载均衡器中使用百分比值调整用户分配</a> </p> <p>您现在可以在工作负载均衡器中使用百分比而不是小时管理用户的分配。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">在工作负载均衡器中的小时值和百分比值或分配时间和剩余时间之间切换的新图标</a> <p>我们添加了一个新设置，该设置允许您在查看工作负载均衡器时在已分配小时数和百分比之间切换。 通过这个新图标，我们还删除了“设置”面板中的“用户工作负载”部分。 工作负载均衡器默认显示已分配时间，并且我们已将“剩余小时数”设置移动到新的百分比或小时数图标。</p></td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月25日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#a" class="MCXref xref" xrefformat="{para}">用于工作负载均衡器的全新内置过滤器：项目中的用户</a> </p> <p>为了使您在工作负载均衡器中的过滤体验更有效，我们在已分配的工作区域中添加了一个新的内置过滤器。 您现在可以应用项目用户过滤器，该过滤器显示分配给您指定项目中的任务和问题的用户。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月25日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#visualiz" class="MCXref xref" xrefformat="{para}">在工作负载均衡器中可视化已完成的工作</a> </p> <p>为了让您轻松识别已完成的工作以便正确管理用户分配，我们在工作负载均衡器中启用了一个视觉指示器，用于显示所选时间范围内的项目何时完成。 现在，您可以看到任务的绿色复选标记，即任务完成后出现的问题。 当有工作项在屏幕上显示的时间范围内完成时，项目还会显示绿色复选标记。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月11日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">工作负载均衡器中已分配工作区域的新默认过滤器</a> </p> <p>现在，工作负载均衡器中已分配工作区域的默认过滤器仅显示您作为登录用户关联的所有团队成员的用户。 默认情况下，新筛选器现在会显示与您最相关的信息。</p> <p>在此增强功能之前，您有权查看的所有用户都将显示在此区域中。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月11日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#user" class="MCXref xref" xrefformat="{para}">工作负载均衡器中的用户分配图表</a> </p> <p>为了让您在给定的时间范围内拥有用户分配的高级别可视化表示形式，现在新增设置以启用图表视图，了解分配在工作负载均衡器中如何显示。 启用此设置会在折线图中显示用户的分配，以红色块表示过度分配，以蓝色表示过度分配。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月29日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#show" class="MCXref xref" xrefformat="{para}">在工作负载均衡器中显示或隐藏已完成的工作</a> </p> <p>现在，通过新设置可在工作负载均衡器中显示或隐藏已完成的工作项。 该设置默认处于启用状态，并且与过滤条件和所选时间范围匹配的工作项会显示在工作负载均衡器中。 </p> <p>在此增强功能之前，已完成的工作项始终显示在工作负载均衡器中。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月21日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#usabilit" class="MCXref xref" xrefformat="{para}">改进了工作负载均衡器的可用性</a> </p> <p>为了确保您在工作负载均衡器管理资源时获得简化且用户友好的体验，现在提供了各种可用性改进。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月21日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 项目管理增强功能 {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">从项目、任务或问题的详细信息部分中导出自定义表单和概述信息</a> </p> <p>您现在可以将自定义表单信息导出为.pdf文件。 在访问对象的“详细信息”部分中的表单时，可以从项目、任务或问题中导出自定义表单。 </p> <p>除了导出项目、任务和问题的自定义表单之外，您现在还可以将概述区域包含在导出的pdf中。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日（2020年11月3日添加了导出概述区域）</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#quickly" class="MCXref xref" xrefformat="{para}">快速添加迭代</a> </p> <p>为了简化创建小版本的体验，我们添加了一个新按钮，允许您从“小版本”选项卡添加小版本。 在这里，您可以创建迭代，然后稍后添加任务和问题。</p> <p>您仍然可以在积压工作标记上创建迭代，就像之前一样。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日</p> <p>生产版本：随20.4版提供 <span style="color: #dc143c; font-weight: bold;">暂时不可用</span></p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">项目中可用的新量度部分</a> </p> <p>为了节省时间并更好地了解项目的总体运行状况，项目中现在提供了“量度”部分，其中包含有关以下内容的信息：</p> 
    <ul> 
     <li>完成、未完成、逾期和即将完成的工作</li> 
     <li>按状态或优先级分组的任务和问题金额</li> 
     <li>分配给每个用户的工作投入</li> 
    </ul> <p>您可以在图表上进行选择，以查看项目中任务和问题的不同方面，然后单击某些元素以显示任务信息。</p> <p>要了解更多信息，请参阅 <a href="../../../manage-work/projects/manage-projects/project-metrics.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">项目指标概述</a>.</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月23日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">放弃请求草稿时取消操作的新选项</a> <p>放弃已保存的草稿时，您现在可以在通知您将删除草稿的确认消息上单击取消。 这样，您就不会丢失草稿，以防您改变放弃草稿的想法。</p></td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月25日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#replace" class="MCXref xref" xrefformat="{para}">将“处理此项工作”按钮替换为“开始”按钮</a> </p> <p>为了帮助捕获工作项实际开始工作的日期和时间，用户可以将“处理工作”按钮替换为自动更新工作项状态和实际开始日期的“开始”按钮。</p> </td> 
   <td> <p><strong>在以下日期可用：</strong> </p> <p>Beta预览版： 2020年8月20日</p> <p>生产版本： 2020年10月8日</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">通过新字段，可报告顶级组及其所有子组的数据</a> </p> <p>为了帮助您识别与顶级组及其子组关联的数据，我们添加了一个新的顶级父项ID字段，在创建有关组对象的报表时，您可以在筛选器、视图和组中使用该字段。</p> <p>此字段应该对管理包含多个子组的组的组的组管理员特别有用。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月29日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#allow" class="MCXref xref" xrefformat="{para}">允许一个队列主题使用多个草稿</a> </p> <p>为了在处理请求时为您提供更大的自由度，您可以为一个队列主题保存多少草稿不再有任何限制。 创建新请求时，您可以从同一队列主题的草稿列表中选择现有草稿，覆盖它并将其作为新请求提交，也可以从头开始创建新请求。 </p> <p>在此增强功能之前，Workfront仅为请求队列中的每个队列主题保存一个草稿。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年8月21日</p> <p>生产版本： 2020年9月17日</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 已优化的分析  {#enhanced-analytics}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-analytics-enhancements.md#paginati" class="MCXref xref" xrefformat="{para}">已将分页和排序添加到增强型分析</a> </p> <p>为了让您无需应用限制过滤器即可查看希望查看的信息，我们为增强分析区域中的每个图表添加了分页和排序选项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 校对增强功能 {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">生成新版本时结转现有验证工作流</a> </p> <p>现在，现有的校样工作流会传递到您创建的任何新版本，无论这些版本是在什么方法中生成的。</p> <p>以前，验证工作流的传送方式略有不同，具体取决于您在Workfront中生成它们的位置。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月8日</p> <p>生产版本：随20.4版提供 <span class="uitext" style="color: #dc143c;">（推迟到2021年3月）</span></p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#auto-gen" class="MCXref xref" xrefformat="{para}">上传默认禁用的文档设置时自动生成验证</a> </p> <p>默认情况下，新验证用户将禁用用户配置文件中在上传文档时自动生成验证的选项。 此更改不会影响当前用户。 如果已启用此设置，则会保持启用状态。</p> <p>以前，默认为新用户启用此设置。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月18日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#document" class="MCXref xref" xrefformat="{para}">验证查看者中可用的文档审批按钮</a> </p> <p>为了与Classic中的验证体验保持一致，文档审批按钮现在在新Adobe Workfront Experience的验证查看器中可用。</p> <p>以前，您只能从文档详情区域批准文档。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月9日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 移动和集成增强功能 {#mobile-and-integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#added" class="MCXref xref" xrefformat="{para}">在Microsoft Teams通知中添加了功能 </a> </p> <p>为了让您更轻松地通过Microsoft Teams使用Workfront，我们为从Workfront发送的Microsoft Teams通知添加了新功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版：待定</p> <p>生产版本：随20.4版提供 <strong>（推迟到2020年12月或2021年初）</strong></p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#get" class="MCXref xref" xrefformat="{para}">获取有关Workfront mobile虚拟助理命令的帮助</a> </p> <p>在移动应用程序中，您可以通过说“我能做什么？”来请求虚拟助理帮助您执行命令。 一个“帮我听命令”</p> <p>这些命令显示您可以向助理询问的不同内容的列表。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版：不适用</p> <p>生产版本：随20.4版提供 </p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">在Workfront移动设备应用程序中快速创建任务</a> </p> <p>使用Workfront移动设备应用程序中的新快速任务选项快速创建任务。 只需输入任务名称并附加您可能拥有的任何文档即可。 如果需要，您仍然可以填写其他字段，如说明和分配。 只需单击任务名称右侧的箭头。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月18日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他增强功能 {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">改进了Workfront Proof的加密</a> </p> <p>我们正在进行一些更改，以提高Workfront校对应用程序的数据移动加密强度。 弱的TLS密码将于2020年11月11日弃用。</p> <p>访问Workfront时，请确保您使用支持的浏览器。 </p> <p> </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月20日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">3个电子邮件模板的新外观</a> </p> <p>为了提高可读性和整体体验，以下电子邮件模板具有新外观</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">团队的新电子邮件通知</a> </p> <p>我们为团队添加了2个新的电子邮件通知：当分配给您团队的任务的单个前置任务完成时，以及分配给您团队的任务的所有前置任务完成时。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年10月15日</p> <p>生产版本：随20.4版提供</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">触发事件订阅更新的新API对象</a> </p> <p>创建了两个新的API对象documentVersion和proofApproval，并将其配置为在文档进行版本控制或审批时触发事件订阅更新。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>Beta预览版： 2020年9月11日</p> <p>生产版本：随着版本20.4的发布进入生产环境</p> <p><strong>在以下环境中可用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Scenario Planner增强

Workfront Scenario Planner版本20.4中包含的大多数新增功能。 有关这些现在可在“预览”中使用的新功能的信息，请参阅 [Workfront Scenario Planner的20.4版本 — 2020年10月14日](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-20.4.md).

## Workfront目标增强功能

Workfront Goals 20.4版本中随附的大多数新增功能。 有关这些现在可在“预览”中使用的新功能的信息，请参阅 [Workfront 20.4版本的目标](../../../product-announcements/product-releases/goals-release-activity/goals-release-20-4.md).

## Workfront Fusion增强

Workfront Fusion中的新增功能在20.4发布计划之外的生产环境中以一定节奏提供。 有关最新功能的更多信息，请参阅 [Adobe Workfront Fusion发布活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API增强功能

API版本12现已在20.4版本中提供。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

有关新增功能和更新内容的信息，请参阅 [API版本12中的新增功能](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

有关API版本的更多信息，请参阅 [API版本控制和支持计划](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

。

## Workfront 维护更新

有关20.3版本中进行的维护更新的信息，请参阅 [Workfront维护更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 公告

* [Flash弃用](#flash-deprecation)
* [20.4版本网络研讨会](#20-4-release-webinar)
* [预览版本节奏中的更改](#change-in-preview-release-cadence)
* [访问Workfront所需的其他域的允许列表](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Workfront One](#workfront-one)

### Flash弃用 {#flash-deprecation}

2020年底，Adobe和所有主要浏览器都最终确定了弃用的AdobeFlash技术，这意味着这些工具将停止运行。

Workfront旨在通过提供一套不依赖Flash的新解决方案，帮助您转向较新的技术。 有关每个特定基于Flash的工具的替换解决方案的更多信息，请参阅以下文章： [Adobe Workfront中基于Flash的工具的替换](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

所有基于Flash的工具将于2020年11月19日从所有产品中删除。 我们建议您开始使用新工具，并在之后停用Flash工具，以提高实例的安全性。 如果您希望我们在11月19日之前禁用Flash工具，您可以联系客户支持。

### 20.4版本网络研讨会 {#20-4-release-webinar}

Workfront 20.4发布网络研讨会将于2020年10月28日星期三上午11:00（东部夏令时间）举行。 注册网络研讨会 [此处](https://webinars.on24.com/workfront/204release?partnerref=CXnewsletter).

### 预览版本节奏中的更改 {#change-in-preview-release-cadence}

从2020年5月20日开始，Workfront每周开始在预览环境中提供一次功能。 在此更改之前，通常每两周向预览环境发布一次功能。

有关更多信息，请参阅 [Workfront中的更改预览发行节奏常见问题解答](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### 访问Workfront所需的其他域的允许列表 {#allowlist-of-additional-domains-required-for-accessing-workfront}

如果贵组织使用防火墙，则必须将以下其他域添加到列入允许列表中，以确保对Workfront的访问不会出现中断：

* event.split.io
* sdk.split.io

有关更多信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

借助Workfront One，您可以从Workfront中发现最重要的内容、资源和新闻 — 全部放在一个地方，只需登录一次。 我们统一了Experience、Community和Training站点，让您能够更轻松地找到您所寻找的内容。

[了解有关Workfront One的更多信息](https://www.workfront.com/campaigns/workfront-one).
