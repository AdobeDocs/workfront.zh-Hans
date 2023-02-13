---
title: 22.1版本概述
description: 22.1版本概述
author: Luke
draft: Probably
feature: Product Announcements
exl-id: daf977fe-957a-40ad-a37f-1c164cb4ada3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '4721'
ht-degree: 0%

---

# 22.1版本概述

本页介绍了22.1版本中包含的功能。 所有功能均在新的Adobe Workfront体验中提供。 Adobe Workfront Classic中还提供一些功能；但是， [Workfront Classic将于2022年3月终止](https://one.workfront.com/s/new-workfront-experience)，紧随其后，Workfront Classic于2022年7月终止其生命周期。

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
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment. As the 22.1 release nears its planned Production release the week of January 17, 2022
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in October 2021
</MadCap:conditionalText>
, this page will be updated with all functionality included with 22.1. </p>
-->

这些增强功能已于2022年1月17日这一周的生产环境中提供。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of January 17, 2022, unless otherwise specifiedthe week of May 10, 2021
</MadCap:conditionalText>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
For specific release dates and times for each cluster, see the
<a href="https://status.adobe.com/en/products/5943" target="_blank">Adobe Workfront status page</a> on
<a href="http://status.adobe.com/" target="_blank">status.adobe.com</a>. You must log in to see specific release times
</MadCap:conditionalText>
-->

。

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [项目增强功能](#project-enhancements)
* [资源管理增强功能](#resource-management-enhancements)
* [请求增强功能](#requests-enhancements)
* [校对增强功能](#proofing-enhancements)
* [其他增强功能](#other-enhancements)
* [移动设备增强功能](#mobile-enhancements)

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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#document" class="MCXref xref" xrefformat="{para}">记录在“更新”区域中的文档下载</a> </p> <p>为了帮助您的用户跟踪他们存储在Workfront中的文档的下载，现在当有人下载文档时，系统会在“更新”区域中为文档记录一个条目。</p> <p>我们建议在新上传的文档的“预览”中测试此功能。</p> </td> 
   <td> <p>预览版本：2021年12月16日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#create" class="MCXref xref" xrefformat="{para}">创建OAuth2应用程序以将应用程序与Workfront集成</a> </p> <p>现在，您可以将Workfront与Workfront未提供内置集成的其他应用程序集成。 通过为要与集成的应用程序创建OAuth2应用程序，您可以允许该应用程序访问Workfront，同时知道您的数据受安全的行业标准OAuth2身份验证协议的保护。</p> <p>以前，您只能通过内置集成、Workfront Fusion或Workfront API与其他应用程序集成。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月8日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">“公司”区域的界面文本改进</a> </p> <p>在“设置”的“公司”区域中，新的确认消息和细微的措辞更改使管理公司成员资格变得更加容易。 例如，左侧面板中名为“人员”的部分现在为“公司成员”。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月8日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#add" class="MCXref xref" xrefformat="{para}">将自定义表单添加到群组</a> </p> <p>组对象现在支持自定义表单。 这样，贵组织中的群组便于捕获和共享满足其特定需求和工作流程的信息。 用户可以对组执行与其他Workfront对象相同的操作，例如创建自定义表单、附加自定义表单、保存自定义表单等。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月8日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#styling" class="MCXref xref" xrefformat="{para}">自定义Forms区域中的样式更新</a> </p> <p>“自定义Forms”区域具有新的外观，可使其与新Workfront体验中的许多其他区域保持最新。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#many" class="MCXref xref" xrefformat="{para}">许多用于创建计算自定义字段的增强功能</a> </p> <p>现在，通过在新的计算编辑器中添加这些内容，可以更轻松地创建计算自定义字段：</p> 
    <ul> 
     <li> <p>您可以将鼠标悬停在计算中的任何表达式上以显示有关该表达式的信息，包括描述、如何使用该表达式的示例，以及指向帮助文章中更多信息的链接。</p> </li> 
     <li> <p>您添加的每个表达式都采用颜色编码，具体取决于其类型。 这样，您就更容易发现表达式并立即识别其类型。</p> </li> 
     <li> <p> 行号可帮助您在较长的计算中识别和引用函数。</p> </li> 
     <li> <p>开始键入表达式或字段名称时，将显示可用项目列表，以便您选择所需的项目。 此外，当您键入左圆括号时，将自动添加右圆括号。</p> </li> 
     <li> <p>您可以使用现有对象预览计算结果，而无需离开计算编辑器。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月3日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select" class="MCXref xref" xrefformat="{para}">在新的计算字段窗口中选择表达式和字段</a> </p> <p>我们将继续简化在自定义表单中创建计算字段的过程。 现在，当您单击最大化以打开新的计算编辑器时，您可以找到并选择所需的表达式和字段。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月21日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#larger" class="MCXref xref" xrefformat="{para}">用于创建计算字段的更大区域</a> </p> <p>现在，更轻松地在自定义表单中生成复杂的计算字段。 单击新的最大化按钮以打开一个用于生成计算的大型编辑窗口。 完成后，单击最小化以继续处理自定义表单。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月14日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#grant" class="MCXref xref" xrefformat="{para}">使用访问级别授予团队访问权限</a> </p> <p>“访问级别”区域中新增了一个部分，通过该部分可以更精细地控制管理用户对团队的访问权限。 现在，您可以确定谁可以创建、编辑和查看团队。</p> <p>这不会更改用户对团队的现有访问权限。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#group" class="MCXref xref" xrefformat="{para}">Blueprint中现已提供组映射</a> </p> <p>现在，某些Blueprint包括组，您可以在安装Blueprint之前对其进行自定义。 您可以将Blueprint中的组映射到Workfront实例中的现有组，或根据需要创建新组。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#blueprin" class="MCXref xref" xrefformat="{para}">Blueprint公司映射和其他增强功能</a> </p> <p>现在，一些蓝图包括公司，在安装蓝图之前，您可以对其进行自定义。 您可以将Blueprint中的公司映射到Workfront实例中的现有公司，或根据需要创建新公司。</p> <p>Blueprint的其他增强功能也可用。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月11日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#view" class="MCXref xref" xrefformat="{para}">查看有关状态和公司的审核日志信息</a> </p> <p>现在，您可以通过在“设置”的“审核日志”区域中查看与状态和公司有关的信息，更轻松地对涉及状态和公司的事件进行故障诊断。</p> <p>例如：</p> 
    <ul> 
     <li> <p>您可以查找谁重命名、锁定或隐藏了状态，以及他们何时重命名、锁定或隐藏状态。</p> </li> 
     <li> <p>您可以了解从公司中删除某些成员或职务角色的人员，以及他们何时删除了这些角色。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月3日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#manage" class="MCXref xref" xrefformat="{para}">更轻松地管理公司成员资格</a> </p> <p>在“公司”区域中，更新的工具栏可以轻松地向公司添加现有Workfront用户，并删除公司成员。 </p> <p>以前，这些操作仅在“编辑公司”框中可用。</p> <p>更新后的工具栏还包含之前工具栏中可用的所有操作，例如编辑成员的用户配置文件信息并在系统中取消激活它们。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月4日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#groups" class="MCXref xref" xrefformat="{para}">组可以配置自己的时间表和小时首选项</a> </p> <p>在大型组织中，某些组可能需要独立配置工时单和小时首选项以适合其独特工作流，而不是继承由系统级别的管理员配置的首选项。 现在，Workfront管理员可以解锁系统中所有组的工时单和小时首选项，以便他们可以自行配置。</p> <p>最近还为项目首选项以及任务和问题首选项添加了此功能。 </p> </td> 
   <td> <p><b>在以下日期可用：</b> </p> <p>预览版本： 2021年9月9日<br></p> <p>生产版本： 2021年11月8日 <span style="color: #ff0000;">(此功能仅在生产中提供给具有21.4版本的群集4上的客户；它于2021年11月8日在生产中可用于所有其他集群。)</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#select2" class="MCXref xref" xrefformat="{para}">选择要解锁或重新锁定组的多个通知</a> </p> <p>现在，可以更快、更轻松地解锁或重新锁定群组的电子邮件通知。 现在，您可以选择多个通知，检查您的选择以确保它们正确无误，然后单击工具栏中显示的新“解锁”或“锁定”按钮。</p> <p>以前，您必须一次解锁和重新锁定一个通知。 Workfront目前有95条通知，因此，如果您必须为所有通知或许多通知执行此操作，则需要一段时间。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月14日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-admin-enhancements.md#for" class="MCXref xref" xrefformat="{para}">对于组管理员：在删除群组时更便于选择替换群组</a> </p> <p>删除组时，通过“删除组”框中的两项改进，可以更轻松地选择要保留已删除组的用户、工作项和子组的替换组：</p> 
    <ul> 
     <li> <p>您可以开始键入组的名称以快速找到它。 </p> </li> 
     <li> <p>您可以使用新信息图标确保选择所需的替换组。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月14日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
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
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">共享文档文件夹</a> </p> <p>现在，您可以从“文档”区域共享文档文件夹及其内容。 以前，这是不可能的，您必须单独共享文件夹中的每个文档。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月16日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#limit" class="MCXref xref" xrefformat="{para}">限制向您共享的模板添加文档的功能</a> </p> <p>有时，人们会将文档添加到项目模板，以为他们会将文档添加到项目中。 现在，您可以帮助防止出现这种情况 — 当您共享具有“查看”访问权限的模板时，可以禁用新的高级设置“添加文档”。 这会禁用收件人向模板添加文档的功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月14日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#update" class="MCXref xref" xrefformat="{para}">更新了功能板列表和功能板报表中的工具栏</a> </p> <p>现在，四个功能板页面上的工具栏具有与其他Workfront列表（如项目、任务和问题）匹配的现代外观。 现在，这个直观的工具栏可以更轻松地添加、编辑、共享、复制和删除功能板。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月8日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#add" class="MCXref xref" xrefformat="{para}">添加和编辑自定义表单文档的“摘要”面板</a> </p> <p>现在，您可以直接在文档摘要面板中添加和编辑自定义表单。</p> <p>通过此更改，您还将在文档“摘要”中看到新的外观。 新增了“概述”部分，其中包含图像缩略图和文档详细信息。 您还可以在文档详细信息部分中签入和签出文档。</p> <p>以前，必须转到“文档详细信息”中的“自定义表单”选项卡，才能编辑或添加自定义表单。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月18日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#filter" class="MCXref xref" xrefformat="{para}">在敏捷展示板上按用户列表进行筛选时，会显示最先具有大部分分配的用户</a> </p> <p>现在，过滤器会首先显示分配最多的用户，以便无需滚动列表即可更轻松地找到这些用户。</p> <p>以前，看板和清理板上按用户列表进行过滤时，会按字母顺序显示。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月11日 <br></p> <p>生产版本：在2.1版本中 <b style="color: #ff0000;">(已从22.1版本中删除。 不再在“预览”中可用。)</b></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#change" class="MCXref xref" xrefformat="{para}">在复制或移动任务时更改前置任务的默认选项</a> </p> <p>为了在复制或移动任务时最大限度地减少手动步骤的数量，我们更新了默认情况下随任务复制或移动的信息。 现在，所有前置任务都会默认随任务一起复制或移动，因为默认情况下会选择所有前置任务选项。 </p> <p>在此增强之前，在复制或移动任务时，默认情况下会取消选择所有前置选项。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new" class="MCXref xref" xrefformat="{para}">复制一个或多个任务时的新体验</a> </p> <p>为了让您使用Workfront与新的Adobe Workfront体验保持一致，我们在复制任务时重新设计了界面。 当前，在任务级别复制任务或在列表中复制一个或多个任务时，此功能可用。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月18日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">从列表中移动一个或多个任务时的新体验</a> </p> <p>为了在执行同一任务时提供一致的体验，我们现在更新了界面，以便在任务级别移动任务时从列表中移动一个或多个任务以匹配体验。 （我们更新了上一个“预览”版本中在任务级别移动任务的体验。）</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月4日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">在任务级别移动任务时的新体验</a> </p> <p>为了使您对Workfront的使用与新的Workfront体验保持一致，我们重新设计了用于移动任务的界面。 当前在任务级别移动任务时，此功能可用。 在以下版本中，我们将扩展此重新设计以从列表中移动任务。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年10月21日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">在问题级别使用模板将问题转换为项目时的新体验</a> </p> <p>为了使您对Workfront的使用与新的Workfront体验保持一致，我们重新设计了界面，在您从问题页面将问题转换为项目时，使用模板将问题转换为项目。</p> <p>现在，在选择以转换问题后，您可以更轻松地立即访问收藏列表。</p> <p>重新设计的界面与我们最近更新的模板创建项目时的体验相匹配。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月8日<br></p> <p>生产版本：在2.1版本中 <span style="color: #ff0000; font-weight: bold;">(此功能于2022年3月4日从生产环境中暂时删除。 后来从2022年4月28日开始分阶段推出。 推广工作于2022年5月5日完成。 现在，该功能在预览和生产中可供所有客户使用。)</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">使用列表、报表和功能板中的模板将问题转换为项目</a> </p> <p>为了提高工作效率并更便于您在快节奏环境中转换问题，我们添加了使用列表、报表或功能板中的模板将问题转换为项目的功能。</p> <p>在进行此增强之前，仅当您从问题页面转换了问题时，才存在此功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月8日<br></p> <p>生产版本：在2.1版本中 <span style="color: #ff0000; font-weight: bold;">(此功能于2022年3月4日从生产环境中暂时删除。 后来从2022年4月28日开始分阶段推出。 推广工作于2022年5月5日完成。 现在，该功能在预览和生产中可供所有客户使用。)</span></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">改进了“设置”面板，以及在负载平衡器中对项目及其任务进行颜色代码的功能</a> </p> <p>为了改善您在使用工作负载平衡器时的体验，我们引入了以下增强功能：</p> 
    <ul> 
     <li> <p>重新设计了“设置”面板，以包含以前位于工具栏中的选项。 这样可改进工具栏中空间的使用。</p> </li> 
     <li> <p>添加了按项目自定义颜色主题的功能。 在按项目选择颜色代码时，每个项目及其工作项将以相同的颜色显示。 每个项目的颜色各不相同。 在进行此增强之前，您只能按项目状态进行颜色代码。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">使用工作负载平衡器批量分配工作</a> </p> <p>在我们继续努力弃用计划工具并用负载平衡器替换这些工具时，我们增加了批量管理分配的功能。 现在，您可以一次将多个工作项分配给多个用户，将多个工作项中的用户替换为其他用户，以及一次从多个项目中取消分配用户。 通过使用工作负载平衡器中新的批量分配功能，您可以通过一个操作来执行所有这些操作。</p> <p>在此增强之前，您只能手动或通过拖放方式将一个用户分配给一个工作项。</p> <p>除了“名称”之外，新的“批量分配”还包含按“项目”和“任务状态”划分的新筛选功能。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-resource-mgt-enhancements.md#override" class="MCXref xref" xrefformat="{para}">管理作业角色时覆盖货币</a> </p> <p>为了帮助您轻松管理跨全球组织的成本和计费率，我们实施了凌驾于职务职位货币之上的政策。 使用此功能，您现在可以使用与职务角色位置匹配的币种设置职务角色的成本和开单费率。 这将覆盖任务角色的所有财务计算中的系统货币。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
 </tbody> 
</table>

### 请求增强功能 {#requests-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>功能</strong> </p> </td> 
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#interfac" class="MCXref xref" xrefformat="{para}">改进了无权创建请求的用户的界面</a> </p> <p>为了改善用户在处理请求时的体验，我们对界面进行了改进，以指示登录用户无权创建请求。 通过这项改进，对于无权创建问题的用户，“新建请求”按钮将变暗。 将鼠标悬停在灰显按钮上会显示工具提示，说明Workfront管理员限制了当前用户创建请求的访问权限。 </p> <p>在进行此增强之前，“新建请求”按钮未显示在这些用户的“请求”区域中。 复制和提交新请求也受到限制。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：2021年12月2日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#copy" class="MCXref xref" xrefformat="{para}">复制和提交请求</a> </p> <p>为了优化您提交请求的流程，我们引入了新功能，允许您复制现有请求并将其作为新请求提交。 当您经常提交类似请求时，这非常有用。 在这种情况下，您可以重复使用现有请求，进行一些更改，然后作为新请求提交。</p> <p>根据这项更改，可以查看其他人提交的请求的用户也可以复制这些请求并将其作为新请求提交。 您可以通过更新请求队列项目中的以下设置来阻止这种情况发生：来自同一公司的人员将继承所有请求的相同权限。</p> <p>在发布此功能之前，您无法复制并重新提交已提交到请求队列的问题，而没有队列主题。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月18日 <br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-requests-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">更新了“请求”区域“已提交”部分的“摘要”面板体验</a> </p> <p>为了提高“摘要”面板的可见性和与“摘要”面板的交互性，我们在“请求”区域的“已提交”部分的“打开摘要”图标中添加了标签。 标签现在为动态标签，它会根据面板是打开还是关闭进行更新。 </p> <p>在未首先选择请求的情况下打开“摘要”面板时，现在会显示一个更加用户友好的图像，以明确指示用户在打开面板之前选择项目。 </p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年11月4日<br></p> <p>生产版本：在2.1版本中 </p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
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
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">改进了审阅人和请求人的校对功能</a> </p> <p>为了在Workfront和Proof之间提供更加集成的体验，我们在审阅人和请求人的校对功能方面进行了多项改进：</p> 
    <ul> 
     <li> <p>您可以向Workfront中的任何用户授予审核者或作者角色，而不管这些用户是否具有校对许可证，都可以为他们授予其他权限，例如应用操作或解析注释。</p> </li> 
     <li> <p>您可以将审阅人和请求人添加到需要登录或需要以电子方式签名的校样中。</p> </li> 
     <li> <p>所有用户还可以从Workfront与Proof之间改进的连接中受益。 现在，在停用用户或更新用户的电子邮件地址时，当在Workfront中更改时，校样中会正确反映您的更新。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日 <b style="color: #ff0000;">(仅适用于具有集成校样的EMEA客户；（2022年1月17日可供所有剩余客户使用）</b><br></p> <p>生产版本： 2021年12月21日 <b style="color: #ff0000;">(仅适用于具有集成校样的EMEA客户；（适用于所有剩余客户）</b><br></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#electron" class="MCXref xref" xrefformat="{para}">验证的电子签名增强功能</a> </p> <p>我们为用户提供了电子校样的签名。 现在，用户可以使用其Workfront凭据来签署校样决策。</p> <p>要使用SSO凭据以电子方式对校样进行签名，您必须在Workfront校样中设置SSO。 </p> <p>以前，用户必须使用Workfront校样凭据，这些凭据与其Workfront凭据不同。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日 <b style="color: #ff0000;">（适用于EMEA和美国客户）</b><br></p> <p>生产版本：待定 <b style="color: #ff0000;">(2021年12月21日面向EMEA地区的客户；2022年2月3日可供所有其余客户使用)</b></p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-proofing-enhancements.md#desktop" class="MCXref xref" xrefformat="{para}">桌面查看器升级</a> </p> <p>我们已升级了桌面校对查看器，使其最高支持Chrome版本91，以增强与交互式校样的兼容性。</p> <p>Windows用户必须手动重新安装桌面查看器才能升级到最新版本。 之后，将自动更新桌面校样查看器。</p> <p>Mac用户将自动升级到最新版本。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：不适用<br></p> <p>生产版本： 2021年12月2日</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
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
   <td> <p><strong>发行日期和环境</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">“用户”列表的新工具栏</a> </p> <p>更现代、更直观的工具栏更便于在用户列表中管理用户。 利用工具栏按钮，可快速将人员添加到Workfront、提醒他们注册和管理其配置文件。 您还可以导出用户列表。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月8日<br></p> <p>生产版本：在2.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#default" class="MCXref xref" xrefformat="{para}">“计划完成日期”的默认升序以及按“主工作列表”中的“计划开始日期”分组的功能</a> </p> <p>为了更方便、更快地查找需要您注意的项目，我们添加了两项增强功能，允许您在默认情况下看到工作列表顶部显示最早到期的项目，并按计划开始日期对任务和问题进行分组。 </p> <p>在进行这些增强之前，您只能按计划完成日期和提交日期对项目进行分组。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日<br></p> <p>生产版本：在2.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#add" class="MCXref xref" xrefformat="{para}">为所有授权用户添加“我的更新”区域</a> </p> <p>为了在Workfront Classic与新的Workfront体验之间实现对等，我们为所有用户重新引入了“我的更新”区域。</p> <p>作为本次更新的结果，审核用户可以找到此区域作为其默认登录页面，除非将他们分配到布局模板。</p> <p>Workfront或组管理员可以使用布局模板将此区域添加到所有用户的“主菜单”和“顶部”导航中。</p> <p>现在，当您打开“我的更新”区域时，您可以快速找到以下信息：</p> 
    <ul> 
     <li> <p>等待您决策的批准将显示在“我的更新”页面的上半部分。 您可以批准、拒绝、建议更改、授予访问权限或将您的批准委派给其他人。</p> </li> 
     <li> <p>其中包含您的评论显示在“我的更新”页面下半部分的“提及次数”部分。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日<br></p> <p>生产版本：在2.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#improvem" class="MCXref xref" xrefformat="{para}">工时单改进</a> </p> <p>为了改善在Workfront管理时间的每个人的体验，我们将对时间表进行各种更新。</p> <p>其中一些更新包括：</p> 
    <ul> 
     <li> <p>当用户拥有当前工时单时，“工时单”区域现在会打开到当前工时单，以节省搜索和单击当前工时单的时间。 当没有当前工时单时，“工时单”区域仍显示“我的工时单”部分，就像今天一样。</p> </li> 
     <li> <p>将鼠标悬停在或您单击进入的行上以进入时间，该行会突出显示以提高可见性。</p> </li> 
     <li> <p>现在，包含时间表按钮的页脚具有粘滞性，这样您就可以始终访问保存和取消页面，而无需滚动到页面底部。 我们在此区域中还添加了一个新的“返回到顶部”按钮，以快速返回到页面顶部。</p> </li> 
     <li> <p>现在，新的警告通知会提醒您未保存的更改，以防止您在离开时间表时丢失信息。</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本： 2021年12月2日<br></p> <p>生产版本：在2.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> <p>Adobe Workfront Classic(<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic将于2022年3月终止</a>，紧随其后的是2022年7月Workfront Classic的生命周期终止日期。)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-other-enhancements.md#updated" class="MCXref xref" xrefformat="{para}">更新了“帮助”菜单</a> </p> <p>现在，当您单击顶部导航栏中的“帮助”链接时，会显示更新、更简化的菜单。 新菜单提供了相同的信息，但导航级别较低，需要较少的点击才能查看相关内容。</p> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：不适用<br></p> <p>生产版本：在2.1版本中</p> <p><strong>可在以下环境中使用：</strong> </p> <p>新的Adobe Workfront体验 </p> </td> 
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
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-mobile-enhancements.md#enhancem" class="MCXref xref" xrefformat="{para}">增强了移动设备应用程序中的校样功能</a> </p> <p>在Adobe Workfront移动应用程序中，您现在可以：</p> 
    <ul> 
     <li> <p>与内部和外部收件人共享校样</p> </li> 
     <li> <p>查看校样注释</p> </li> 
     <li> <p>下载校样</p> </li> 
    </ul> </td> 
   <td><strong>在以下日期可用：</strong> <p>预览版本：不适用<br></p> <p>生产版本：2022年2月初</p> <p><strong>可在以下环境中使用：</strong> </p> <p>iOS移动应用程序</p> <p>Android移动设备应用程序</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion增强功能

在22.1版本计划之外，Workfront Fusion的新增功能会在生产环境中以一定频率提供。 有关最新功能的更多信息，请参阅 [Adobe Workfront Fusion版本活动](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Workfront Scenario Planner增强功能

此时版本中没有方案计划员更新。 此区域将在更新可用时进行更新。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof增强功能

Workfront校样中的新增功能现已可用。 有关更多信息，请参阅 [Workfront Proof发行活动：2021年11月29日一周](../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md).

## Workfront目标增强功能

此时，版本中没有Workfront Target目标更新。 此区域将在更新可用时进行更新。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API版本14

对于API版本14，我们修改了一些资源和端点。 某些更改支持新功能，而其他更改则使您能够更轻松地使用通过API提供的信息。

有关新增功能和更新功能的信息，请参阅 [API版本14的新增功能](../../../wf-api/api/new-api-version-14.md).

有关API版本的信息，请参阅 [API版本控制和支持计划](../../../wf-api/api/api-version-support-schedule.md).

## Workfront 维护更新

有关22.1版本期间进行的维护更新的信息，请参阅 [Workfront维护更新](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## 22.1版网络研讨会

Workfront 22.1版网络研讨会于2022年1月12日召开。 您可以在 [Workfront One上的事件页面](https://one.workfront.com/s/event).

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

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关更多信息，请参阅 [培训版本更新页面](https://one.workfront.com/s/training-release-updates).

## 不再支持的功能

### Internet Explorer 11

由于移除了对Internet Explorer的支持，Workfront现在正式支持Microsoft Edge。

有关支持的浏览器的更多信息，请参阅 [Adobe Workfront浏览器要求](../../../workfront-basics/workfront-browser-requirements.md).
