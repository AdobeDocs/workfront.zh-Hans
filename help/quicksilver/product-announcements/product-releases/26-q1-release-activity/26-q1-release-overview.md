---
title: 2026年第一季度发行版概述
description: 本页介绍了2026年第一季度版本中包含的功能。 这些增强功能计划本季度在“生产”环境中提供。
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 8d177d1081590f6a6733f29e0d615828394394c7
workflow-type: tm+mt
source-wordcount: '2886'
ht-degree: 1%

---

# 2026年第一季度发行版概述

本页介绍了计划于2026年1月发布的2026年第一季度版本中包含的功能。

此页面上的增强功能在“预览”环境中可用。 在2026年第一季度版本接近其计划发布的生产版本时，此页面将进行额外的增强。


<!-- Keep commented until Final Preview release.

The <add release> release webinar will be held on <date>. You can [register for the webinar here <get link from product ops>. -->

>[!IMPORTANT]
>
>
>除非另有说明，否则每月和季度发行计划于当月第二整周的星期四提供。
>
>| 每月发布 | 季度发布 |
>|----|----|
>| <ul><li>25.11（2025年11月13日）</li><li>25.12（2025年12月11日）</li><li>26.1（2026年1月14日）</li></ul> | <ul><li>26.1（2026年1月15日）</li></ul> |
>
>请注意，对于每季度的最终版本（本季度26.1版），按照快速发布计划的用户将提前一天收到版本（2026年1月14日）。
>
>有关快速发布过程的详细信息，请参阅[启用或禁用快速发布过程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [文档和审批增强功能](#documents-and-approvals-enhancements)
* [主页增强功能](#home-enhancements)
* [集成增强功能](#integration-enhancements)
* [项目增强功能](#project-enhancements)
* [报表增强功能](#reporting-enhancements)
* [请求增强功能](#requests-enhancements)
* [其他增强功能](#other-enhancements)

### 管理员增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">管理布局模板中的优先级</a>
            <p><span class="preview">在预览环境中暂时不可用</span></p>
            <p>您现在可以在布局模板中启用或禁用特定用户的优先级。 如果之前已为您的组织禁用了优先级，则进行此更改后，布局模板中将保持禁用状态。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2025年1月14日</td>
        <td>2025年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">检查已计算的自定义字段是否存在多表单冲突</a>
            <p>为了能够查看在自定义字段上编辑表达式时可能受影响的对象，我们添加了一个用于检查冲突的选项。 此对话框显示可能受更改公式影响的所有对象，按对象类型分组。 您可以导航到每个对象的详细信息并查看字段，以确定是应从任何表单中删除字段还是表达式应保持不变。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2025年1月14日</td>
        <td>2025年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">输入日期和输入者ID存储在自定义对象中</a><p>[!BADGE Off Schedule]{type=Neutral}</p>
            <p>输入日期和按ID输入的内容现在存储在自定义表单、字段和部分中。 您可以在报表中将这些数据选项用作过滤器、视图或分组。 要在“设置”中的自定义表单、字段或节列表中显示它们，请添加“输入日期”和“输入者：名称”作为新视图或现有视图中的列。</p>
        </td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
    </tr>  
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">编辑布局模板时更新按钮名称</a>
            <p>为了与“设置”的其他区域（如自定义表单设计器）更加一致，您在编辑布局模板时看到的按钮已更改为“应用”、“保存并关闭”和“取消”。 新选项“应用”允许您保存对布局模板所做的更改并继续编辑。 以前，可用的选项为“保存”和“取消”。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>  
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-admin-and-setup.md" class="MCXref xref" xrefformat="{para}">自定义字段上使用活动标志改进了字段管理</a>
            <p>当系统中具有大量自定义字段时，在自定义表单和报告中管理这些字段可能比较困难。 您现在可以使用新的<b>活动</b>标志将自定义字段标记为不活动。 在自定义表单中使用字段，或者从“字段”列表添加或编辑字段时，此标志可用。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 文档和批准增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
        </tr>
       <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Set up brands for the AI reviewer in Workfront<p>[!BADGE Off schedule]{type=Neutral}</p> </a>
            <p>You can now set up brands for the AI reviewer in the Workfront Setup area. This allows you to customize the AI review process based on your organization's branding guidelines.</p>
            <p>The AI reviewer is currently in beta.</p>
        </td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
        <td>January 8, 2026</td>
    </tr> -->
    </tr>
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">在Adobe Express中发送审阅时选择Workfront项目<p>[!BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>您可以选择要向其发送验证的Workfront项目。 这有助于将所有相关的资源和验证组织在同一项目中。</p>
        </td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
    </tr> 
     <tr>
        <td>
            对具有Workfront校对的Adobe Express的<a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">跨组织支持<p>[!BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>我们正在引入对具有Workfront Proofing的Adobe Express的跨组织支持。 此增强功能允许跨多个IMS组织运营的客户无缝使用和管理验证工作流。</p>
        </td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
        <td>2025年11月13日</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-documents-approvals.md" class="MCXref xref" xrefformat="{para}">Adobe Experience Manager现在可与Frame.io集成一起使用 <p>[!BADGE Off Schedule]{type=Neutral}</p> </a>
            <p>现在，您可以使用Experience Manager Assets​管理和存储已经过审核和批准周期的数字资源。 此集成允许您利用Adobe Experience Manager、Frame.io和Workfront的功能来简化内容管理和协作流程。 </p>
        </td>
        <td>2025年10月30日</td>
        <td>2025年10月30日</td>
        <td>2025年10月30日</td>
    </tr>   
  </tbody>
</table>



### 主页增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-home.md" class="MCXref xref" xrefformat="{para}">更新到主页中的提及小组件</a>
            <p>我们已对主页中的“提及”小组件进行以下改进： <ul><li>在大多数Workfront对象的更新区域中，相同的体验现在也可在主页中的提及小组件中获得。 </li><li>“提及次数”小组件现在包含用户在过去两周内发表或标记为的评论</li><ul></p>
        </td>
        <td>2025年12月17日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 集成增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">在Creative Cloud Express中发送审核时选择Workfront项目</a><p>[!BADGE Off Schedule]{type=Neutral}</p>
            <p>您可以选择要向其发送验证的Workfront项目。 这有助于将所有相关的资源和验证组织在同一项目中。 </p>
        </td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
        <td>2025年12月15日</td>
    </tr>   
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">已为Experience Manager Assets本机集成更新Adobe Workfront的资源选择器</a>
            <p>我们已在Adobe Workfront中为Experience Manager Assets集成升级了资源选择器。 通过此升级，您现在可以选择并将AEM收藏集直接拉入Workfront。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
    </tr>   
    <!-- <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-integrations.md" class="MCXref xref" xrefformat="{para}">New version of Salesforce integration now available </a>
            <p>To stay up-to-date with recent changes to the Workfront API, we've created a new Salesforce integration. The new integration features the same functionality as the previous version, and was updated to avoid losing functionality deprecated in the API.</p><p>NOTE: The Workfront for Salesforce integration, including the new version, will not be available after **February 28, 2026**. </p>
        </td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
        <td>October 30, 2025</td>
    </tr>   -->
  </tbody>
</table>

### 项目增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
         <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-projects.md" class="MCXref xref" xrefformat="{para}">轻量级用户可以登录项目</a>
            <p>轻量级用户现在可以直接在项目上记录时间。 以前，只有Standard许可证用户可以在项目上记录小时数。</p>
        </td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 报表增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
 <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">画布功能板中的货币更新</a>
            <p>我们对货币字段进行了以下更新：<ul><li>在Workfront中定义多种货币后，您现在可以在创建过程中为功能板选择默认货币。 </li><li>创建报告时，您可以锁定货币字段。 这可确保仪表板级别的货币首选项不会影响这些值的显示。</li><li>查看功能板时，用户可以在Workfront中定义的任何货币之间进行切换。 这些更改适用于整个仪表板，但锁定的货币字段除外</li></ul></p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
 <tr>
        <td>
            画布仪表板中的<a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">快速搜索表结果</a>
            <p>我们在表格报表中添加了快速搜索。 此搜索适用于所有页面，因此即使数据当前不可见，您也可以找到数据。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">新的饼图显示总计选项</a>
            <p>我们引入了一个新的“显示总计”选项，该选项可将饼图转换为圆环图。 此功能允许用户显示一个中心值，代表图表中所有区段的总数。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">画布仪表板中饼图的新配置选项</a>
            <p>我们为饼图引入了两个新的配置选项： <ul><li>隐藏区段标签：现在，您可以选择在饼图上隐藏区段标签（如果区段标签太长并影响图表可读性）。</li><li>隐藏和重新定位图表图例：您现在可以选择隐藏饼图图例。 您还可以将图例的位置设置为图表的右侧（默认）、左侧、顶部或底部。 </li></ul></p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">画布功能板分组计数改进</a>
            <p>我们更新了画布仪表板中的分组栏，以显示当前页面的记录计数以及跨所有页面的分组的整体记录计数。 </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">画布功能板报告中的新参考线功能</a>
            <p>现在，您可以在条形图、柱形图和折线图中定义参考线，以设置基于系列报表的目标或阈值。 </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">自定义画布仪表板中图表报表的轴标签</a>
            <p>您现在可以自定义图表报表上的轴标签。 此新功能允许您输入要显示的替换轴标签，而不是默认对象和字段路径。 此外，您可以选择完全隐藏轴标签。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">在画布仪表板中复制报告</a><p>[!BADGE Off Schedule]{type=Neutral}</p>
            <p>现在，您可以在创建KPI、表或图表报表后，将其复制到画布仪表板中。 复制后，您可以在保存之前根据需要编辑报表。</p>
        </td>
        <td>2025年10月23日</td>
        <td>2025年10月23日</td>
        <td>2025年10月23日</td>
    </tr>   
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">正在从报告筛选器中删除字段选项</a>
            <p>我们删除了以下之前在将过滤器应用于报表时可用的字段选项：
            <ul>
            <li>其他组ID</li>
            <li>其他角色ID</li>
            <li>其他团队ID</li>
            </ul>
            </p>
        </td>
        <td>2025年11月6日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>    
       <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-reporting.md" class="MCXref xref" xrefformat="{para}">新护栏可缩短画布仪表板中的加载时间</a>
            <p>为了避免加载时间延迟并提高画布仪表板中的整体性能，我们对可以向仪表板添加多少仪表板组件施加了限制：
            <ul>
            <li>每个仪表板的报表数：25个限制</li>
            <li>表视图上的分组：5个限制</li>
            <li>与报表的基本对象的距离：10限制</li>
            <li>表格视图中的列：25个限制</li>
            <li>仪表板级别筛选器提示： 10次限制</li>
            </ul></p>
        </td>
       <td>2025年11月6日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
    </tr>   
  </tbody>
</table>

### 请求增强功能

<table style="table-layout:auto">
  <tbody>
   <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">已创建的对象链接现在可在“请求”区域和“我的请求”小组件中使用</a>
            <p>为了让您更轻松地转到由特定请求创建的对象，我们添加了指向“已创建对象”列的链接。 现在，您可以单击此列中的链接以直接转到所创建对象的页面。/p&gt;
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <!--<tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">Create groupings in the Requests list and My Requests widget</a>
            <p>To make it easier for you to find the requests you need, we've added groupings to the Requests list and the My Requests widget. Now, you can group requests by any column on the list. These groupings become part of the view that you are using when you create the grouping.</p>
        </td>
        <td>December 18, 2025</td>
        <td>January 14, 2026</td>
        <td>January 15, 2026</td>
    </tr> -->
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">将自定义字段添加到请求列表和我的请求小组件</a>
            <p>为了更便于您查看所需信息，我们添加了将自定义字段作为列添加到请求列表和我的请求小组件（位于主页）的功能。 现在，您可以从自定义表单中将字段添加为列，并且该字段中有信息的请求将在列表或小部件中显示该信息。</p><p>此功能仅在新的请求体验中可用。</p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">当前用户通配符在请求筛选器中可用</a>
            <p>为了更便于筛选适用于您的请求，我们创建了一个当前用户通配符。 现在，在筛选时，您可以选择“我（已登录用户）”。 该过滤器随后将应用于正在查看请求列表的用户。   </p>
        </td>
        <td>2025年12月18日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">由AI提供支持的Form Fill现在可用于请求</a>
            <p>为了更便于创建请求，我们创建了由AI提供支持的表单填写。 现在，您可以粘贴提示或将文档上传到请求表单，AI将提取相关信息并填写表单。  </p>
        </td>
        <td>2025年12月11日</td>
        <td>2025年12月11日</td>
        <td>2025年12月11日</td>
    </tr> 
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">在“请求”区域和“我的请求”小组件中共享视图</a>
            <p>为了更便于确保查看您需要的信息，我们添加了将视图共享到新报告体验的功能。 现在，您可以与其他用户、团队或组共享视图。 </p>
        </td>
        <td>2025年12月4日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr> 
     <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">将请求草稿保存在新的请求体验中</a>
            <p>为了更便于创建和提交请求，我们添加了将草稿保存到新请求体验的功能。 现在，当您开始填写并关闭请求时，请求将保存为草稿状态，并可在用于创建草稿的请求表单上找到。 之后，您可以随时重新打开、更新和提交草稿。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>  
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">删除新请求体验中已提交的请求</a>
            <p>为了更便于保持请求的组织性和整洁，我们向新的请求体验添加了删除请求的功能。 现在，您可以删除已提交的请求。 Workfront管理员和Workfront Planning Workspace管理员也可以删除请求。</p>
        </td>
        <td>2025年11月20日</td>
        <td>2026年1月14日</td>
        <td>2026年1月15日</td>
    </tr>   
        <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-1-q1-requests.md" class="MCXref xref" xrefformat="{para}">通过复制新请求体验中先前提交的请求来创建新请求</a>
            <p>为了更便于提交请求，我们添加了将请求复制到新请求体验的功能。 现在，您可以复制请求、编辑任何字段并将其作为新请求提交。 </p>
        </td>
        <td>2025年11月20日</td>
        <td>2025年12月11日</td>
        <td>2026年1月15日</td>
    </tr>    
  </tbody>
</table>

### 其他增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 25%;" />
            <tbody>
               <tr>
        <td><strong>功能</strong>
        </td>
        <td><strong>预览</strong></td>
        <td><strong>快速发布</strong></td>
        <td><strong>每季度</strong></td>
    </tr>   
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">在2026年第一季度发布时间范围内的外观更新</a>
                        <p>在2026年第一季度发布时间范围内，对Adobe Workfront应用程序各个区域的外观和工作方式进行了小幅更新。 </p>
                    </td>
                    <td><p>在整个2026年第一季度发布时间范围内<br /></p>
                    <td colspan="2"><p>快速发布：发布到“预览”后至少1周（除非另有指定）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                 <td>
                <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">多选字段的选择限制</a>
              <p>现在，当用户填写表单时，允许进行多选择的字段（例如复选框和多选下拉列表）限制为5000个选择。</p>
             </td>
        <td>2025年10月30日</td>
        <td>2025年11月13日</td>
        <td>2026年1月15日</td>
             </tr>   
    <tr>
        <td>
            <a href="/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-other.md" class="MCXref xref" xrefformat="{para}">Adobe统一体验现在可供更多Workfront组织使用</a><p></p>
            <p>为了让组织能够访问Adobe Unified Experience的优势，我们将继续将其提供给现有的Workfront客户。</p>
        </td>
        <td><p>2025年12月11日</p></td>
        <td><p>2026年1月15日</p></td>
        <td><p>2026年1月15日</p></td>
    <tr>
            </tbody>
        </table>


### 即将从Workfront中删除的功能

#### 在25.11版本中弃用了工作角色上的覆盖货币

作为财务模型简化的一部分，我们将通过25.11版本在10月30日的“预览”和“生产”版中为所有客户弃用工作角色的覆盖货币。 此更改会影响货币和汇率在“设置”区域中的工作角色配置方式。

* 工作角色中的&#x200B;**覆盖货币**&#x200B;字段将不再可用。
* 每个工作角色将具有与其关联的成本和记帐费率的单一货币。
* 所有现有的覆盖货币及其汇率值将自动迁移以成为该工作角色的唯一货币和汇率。

## 界面现代化

我们正在更新整个Adobe Workfront中的界面，以改进用户体验并将其与其他Adobe应用程序相统一。 这些更改将在标准发布计划之外发布。 有关这些更改的列表，请参阅[接口现代化](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md)。

## 其他区域的发行说明

### Workfront Fusion增强

Workfront Fusion中的新增功能在标准发布计划之外的生产环境中提供。 有关最新功能的详细信息，请参阅[Adobe Workfront Fusion发行活动](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。

### Workfront规划增强功能

Workfront Planning中的新增功能已在生产环境中可用。 有关最新功能的详细信息，请参阅[Adobe Workfront计划的2026年第一季度发布活动](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-26-q1.md)。

在这个版本中，以下内容暂无更新：

* 场景计划器
* 校样
* 目标

## 桌面校对查看器更新

### 版本 2.1.54

**适用于所有客户的生产版本： 2025年12月11日**

桌面校对查看器已从2.1.52更新到2.1.54。此更新包括内部工具更新，不会影响最终用户功能。

2.1.53版本还包括内部工具更改。

此更新适用于Mac和Windows。

### 版本 2.1.52

**适用于所有客户的生产版本： 2025年7月31日**

桌面校对查看器已更新至版本2.1.52，该版本解决了错误修复问题。

2.1.51更新包括内部工具更新，不会影响最终用户功能。

此更新适用于Mac和Windows。

## 公告

### API版本21

Workfront API版本21于2025年10月23日发布。 对于API版本21，我们修改了一些资源和端点。 一些更改支持新功能，而其他更改使您能够更轻松地使用通过API获得的信息。

>[!IMPORTANT]
>
>此API版本更改具有可能影响现有API调用的重大更改。 这是由于API版本21使用事件订阅版本2。
>
> 对于多选字段，事件订阅版本2始终以数组形式发送。 如果选择了多个值，则版本1会发送一个数组。 如果只选择一个值，则会发送一个字符串。

有关新增功能和更新的信息，请参阅[API版本21](/help/quicksilver/wf-api/api/new-api-version-21.md)中的新增功能。

有关API版本的信息，请参阅[API版本控制和支持计划](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### 适用于Microsoft Teams的Workfront的新版本

由于[Microsoft将过渡到“新团队”客户端](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability)，因此Classic Teams客户端在2025年7月1日后将不再可用。 要继续使用Microsoft Teams和Workfront等集成应用程序，客户必须在此日期之前过渡到新团队客户端。

更新的Workfront集成现已可用，并与新团队体验完全兼容。 在大多数情况下，用户完成过渡后，Workfront会自动显示。 如果不包含，则可以从Microsoft Teams App Store手动安装集成。 若要在New Teams客户端中安装或验证Workfront集成，请参阅[安装 [!DNL Adobe Workfront] Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)。

### Workfront for Microsoft Outlook

[Microsoft正在禁用对旧版Exchange联机令牌](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens)的支持，Workfront Outlook加载项当前使用这些令牌进行身份验证。 Microsoft的这一更改已开始影响客户，并将在2025年10月之前继续分阶段推出。

* **在Microsoft完全禁用这些令牌后，Workfront for Microsoft Outlook集成将无法再正常使用。**

作为此更改的一部分，Microsoft已决定更改令牌的重新启用方式。 在&#x200B;**2025年6月30日**&#x200B;之后，管理员将无法再自行重新启用令牌 — 只有Microsoft支持部门可以授予例外。 **在2025年10月1日，将为所有租户关闭旧版令牌。 将不会授予例外。**

### 其他Workfront集成过渡

为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，以下集成在&#x200B;**2026年2月28日**&#x200B;之后不可用：

* Workfront for G Suite
* Workfront for Jira
* 适用于Salesforce的Workfront。

为了满足贵组织与Google Workspace的集成需求，我们建议使用Workfront自动化和集成。
有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。


### Workfront 维护更新

有关2025年第一季度版本中所做维护更新的信息，请参阅[Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=zh-Hans)。

### 培训更新

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关详细信息，请参阅[Workfront教程页面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=zh-Hans)的“新增功能”部分。
