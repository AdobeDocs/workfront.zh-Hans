---
content-type: release-notes
keywords: 注释，季度，更新
navigation-topic: product-releases
title: 21.1版本概述
description: 21.1版本于一周的生产环境中提供。
author: Luke
feature: Product Announcements
exl-id: 3affee76-347e-4610-b255-4b1bb4414c5d
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '3635'
ht-degree: 0%

---

# 21.1版本概述

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The 21.1 release was made available in the Production environment the week of .</p>
-->

本页介绍了21.1版本中包含的Adobe Workfront Classic和新Adobe Workfront体验的功能信息。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

在此版本中，我们将发布新功能和增强功能，以帮助您通过适应性策略、自动化工作流程和连接的数字基础架构引领2021年的复出，从而在整个企业中取得成功。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 21.1 release nears its planned Production release, this page will be updated with all functionality included with 21.1.</p>
-->

这些增强功能当前可用

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the Preview environment and will be made available
</MadCap:conditionalText>
-->

中。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in the first quarter of 2021
</MadCap:conditionalText>
-->

这些报告在2021年2月15日的一周发布。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.workfront.com/" target="_blank">Adobe Workfront Status Site</a>.
</MadCap:conditionalText>
-->

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [资源管理增强功能](#resource-management-enhancements)
* [项目管理增强功能](#project-management-enhancements)
* [增强的分析改进功能](#enhanced-analytics-improvements)
* [集成增强功能](#integration-enhancements)
* [移动设备增强功能](#mobile-enhancements)
* [其他增强功能](#other-enhancements)

### 管理员增强功能 {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">为复制项目引入新的访问级别设置</a> </p> <p>为了以系统管理员的身份更好地控制计划员对项目的操作，我们通过引入新设置来允许或禁止计划员复制项目的功能，使访问级别中项目的“编辑”访问权限更加精细。 在进行此项更改之前，当您允许用户访问“编辑”项目时，他们将自动拥有复制这些项目的权限。 通过使用新功能，您可以通过禁用新的“复制”设置，为某人授予编辑项目的权限，而不必拥有复制项目的权限。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#in" class="MCXref xref" xrefformat="{para}">在对象的自定义表单中，在多选下拉字段中选择所有项目</a> </p> <p>在对象的“详细信息”(Details)页面上，当您在自定义表单上填写多选下拉字段时，如果需要选择所有可用选项，可以单击全选。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">（当前在您提交新请求时不可用。）</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#recalcul" class="MCXref xref" xrefformat="{para}">为对象重新计算所有自定义表单字段</a> </p> <p>现在更容易确保计算自定义字段中的所有数据都是对象的最新数据。 通过新的“重新计算表达式”菜单选项，您可以快速重新计算这些字段中的所有数据。</p> <p>当某人在对象中的计算自定义字段所引用的另一个对象中编辑数据时，此功能特别有用。</p> <p>以前，用户必须使用解决方法来确保计算自定义字段中的所有数据都是最新的。 例如，他们编辑了对象以及其他对象，以使用可批量编辑的重新计算选项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月10日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#unlock" class="MCXref xref" xrefformat="{para}">解锁组管理员的任务和问题首选项</a> </p> <p>Workfront管理员现在可以通过解锁单个任务和问题首选项来为组管理员提供更多自治权。 解锁首选项后，组管理员可以将其配置为其组，以提供每个组的独特需求和内部进程。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">(在2021年6月24日之前，这仅作为分阶段推出的一部分提供，仅供群集4和6上的客户以及其他一些客户使用。 现在，它可在生产环境中供所有客户使用。)</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">分别为项目组合和项目群配置访问级别设置</a> </p> <p>现在，管理用户对项目组合和项目的访问权限变得更加简单，因为您可以单独配置其访问级别设置。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">在自定义表单中编辑信息时，选中系列中的所有复选框</a> </p> <p>在对象的“详细信息”(Details)页面上，在填写包含复选框的“自定义表单”(Custom Form)字段时，如果需要选择所有可用的复选框，则可以单击“全选”(Select All)。</p> <p>仅当字段包含的复选框数超过2时，才会显示此选项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">（当前在提交请求时不可用。）</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur2" class="MCXref xref" xrefformat="{para}">配置Workfront电子邮件允许列表</a> </p> <p>为了更好地保护您的数据，您现在可以使用电子邮件域允许列表:</p> 
    <ul> 
     <li> <p>如果Workfront电子邮件包含存储在Workfront中的报表或文档，则可以控制其转到何处</p> </li> 
     <li> <p>控制电子邮件域可以位于用户在其用户配置文件中指定的电子邮件地址中</p> </li> 
    </ul> <p>例如，如果要保护敏感数据（例如列出风险客户的报表），则只能在电子邮件中包含内部电子邮件域或允许列表域。 这样，用户便无法将该报表(或任何其他Workfront报表)发送到外部电子邮件地址。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本：在21.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">为子组分配组管理员</a> </p> <p>为了更便于贵组织的级别独立运行，我们添加了将组管理员分配给子组的功能。 现在，您可以确保将子组管理委派给适当的人员。</p> <p>以前，只有顶级组才能具有组管理员，这些管理员管理了顶级组下的所有子组。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#work" class="MCXref xref" xrefformat="{para}">在“组”区域中使用组项目和审批流程</a> </p> <p>如果您是组管理员，那么当您的组项目和审批流程列在“组”区域中时，查看和处理这些项目和审批流程会非常方便。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#configur3" class="MCXref xref" xrefformat="{para}">为组配置事件通知</a> <span style="color: #dc143c; font-weight: bold;">预览中的新增功能！</span></p> <p>Workfront管理员现在可以为组管理员配置顶级组的事件通知，从而赋予组管理员更多的自主权。 子组从其顶部父组继承事件通知配置。</p> <p>以前，事件通知只能由Workfront管理员在系统级别进行配置，这意味着所有组都必须使用同一组事件通知。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月22日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">(最初仅在生产中提供给群集4上的客户，这是分阶段推出的一部分；之后不久便可用于其他群集)</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">查看组中使用和分配的许可证数</a> </p> <p>要确定许可证的分配情况，您现在可以查看组及其下任何子组中使用的许可证数量。</p> <p>如果您管理顶级组，则可以查看组（及其子组）中使用的许可证数量以及为组分配的许可证数量上限。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
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
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workload" class="MCXref xref" xrefformat="{para}">项目的负载平衡器</a> </p> <p>工作负载平衡器现在可在项目中使用。 现在，您可以选择使用负载平衡器还是使用计划工具来管理项目资源。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月17日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-resource-mgt-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Workfront平衡器适用于团队</a> </p> <p>工作负载平衡器现在在团队中可用。 现在，您可以选择使用负载平衡器还是使用计划工具来管理团队资源。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
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
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">导出现在可在项目的“量度”部分中使用</a> </p> <p>为了更轻松地共享项目的状态和进度，您现在可以将项目“量度”部分的整个功能板导出为.png文件。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月15日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#update" class="MCXref xref" xrefformat="{para}">更新从问题更新转换的项目或任务完成的问题百分比</a> </p> <p>我们更新了已转换为项目或任务的问题完成百分比的工作方式。 使用新功能，当问题转换为任务或项目时，当从设置中启用“解决对象更改状态时自动更新可解决的问题状态”设置时，问题完成百分比将与解决任务或项目完成百分比同步更新。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#fields" class="MCXref xref" xrefformat="{para}">从“新请求”页面中删除的字段</a> </p> <p>在重新设计“新请求”页面时，我们更新了在项目的“队列设置”部分中设置的“新问题字段”。</p> <p>仅当从项目的“问题”部分创建问题时，才会显示各种新问题字段。 在“请求”区域中使用请求队列提交问题时，不会显示这些问题。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">（从版本中删除）</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">在“请求”区域提交请求时的新体验</a> </p> <p>为了在提交请求时与Workfront的新体验保持一致并提高效率，我们重新设计了“请求”区域的“新请求”框。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">(从版本中删除；将保留在“预览”状态，并随21.2一起发布到“生产”状态</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#share" class="MCXref xref" xrefformat="{para}">提交请求时共享指向请求队列的链接</a> </p> <p>现在，在创建请求时，我们允许共享指向请求队列、主题组或队列主题的链接。</p> <p>在提交新请求之前，您可以复制指向请求的请求队列、主题组或队列主题的链接，并将其与其他用户共享，或将其嵌入功能板。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月13日</p> <p>生产版本：在21.1版本中 <span style="color: #dc143c; font-weight: bold;">(从版本中删除；将保留在“预览”状态，并随21.2一起发布到“生产”状态</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">新提交的请求列表</a> </p> <p>为了让您以更简单、更一致的方式管理已提交的请求，我们删除了“请求”区域中的“我已提交的请求”和“所有请求”部分，并将其替换为新的“已提交”列表。 该列表具有与系统中所有其他列表相匹配的熟悉外观，允许您筛选不同类别的已提交请求，并快速搜索可能难以找到的请求。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#search" class="MCXref xref" xrefformat="{para}">搜索要分配给项目的群组并查看其详细信息</a> </p> <p>现在，在为项目分配群组时，更容易确保确定正确的群组。 将鼠标悬停在“组”框中找到的组名称上，然后单击该名称旁边显示的信息图标，以查看“组详细信息”工具提示。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月17日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">新建用户委派报表</a> </p> <p>以前，任务、问题和项目批准委托的信息只能由其“主页”区域的代表查看。 为了让其他用户能够看到此信息，计划用户现在可以创建用户委派报表，该报表会告诉您：</p> 
    <ul> 
     <li> <p>已将这些批准委派给其他用户的人员</p> </li> 
     <li> <p>已将这些批准委派给哪个用户</p> </li> 
     <li> <p>这些代表团的开始和结束日期</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月17日</p> <p>生产版本： 2021年1月21日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 增强的分析改进功能 {#enhanced-analytics-improvements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#people" class="MCXref xref" xrefformat="{para}">“人员”页面现在可用于所有聚类</a> </p> <p>“人员”页面现在在用于群集4的Workfront Classic上可用。 本页包括按团队、资源能力和团队能力划分的活动图表。</p> <p>此前，在20.3版本的Workfront Classic中和所有其他群集的新Workfront体验中，均提供了此页面。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月28日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验（以前提供）</p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#enhanced" class="MCXref xref" xrefformat="{para}">增强的分析现在默认显示</a> </p> <p>注意：此更改仅适用于新添加到布局模板的用户。 分配给自定义布局模板的用户也不会受到此更改的影响。</p> <p>在默认的布局模板中，Analytics区域现在默认处于启用状态，这意味着分配给此布局模板的用户现在可以在Workfront Classic的全局导航栏中看到Analytics区域，也可以在新Workfront体验中看到主菜单。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月6日</p> <p>生产版本： 2020年12月3日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-enhanced-analytics-improvements.md#availab" class="MCXref xref" xrefformat="{para}">增强的分析功能适用于所有群集</a> </p> <p>增强的Analytics适用于所有Workfront群集，包括群集6上的客户。</p> <p>以前，Google云平台中不提供增强的分析功能，这会阻止群集6上的客户访问Analytics区域。 现在，群集6上的业务客户和企业客户可以访问Analytics区域。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年11月20日</p> <p>生产版本： 2020年12月3日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 集成增强功能 {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">Adobe WorkfrontMicrosoft Teams中的通知增强功能</a> </p> <p>为了更便于您通过Microsoft Teams使用Workfront，我们对从Workfront发送的Microsoft Teams通知添加了各种增强功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本：不适用</p> <p>生产版本： 2021年1月12日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### 移动设备增强功能 {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Adobe Workfront应用程序中的新导航痕迹导航</a> </p> <p>我们在Workfront移动应用程序中添加了痕迹导航导航。 现在，您可以使用此功能导航到项目中的父工作项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本：不适用</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#rich" class="MCXref xref" xrefformat="{para}">Workfront应用程序上自定义表单支持的富文本</a> </p> <p>您现在可以在Workfront移动设备应用程序的自定义表单文本字段中使用富文本格式。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本：不适用</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-mobile-enhancements.md#sso" class="MCXref xref" xrefformat="{para}">SSO用户现在可以使用面部ID或指纹技术重新登录Workfront应用程序</a> </p> <p>如果贵组织使用单点登录(SSO)，则您现在可以在会话超时后使用面部ID或指纹登录到Workfront移动应用程序。 但是，您必须先使用SSO凭据登录。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本：不适用</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>
—&gt;

### 其他增强功能 {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#updates" class="MCXref xref" xrefformat="{para}">更新了事件订阅失败要求</a> </p> <p>我们正在更新“事件订阅”失败的软禁用要求。 除了现有要求外，如果“事件订阅”在2000次尝试内未能成功交付，则现在将软性禁用它们。 这是为了加强现有的70%失败规则，在某些情况下，这一规则可能导致过多的失败。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本：不适用</p> <p>生产版本： 2021年1月11日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">“每日摘要”中提供的新团队字段</a> </p> <p>我们在“需要的每日摘要操作”电子邮件中添加了“团队批准”和“分配”字段。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月17日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#replacin" class="MCXref xref" xrefformat="{para}">替换请求队列中的POP电子邮件选项</a> </p> <p>我们正在将请求队列的POP电子邮件选项替换为新的Workfront管理系统。 您仍可以通过电子邮件提交请求，但是您需要在“请求队列”区域设置一个由Workfront管理的新电子邮件地址。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月17日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#restrict" class="MCXref xref" xrefformat="{para}">限制对工时单的时间编辑</a> </p> <p>为了更好地控制工时单和工时编辑，我们添加了一个设置，允许您将工时编辑限制在工时单所有者和系统管理员。</p> <p>以前，在其访问级别中启用“工时单和工时”选项的用户可以编辑任何工时单上的工时。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2021年1月21日</p> <p>生产版本：在21.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">改进了“工时单”区域中的过滤器和视图</a> </p> <p>我们为项目和问题添加了过滤器，并在“搜索”页面中添加了“查看”和“分组”选项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本： 2021年1月21日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#hide" class="MCXref xref" xrefformat="{para}">在工时单中隐藏超时框</a> </p> <p>现在，如果您不在Workfront中跟踪超时，则可以隐藏超时框以缓解用户混淆。 您可以隐藏一次性使用的工时单或工时单配置文件的超时框。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月2日</p> <p>生产版本： 2020年12月16日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#expand" class="MCXref xref" xrefformat="{para}">在痕迹导航导航中展开或折叠项目</a> </p> <p>为了更便于查看完整的痕迹导航路径，我们添加了展开和折叠功能。</p> <p>现在，任何已截断的项目都会在项目之前进行分组，并包含文本“更多”。 例如，“3个以上”表示有3个对象未显示。</p> <p>以前，您必须单击省略号才能在下拉菜单中显示任何截断的对象。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年1月7日</p> <p>生产版本： 2021年1月21日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/21.1-release-activity/21-1-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">痕迹导航的新外观</a> </p> <p>为了帮助用户更好地识别他们在Workfront中的位置，并更轻松地在对象之间导航，我们对痕迹导航进行了多项改进。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>测试版预览版本： 2020年12月10日</p> <p>生产版本： 2021年1月21日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront目标增强功能

21.1版本中Workfront Target版本的大多数新增功能。 有关预览中当前提供的这些新增功能的信息，请参阅 [Adobe Workfront Goals与21.1版本](../../../product-announcements/product-releases/goals-release-activity/goals-release-21-1.md).

## Workfront Scenario Planner增强功能

21.1版本中Workfront方案规划器版本的新增功能。 有关预览中当前提供的这些新增功能的信息，请参阅 [Adobe Workfront 21.1版本的方案规划器](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-21-1.md).

## Workfront Fusion增强功能

在21.1版本计划之外，Workfront Fusion的新增功能在生产环境中以一定频率提供。 有关最新功能的更多信息，请参阅 [Adobe Workfront Fusion版本活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## API增强功能

API版本12现已在20.4版本中提供。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

有关新增功能和更新功能的信息，请参阅 [API版本12的新增功能](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

有关API版本的更多信息，请参阅 [API版本控制和支持计划](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

。

## Workfront 维护更新

有关21.1版本期间进行的维护更新的信息，请参阅 [Workfront维护更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 公告

* [21.1版本中Workfront电子邮件的新IP地址](#new-ip-addresses-for-workfront-email-with-the-21-1-release)
* [允许列表为事件订阅管理其他IP地址](#allowlist-of-additional-ip-addresses-for-event-subscriptions)
* [允许列表访问Workfront所需的其他域](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Flash弃用](#flash-deprecation)
* [21.1版网络研讨会](#21-1-release-webinar)
* [预览版发行频率的更改](#change-in-preview-release-cadence)
* [Workfront One](#workfront-one)

### 21.1版本中Workfront电子邮件的新IP地址 {#new-ip-addresses-for-workfront-email-with-the-21-1-release}

为了增加成功的电子邮件投放，我们正在通过群集1、2、3、4和5的21.1生产版本添加新的IP地址。

有关需要为群集添加哪些IP地址的详细信息，请参阅 [21.1版本中Adobe Workfront电子邮件的新IP地址](../../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md).

要了解您所在的群集，请转到设置>系统>客户信息。

### 允许列表为事件订阅管理其他IP地址 {#allowlist-of-additional-ip-addresses-for-event-subscriptions}

为了增加成功的事件订阅交付，我们将在2021年第一季度的21.1生产版本中添加4个新IP地址。 您必须在2021年2月之前将这允许列表些IP地址添加到您的，以确保您的用户继续接收事件订阅。

请联系您的内部IT和/或安全部门，以获取有关添加文章中新IP的帮助， [事件订阅API](../../../wf-api/general/event-subs-api.md).

### 允许列表访问Workfront所需的其他域 {#allowlist-of-additional-domains-required-for-accessing-workfront}

如果贵组织使用防火墙，则必须向您的中添加以允许列表下其他域，以确保无中断地访问Workfront:

* event.split.io
* sdk.split.io

有关更多信息，请参阅 [配置防火墙的允许列表](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Flash弃用 {#flash-deprecation}

2020年11月19日，所有基于Flash的工具都从所有产品中删除了。

请在以下文章中了解有关每个基于Flash的特定工具的替换解决方案的更多信息： [在Adobe Workfront中替换基于Flash的工具](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

### 21.1版网络研讨会 {#21-1-release-webinar}

Workfront 21.1版网络研讨会将于美国东部夏令时上午11:00 /英国夏令时下午4:00举行。 注册网络研讨会 [此处](https://event.on24.com/eventRegistration/EventLobbyServlet?target=reg20.jsp&amp;partnerref=ac&amp;eventid=2934272&amp;sessionid=1&amp;key=5C231B3385686D1E224A49EBE0BF0E37&amp;regTag=&amp;V2=false&amp;sourcepage=register).

### 预览版发行频率的更改 {#change-in-preview-release-cadence}

从2020年5月20日开始，Workfront每周都会在预览环境中提供相应功能。 在进行此项更改之前，通常每两周向预览环境发布一次功能。

有关更多信息，请参阅 [Workfront预览版发行频度常见问题解答中的更改](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### Workfront One {#workfront-one}

借助Workfront One，您将能够从Workfront中发现最重要的内容、资源和新闻 — 所有这些内容都位于一个位置，只需登录一次。 我们统一了体验、社区和培训网站，从而更轻松地找到您要查找的内容。

[进一步了解Workfront One](https://www.workfront.com/campaigns/workfront-one).
