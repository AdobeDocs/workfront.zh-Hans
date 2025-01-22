---
title: 22.2发行版概述
description: 22.2发行版概述
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: e490a955-b2cb-4b9b-9794-12ff2a2c2338
source-git-commit: 552e97c427e618f299b55a2eab5868c7b90a4156
workflow-type: tm+mt
source-wordcount: '3974'
ht-degree: 0%

---

# 22.2发行版概述

本页介绍了22.2版本中包含的功能。 新增的Adobe Workfront Experience中提供了列出的所有功能。 Adobe Workfront Classic中还提供了某些功能；但是，[Workfront Classic将于2022年3月停产](https://one.workfront.com/s/new-workfront-experience)，此后不久将于2022年7月结束Workfront Classic的生命周期。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
to help you unlock productivity and collaboration.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.2 release nears its planned Production release later this year
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
the week of January 17, 2022
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.2. </p>
-->

这些增强功能在2022年4月4日当周的生产环境中提供。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
later this year
</MadCap:conditionalText>
the week of April 4, 2022, unless otherwise specified. For specific release dates and times for each cluster, see the <a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on <a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times. </p>
-->

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [项目增强功能](#project-enhancements)
* [资源管理增强功能](#resource-management-enhancements)
* [主页增强功能](#home-enhancements)
* [移动增强功能](#mobile-enhancements)
* [集成增强功能](#integrations-enhancements)
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#configur" class="MCXref xref" xrefformat="{para}">配置自定义表单以使用多个对象类型</a> </p> <p>现在，您可以配置新的或现有的自定义表单以与多个对象类型一起使用，从而使表单具有更广泛的用途。 用户将能够在您为其配置表单的所有类型的对象上附加和填写表单。</p> <p>以前，您可以将自定义表单配置为仅使用一个对象类型。</p> <p>此功能适用于之前在Workfront系统中创建的所有自定义表单。 例如，如果您已经拥有为Task对象类型创建的自定义表单，则现在可以将其配置为也与其他对象类型一起使用，如“项目”和“问题”。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Blueprint目录可供所有用户使用，管理员可以允许请求</a> </p> <p>所有Adobe Workfront用户现在都可以浏览可用Blueprint的目录。 </p> <p>此外，系统管理员可以为用户启用访问权限，以请求安装Blueprint。 通过分配请求队列来存储请求，用户可以从Blueprint目录发出请求。 </p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">将图像添加到自定义表单</a> </p> <p>在您创建或编辑的自定义表单中，您现在可以添加图像并包含信息性或说明性工具提示，用户将鼠标悬停在该图像上时可以阅读这些工具提示。</p> <p>例如，这对于显示新产品的品牌或提供用户在填写表单时所需的视觉信息可能很有帮助。</p> <p>以前，自定义表单完全基于文本。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#deactiva" class="MCXref xref" xrefformat="{para}">停用组</a> </p> <p>随着内部组织的变化，您可能需要停止使用Workfront中的某些组并创建新组。 为了帮助解决此问题，我们添加了取消激活组的功能，而不会丢失其历史数据。 对于不需要查看的非活动用户，将从组预输入字段中清除非活动组。</p> <p>您仍然可以查找和配置您管理的非活动组的选项、首选项和对象关联。 而且，停用组不会更改与该组连接的对象有关的任何内容。</p> <p>以前，无法停用组。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#new" class="MCXref xref" xrefformat="{para}">新的默认访问级别配置</a> </p> <p>为了更好地满足大多数创建访问级别的管理员的需求，我们更改了当您单击编辑按钮上的齿轮图标时显示的若干“微调您的设置”选项的默认配置。</p> <p>以前默认启用的选项现在处于禁用状态。 如果这不符合贵组织的需求，则可以在设置新访问级别时或稍后随时启用它们。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年1月27日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月停产</a>，之后不久将于2022年7月终止Workfront Classic的生命周期。)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#blueprin2" class="MCXref xref" xrefformat="{para}">Blueprint安装历史记录增强</a> </p> <p>安装Blueprint时，现在会显示一条消息，其中显示已成功与Blueprint一起安装的特定对象（例如角色、团队或组）以及任何无法安装的对象。 您还可以通过单击安装历史记录表中特定安装旁边的查看详细信息，查看“Blueprint详细信息”页面上的已安装对象列表。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-admin-enhancements.md#a" class="MCXref xref" xrefformat="{para}">在生产中安装仅预览版Blueprint时现在显示警告</a> </p> <p>某些Blueprint仅可用于在“预览”环境中安装以进行测试。</p> <p>如果您在生产环境、沙盒1或沙盒2中访问仅预览内容，则安装按钮无效，您可能会看到一条警告消息。</p> </td> 
   <td><b>在以下日期可用：</b> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 项目增强功能 {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">Adobe Workfront讨论区现已可用！</a> </p> <p>展示板是一种灵活的工具，通过提供对包含列和卡片的共享展示板的访问，允许团队协作。 </p> <p>使用展示板，您可以快速设置具有多个列的任务展示板、配置列以显示状态或类别、将其他用户添加到展示板并将它们分配给信息卡等。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#addition" class="MCXref xref" xrefformat="{para}">对Workfront展示板的其他改进</a></p> <p>Workfront展示板现在提供以下其他改进：</p> 
    <ul> 
     <li> <p>展示板上的标记卡</p> </li> 
     <li> <p>移动卡片</p> </li> 
     <li> <p>复制卡片</p> </li> 
     <li> <p>在讨论区中搜索</p> </li> 
     <li> <p>在展示板中设置卡的到期日期</p> </li> 
    </ul> </td> 
   <td><b>在以下日期可用：</b> 
    <ul> 
     <li> <p>预览版本： 2022年3月24日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#undo" class="MCXref xref" xrefformat="{para}">撤消更新帖子的选项</a> </p> <p>现在，在发布更新时更容易发现错误。 现在，在对象的“更新”选项卡中完成评论时，会创建一个弹出窗口，持续7秒，允许您在系统为其设置时间戳或发送任何电子邮件和应用程序内通知之前取消帖子并返回编辑。 如果关闭弹出窗口，离开页面，或等待窗口超时7秒，则正常开机自检。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">复制项目时的新体验</a> </p> <p>为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们重新设计了用于复制项目的界面。 当前在从项目页面复制项目时，或者从列表或报表复制项目时，此功能可用。 在此更新之前，您只能从项目页面复制项目。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#ability" class="MCXref xref" xrefformat="{para}">能够通过新的“更多”菜单从列表和报告管理项目</a> </p> <p>我们在项目列表和报告中添加了新的“更多”菜单，允许您从这些区域执行以下操作：</p> 
    <ul> 
     <li> <p>对于同时执行多个项目：</p> </li> 
     <li> <p>重新计算时间线</p> </li> 
     <li> <p>重新计算财务</p> </li> 
     <li> <p>重新计算自定义表达式</p> </li> 
     <li> <p>对于单个项目：</p> </li> 
     <li> <p>附加模板</p> </li> 
     <li> <p>导出至 MS 项目</p> </li> 
     <li> <p>订阅</p> </li> 
    </ul> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">使用问题级别的模板将问题转化为项目时的新体验</a> </p> <p>为了让您在使用Workfront时与新的Workfront体验保持一致，我们重新设计了界面，在您从问题页面转换模板时将问题转换为项目时，使用该界面。</p> <p>现在，在选择转换问题后，您可以更轻松地立即访问收藏夹列表。</p> <p>重新设计的界面与我们最近更新的模板创建项目时的体验相匹配。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2021年12月8日<br></p> </li> 
     <li> <p>生产版本：在22.1版本<span style="color: #ff0000; font-weight: bold;">中，此功能已于2022年3月4日从生产环境中临时删除。 该版本后来在2022年4月28日开始分阶段发布。 推广已于2022年5月5日完成。 现在，所有客户都可以在预览和生产环境中使用它。</span></p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">使用列表、报告和报告面板中的模板将问题转化为项目</a> </p> <p>为了提高您的工作效率并让您更轻松地在快节奏环境中转化问题，我们添加了使用列表、报告或功能板中的模板将问题转化为项目的功能。</p> <p>在此增强功能之前，仅当您从问题页面转换问题时，此功能才存在。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2021年12月8日<br></p> </li> 
     <li> <p>生产版本：在22.1版本<span style="color: #ff0000; font-weight: bold;">中，此功能已于2022年3月4日从生产环境中临时删除。 该版本后来在2022年4月28日开始分阶段发布。 推广已于2022年5月5日完成。 现在，所有客户都可以在预览和生产环境中使用它。</span></p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">复制和移动问题时更新体验</a> </p> <p>为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们重新设计了用于复制和移动问题的界面。 目前，在复制或移动单个问题，或者从列表或报告批量复制或移动问题时，此功能可用。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月18日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>将问题转化为项目后，<a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#keep" class="MCXref xref" xrefformat="{para}">将用户保留在仪表板、列表或报告中</a> </p> <p>为了提高效率并消除点击次数，在从列表、报告或仪表板将问题转化为项目时，我们发布了一项改进。</p> <p>将问题转化为项目后，用户仍保留在列表、报表或功能板中，而不是被重定向到项目的页面。 转换完成后，将显示一个成功通知，其中包含指向项目的链接，以便您根据需要轻松导航到项目。 </p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日<br></p> </li> 
     <li> <p>生产版本： 2022年2月24日</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">对分配进行更改时，分配小时数将不再删除</a> </p> <p>为了确保数据的准确性，我们在更改任务的分配时，进行了相应更改，以保留分配小时数，并保留任务计划小时数不变。</p> <p>已对具有简单持续时间类型的任务进行了以下更改：</p> 
    <ul> 
     <li> <p>替换用户和角色时，会保留单独的分配分配。</p> </li> 
     <li> <p>删除用户时，会保留角色上的各个分配分配。</p> </li> 
     <li> <p>删除所有被分配人时，保留计划的小时数。 <span style="color: #ff0000;">(已从版本中删除。 现在，在删除所有被分配人后，计划小时数将设置为0。)</span></p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日<br></p> </li> 
     <li> <p>生产版本：在22.2版本<span style="color: #ff0000; font-weight: bold;">中，此功能将在22.2版本</span>之后不久发布到生产环境</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月停产</a>，之后不久将于2022年7月终止Workfront Classic的生命周期。)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">仅在文件夹层次结构的最前五个级别共享文件夹</a> </p> <p>为确保用户共享文件夹获得最佳性能，我们当前将共享限制为对象上文件夹层次结构中的前五个级别。</p> <p>第六级或更低级别的每个文件夹都从其正上方的文件夹继承其共享配置。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日<br></p> </li> 
     <li> <p>生产版本：在22.2版本<span style="color: #ff0000; font-weight: bold;">中，此功能暂时不可用。 当此功能在生产环境中可用时，将更新此页面。</span></p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月停产</a>，之后不久将于2022年7月终止Workfront Classic的生命周期。)</p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">工作负载均衡器导航改进</a> </p> <p>为了改进在使用工作负载均衡器时的体验，我们引入以下增强功能：</p> 
    <ul> 
     <li> <p>现在，即使任务时间长于屏幕上包含的时间范围或者显示摘要面板，调整分配时的取消和保存按钮都是粘滞的。</p> </li> 
     <li> <p>显示用户名称和工作项的左侧面板现在为“粘性”，可让您水平滚动较长的时间范围，并且仍然能够读取面板中列出的项目名称。</p> </li> 
     <li> <p>只需单击一下即可折叠和展开左侧面板中列出的所有项目，而无需在用户或项目级别单击。</p> </li> 
     <li> <p>现在，左侧面板也可以调整大小。</p> </li> 
     <li> <p>工作负载均衡器现在提供全屏模式。</p> </li> 
    </ul> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#access" class="MCXref xref" xrefformat="{para}">访问工作负载均衡器中的高级分配</a> </p> <p>为了使分配工作项更容易、更准确，现在当在工作负载均衡器中手动分配工作项时，可以进行高级分配。 在此增强功能之前，您可以在编辑项目、项目标题或列表中访问高级工作。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-resource-management-enhancements.md#new" class="MCXref xref" xrefformat="{para}">选择“默认计划”首选项时用于计算用户可用性的新公式</a> </p> <p>为了在资源管理工具中提供更准确的信息，我们更改了Workfront管理员在资源管理首选项中选择默认计划时Workfront用于计算用户可用性的公式。 通过新的更新，Workfront使用以下公式计算用户可用性：</p> <p>用户可用小时数=（默认计划小时数 — 例外）* FTE — 休息时间小时数</p> <p>在此更新之前，在选择了“默认计划”时，Workfront使用以下公式计算用户可用性：</p> <p>用户可用小时数=(默认计划小时数 — （计划例外+休息时间小时数）)x用户FTE值</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月停产</a>，之后不久将于2022年7月终止Workfront Classic的生命周期。)</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 主页增强功能 {#home-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-home-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">主页工作列表中的筛选器改进</a> </p> <p>为了更好地控制和关注您的工作列表，我们在“主页”区域对过滤器进行了多项改进。 利用新的改进功能，您可以按对象类型选择筛选器，并按工作项的状态（例如，准备开始、处理或请求）进一步缩小结果。 现在，当您应用对象类型和工作项状态筛选器的组合时，新的主页筛选器可提供任务、问题、个人工作项和审批的正确计数。</p> <p>在此体验之前，当您选择一个或多个筛选器时，主页区域中的筛选器未提供列表中工作项数量的准确计数，并且这些筛选器导致工作项状态混乱。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 移动增强功能 {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-mobile-enhancements.md#drawings" class="MCXref xref" xrefformat="{para}">移动应用程序中的验证文档的绘图和注释</a></p> <p>Adobe Workfront移动设备应用程序现在允许您在校样文档中添加绘图和注释。 验证中的新工具栏包含形状绘制工具。 可以为每个形状选择颜色和线条粗细等设置。 在校样上绘制形状可将您的注释连接到校样文档的该区域。</p> <p>您也可以回复他人对证明所做的评论。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本：不适用<br></p> </li> 
     <li> <p>生产版本： 2022年4月中下旬 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>iOS移动应用程序</p> </li> 
     <li> <p>Android移动应用程序</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">对移动应用中的校对功能的增强</a> </p> <p>在Adobe Workfront移动设备应用程序中，您现在可以：</p> 
    <ul> 
     <li> <p>与内部和外部收件人共享验证</p> </li> 
     <li> <p>查看校对评论</p> </li> 
     <li> <p>下载校样</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本：不适用<br></p> </li> 
     <li> <p>生产版本：2022年2月初（这些增强功能最初与22.1版本沟通。）</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>iOS移动应用程序</p> </li> 
     <li> <p>Android移动应用程序</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 集成增强功能 {#integrations-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发布日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe" class="MCXref xref" xrefformat="{para}">与Anaplan集成的Adobe Workfront现已可用</a> </p> <p>为了让您更灵活地了解Workfront项目的财务方面，Workfront现在可以与您的Anaplan帐户集成。 通过将Workfront对象链接到Anaplan对象，您可以自动更新这两个帐户之间的信息，确保这两个帐户中的信息都是最新且相同的。 </p> <p>您还可以根据Workfront中的操作在Anaplan中触发自动流程（反之亦然）。</p> <p>例如，您可以在Anaplan中创建营销策划，然后创建链接到该营销策划的Workfront项目或项目。 在Workfront中跟踪的任何成本都可以上传回Anaplan以审查营销活动效果。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#workfron" class="MCXref xref" xrefformat="{para}">用于Experience Manager增强型连接器更新的Workfront</a> </p> <p>Workfront for Experience Manager增强型连接器现在包含以下更新：</p> 
    <ul> 
     <li> <p>现在，即使存在多个项目链接文件夹配置，您也可以在Adobe Workfront和Adobe Experience Manager Assetsas a Cloud Service之间创建链接文件夹。</p> </li> 
     <li> <p>添加了对事件订阅分页的支持</p> </li> 
     <li> <p>添加了对AEM 6.4.x的支持</p> </li> 
     <li> <p>添加了对代理环境的支持</p> </li> 
     <li> <p>基于合作伙伴和客户反馈的多项错误修复</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本：不适用<br></p> </li> 
     <li> <p>生产版本： 2022年3月28日</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
     <li> <p>Adobe Workfront Classic </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see" class="MCXref xref" xrefformat="{para}">查看自定义OAuth2或JWT集成的客户端密钥的详细信息</a> </p> <p>为了让您透明地使用自定义OAuth2和JWT集成，我们让您能够查看集成使用的客户端密钥的详细信息。 现在，您可以查看客户端密钥的创建日期和上次使用日期。 您还可以添加和查看您自己的有关客户端密钥的注释。</p> <p>以前，这些详细信息不可用。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年3月3日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#adobe2" class="MCXref xref" xrefformat="{para}">Adobe Creative Cloud集成现在使用OAuth2</a> </p> <p>为了提高安全性和跨集成实现更一致的体验，我们更新了Adobe Creative Cloud集成，以使用OAuth2身份验证（一种行业标准对用户进行身份验证的方式）。 现在，当您的用户登录时，他们可以看到集成有权访问的特定操作和区域，并且可以允许访问。 之后，他们无需频繁登录。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月24日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#see2" class="MCXref xref" xrefformat="{para}">在自定义OAuth2应用程序列表中查看身份验证类型</a> </p> <p>现在，当您查看组织中的自定义OAuth2应用程序列表时，可以查看每个应用程序是使用用户身份验证还是服务器身份验证。</p> <p>以前，您只能通过进入每个应用程序上的编辑选项来查看此信息。</p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年2月17日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#set" class="MCXref xref" xrefformat="{para}">在自定义OAuth2集成中设置刷新令牌的过期时间</a> </p> <p>为了更好地控制自定义OAuth2集成的访问和安全性，您现在可以自定义刷新令牌的有效期。 用户的刷新令牌过期后，他们需要再次登录到集成。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日 <br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-integration-enhancements.md#use" class="MCXref xref" xrefformat="{para}">在服务器到服务器应用程序的自定义OAuth2集成中使用公钥和私钥</a> </p> <p>您现在可以在自定义集成中设置服务器到服务器OAuth2应用程序。 通过设置公钥和私钥，您可以允许Workfront与另一个应用程序通信，而无需使用登录凭据。</p> <p>以前，您的自定义OAuth2应用程序中的所有身份验证都使用用户的登录凭据。</p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> 
    <ul> 
     <li> <p>预览版本： 2022年2月10日 <br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供 </p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-look-and-feel-updates.md#enhancem" class="MCXref xref" xrefformat="{para}">在22.2发布时间范围内的外观更新</a> </p> <p>在22.2版本发布时间范围内，对Adobe Workfront应用程序各个区域的外观进行了小幅更新。 这些增强功能将在发布到“预览”环境后至少2周内在“生产”环境中提供。 </p> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本：在整个22.2版本发布时间范围内<br></p> </li> 
     <li> <p>生产版本：发布到“预览”状态后至少2周</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">对顶部导航栏的增强</a> </p> <p>我们对Adobe Workfront顶部导航栏进行了几项增强。</p> 
    <ul> 
     <li> <p>“收藏夹”和“最近访问”在顶部导航栏中有单独的图标。 每个页面仍显示相同的内容（已标记为收藏的页面和最近访问的页面），您可以继续以相同方式添加和删除收藏的页面。</p> </li> 
     <li> <p>针脚和主菜单的外观和感觉已更新为Adobe设计标准，包括色彩和字体。 在主菜单中添加和删除大头针以及您有权访问的区域的方式没有改变。</p> </li> 
     <li> <p>顶部导航栏右侧的图标进行了重新排序，以便更加直观。 图标顺序为：帮助链接、通知、收藏夹、最近访问、搜索、主菜单。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-other-enhancements.md#redesign" class="MCXref xref" xrefformat="{para}">重新设计的工时表列表</a> </p> <p>为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们重新设计了“时间表”区域中的时间表列表。 您可以期待时间表列表具有相同的功能，但用户体验会更干净、更简化。</p> <p>此重新设计的一些亮点包括：</p> 
    <ul> 
     <li> <p>时间表列表现在与Workfront所有其他列表中的体验相匹配。</p> </li> 
     <li> <p>过滤器体验现在与所有其他列表中的过滤器相匹配。 您将可以更灵活地使用对您最有意义的字段和属性创建自己的过滤器，并将其与其他用户共享。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> 
    <ul> 
     <li> <p>预览版本： 2022年3月10日<br></p> </li> 
     <li> <p>生产版本：随22.2版一起提供</p> </li> 
    </ul> <p><strong>在以下环境中可用：</strong> </p> 
    <ul> 
     <li> <p>新的Adobe Workfront体验 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion增强

Workfront Fusion中的新增功能在22.2发布计划之外的生产环境中以一定节奏提供。 有关最新功能的详细信息，请参阅[Adobe Workfront Fusion发行活动](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

## Workfront Scenario Planner增强

此版本中目前没有Scenario Planner更新。 在有可用更新时，将更新此区域。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof增强功能

此版本中目前没有Workfront Proof更新。 在有可用更新时，将更新此区域。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Workfront目标增强功能

此版本中目前没有更新Workfront Goals。 在有可用更新时，将更新此区域。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API版本14

对于API版本14，我们修改了一些资源和端点。 一些更改支持新功能，而其他更改使您能够更轻松地使用通过API获得的信息。

有关新增功能和更新的信息，请参阅[API版本14](../../../wf-api/api/new-api-version-14.md)中的新增功能。

有关API版本的信息，请参阅[API版本控制和支持计划](../../../wf-api/api/api-version-support-schedule.md)。

## Workfront 维护更新

有关22.2版本期间所做的维护更新的信息，请参阅[Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

## 22.2版本网络研讨会

Workfront 22.2版本网络研讨会将于2022年3月24日上午8:00（山区标准时间）举行。 您可以在Workfront One](https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne)的[事件页面上注册该事件。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## 培训更新

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关详细信息，请参阅[培训版本更新页面](https://one.workfront.com/s/training-release-updates)。

## 不再支持的功能

### Internet Explorer 11

由于不再支持Internet Explorer，Workfront现在正式支持Microsoft Edge。

有关支持的浏览器的更多信息，请参阅[Adobe Workfront浏览器要求](../../../workfront-basics/workfront-browser-requirements.md)。
