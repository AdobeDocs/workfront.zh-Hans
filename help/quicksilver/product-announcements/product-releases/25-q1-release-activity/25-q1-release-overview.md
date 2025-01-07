---
title: 2025年第一季度发行版概述
description: 本页介绍了2025年第一季度版本中包含的功能。 这些增强功能计划本季度在“生产”环境中提供。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5bb898fa-d74e-4174-bc93-d8ffb8937680
source-git-commit: 5755894ff320db368d07a3ab3ff18bbc9e157e0a
workflow-type: tm+mt
source-wordcount: '2478'
ht-degree: 0%

---

# 2025年第一季度发行版概述

本页介绍了2025年第一季度版本中包含的功能。 这些增强功能计划本季度在“生产”环境中提供。

<span class="preview">周期外功能（在2025年第一季度发布日期之前发布到生产环境的功能）以黄色突出显示。</span>

>[!IMPORTANT]
>
>23.3版本包括将您的组织移至每月版本的选项。 因此，Workfront更改了版本的编号方案，以说明每月和每季度的版本跟踪。 第一个数字表示年份，第二个数字表示发布月份。 示例： 2025年4月的发行版本为25.4。
>
>除非另有说明，否则每月和季度发行计划于当月第二整周的星期四提供。
>
>| 每月发布 | 季度发布 |
>|----|----|
>| <ul><li>24.11（2024年11月14日）</li><li>24.12（2024年12月12日）</li><li>25.1（2025年1月15日）</li></ul> | <ul><li>25.1（2025年1月16日）</li></ul> |
>
>请注意，对于每季度的最终版本（本季度25.1版），按照快速发布计划排程的用户将提前一天收到版本。
>
>有关快速发布过程的详细信息，请参阅[启用或禁用快速发布过程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [展示板增强功能](#boards-enhancements)
* [文档管理增强功能](#document-management-enhancements)
* [主页增强功能](#home-enhancements)
* [项目增强功能](#project-enhancements)
* [校对增强功能](#proofing-enhancements)
* [报表和功能板增强功能](#report-and-dashboard-enhancements)
* [更新流增强功能](#update-stream-enhancements)
* [其他增强功能](#other-enhancements)

### 管理员增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
           在环境之间比较对象以进行环境升级</a></p>
            <p>为了更便于确定环境升级包中应包含哪个对象，我们添加了跨环境比较对象的功能。 然后，您可以从此比较中直接将对象添加到资源包。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年1月6日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            更多可用于环境升级的对象</a></p>
            <p>为了扩展环境升级功能的功能，我们添加了更多对象。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年1月6日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>  
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在记录小时数时阻止移动任务</a></p>
            <p>由于移动记录小时数的任务或问题有时会导致合规性或审核问题，因此我们在“设置”的“任务和问题首选项”区域中添加了一个首选项，该首选项允许您阻止用户在记录小时数的情况下移动任务和问题。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            用于单次分配任务的项目或用户计划的首选项</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>作为系统或组管理员，您现在有了一个新的首选项，当您为任务分配一个用户，并且项目和用户都关联到时间表时，指示Workfront是否应使用项目或用户的时间表计算项目的时间表。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月21日</li>
                <li>用于快速发布的生产：用于24.12版（2024年12月12日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>     
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            业务规则现在支持超链接</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>现在，您可以在业务规则的自定义错误消息中包含超链接，以指导用户如何在规则的限制内修改其操作。 静态URL可以链接到对用户有益的文档或其他页面。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月21日</li>
                <li>用于快速发布的生产：用于24.12版（2024年12月12日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            现在可对本机预输入字段进行筛选</a></p>
            <p>当您将本地字段引用添加到自定义表单并且它引用预输入字段(例如Portfolio、公司或所有者)时，筛选器选项现在可用。 该过滤器允许您限制用户在使用该字段时可以选择的对象。 此自定义筛选器的工作方式与自定义预输入字段上的筛选器的工作方式相同，使用文本模式定义筛选器。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月21日</li>
                <li>用于快速发布的生产：用于24.12版（2024年12月12日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-administrator-enhancements.md" class="MCXref xref" xrefformat="{para}">
            已将“移至”图标添加到自定义字段</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>当自定义表单包含多个具有许多字段的分区时，可能很难通过拖放方式将字段从一个分区移动到另一个分区。 每个字段都添加了“移至”图标，允许您选择字段所在的部分。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年10月29日</li>
                <li>用于快速发布的生产：用于24.11版（2024年11月14日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 展示板增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-boards-enhancements.md" class="MCXref xref" xrefformat="{para}">
            更改讨论区的所有者</a></p>
            <p>默认情况下，展示板的创建者是所有者。 讨论区所有者是唯一可以在“配置”面板中删除该讨论区或更新其筛选器的人员。</p>
            <p>添加了功能，以允许Workfront系统管理员更改展示板的所有者。 讨论区的当前所有者也可以更改该特定讨论区的所有者。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月18日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 文档管理增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            一次编辑多个文档</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>您现在可以一次编辑多个文档。 您可以编辑说明并更新自定义表单。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月21日</li>
                <li>用于快速发布的生产：用于24.12版（2024年12月12日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>    
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-document-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">
            可用于文档版本审批的新提取状态</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>将新版本添加到具有待审批的文档时，对先前版本的审批现在将显示为“已撤回”，这表示由于添加新版本，先前审批流程已关闭。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月7日</li>
                <li>用于快速发布的生产：用于24.11版（2024年11月14日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
            <p><i>此功能是分阶段发布的一部分，仅适用于特定客户。</i></p>
        </td>
    </tr>
</tbody>
</table>

### 主页增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在优先级中赶超工作</a></p>
            <p>您可以使用“跟上”来帮助缩短查找有关活动项目信息的时间。</p>
            <p>通过Workfront的AI助手，“即时查看”功能会在以下时间范围内对您项目的更新、上传的文档和其他显着更改进行汇总：24小时、3天或7天。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月20日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在优先级的“详细信息”页面上实时查看更改</a></p>
            <p>您现在可以在任务或问题的详细信息页面上查看实时更新。 您还可以通过实时在线状态指示器查看其他人是否与您同时查看页面。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在优先级中上传和查看文档和验证</a></p>
            <p>您现在可以与工作列表和日历中任务和问题的文档和验证进行交互。 在新的“文档”选项卡中，您可以</p>
            <ul>
                <li>上传文档</li>
                <li>创建验证</li>
                <li>启动验证查看器</li>
                <li>等等</li>
            </ul>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            日历视图现在可在“优先级”中使用</a></p>
            <p>您可以使用清晰可见的月份日历跟踪您的工作。 使用优先级日历，您可以</p>
            <ul>
                <li>使用筛选器查找您的工作</li>
                <li>应用状态和焦点级别等自定义字段以标识高优先级工作</li>
                <li>为快速组织应用颜色</li>
                <li>等等</li>
            </ul>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            “优先级”工作列表的更新</a></p>
            <p>我们更新了“优先级”工作列表，以改进功能并与应用程序的其他领域保持一致。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月12日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            从优先级导航到项目的详细信息页面</a></p>
            <p>您现在可以从优先级工作列表直接导航到Workfront中的项目。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月5日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            更新了“优先级”中“我的焦点”列中的选项</a></p>
            [！BADGE In Production ]{type=Informational}
            <p>我们更新了“我的焦点”列中的选项，以帮助您以更直观的方式排定工作的优先级并对工作进行排序。 新标签包括</p>
            <ul>
                <li>紧急</li>
                <li>高</li>
                <li>正常</li>
                <li>低</li>
            </ul>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月14日</li>
                <li><span class="preview">适用于所有客户的生产版本： 2024年11月14日</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-home-enhancements.md" class="MCXref xref" xrefformat="{para}">
            在优先级中查看项目详细信息</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>您现在可以在“优先级”的工作列表中查看项目详细信息和注释。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月6日</li>
                <li>用于快速发布的生产：用于24.11版（2024年11月14日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 项目增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            从快速发布环境的预览和生产中删除了更相关的分配</a></p>
            <p>自2023年12月起一直在“预览”环境中存在的功能以及自2024年3月起一直在“快速发布”的“生产”环境中存在的功能现已移除。 这些功能在分配任务时添加了更相关的智能分配建议。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 校对增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            测试版中提供了用于交互式审阅的新浏览器扩展</a></p>
            [！BADGE In Production ]{type=Informational}
            <p>我们将引入一个新的浏览器扩展Adobe Workfront审阅工具，以取代用于审阅交互式ZIP内容的旧版浏览器扩展。 新的Adobe Workfront审核工具支持跨所有常见浏览器审核ZIP内容。</p>
            <p>旧版浏览器扩展将于2025年2月28日删除。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月7日</li>
                <li><span class="preview">适用于所有客户的生产版本： 2024年11月7日</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 报表和功能板增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            仪表板中最多有25个报告、外部页面或日历</a></p>
            <p>为了保持仪表板性能，我们实施了可放置在仪表板中的报告、外部页面或日历的总数限制。 创建新仪表板时，最多可以添加25个项目。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月16日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-report-and-dashboard-enhancements.md" class="MCXref xref" xrefformat="{para}">
            用于Data Connect的首次读取器帐户创建按钮</a></p>
            [！BADGE In Production ]{type=Informational}
            <p>首次访问Data Connect的管理员现在可以选择通过单击单个按钮来创建新的Snowflake读取器帐户。 该过程需要几分钟才能完成，但无需执行进一步操作。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月14日</li>
                <li><span class="preview">适用于所有客户的生产版本： 2024年11月14日</span></li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 更新流增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><span class="bold">功能</span></p>
        </td>
        <td>
            <p><span class="bold">发行日期</span></p>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">
            更新了“主页”和“我的更新”区域中“提及”小组件中的评论体验</a></p>
            <p>我们正在主页的“提及次数”小组件和“我的更新”区域的提及次数部分中更新评论体验。 现在，在大多数Workfront对象的“更新”区域中，相同的体验也可在我的更新的“提及”小组件和“提及”部分中使用。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年12月19日</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
</tbody>
</table>

### 其他增强功能

<table>
<col style="width: 50%;" />
<col style="width: 50%;" />
<tbody>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            更新如何管理链接文件夹中移动或删除的资源</a></p>
            [！BADGE In Production ]{type=Informational}
            <p>在将Adobe Workfront与Experience Manager Assets和Assets Essentials集成使用时，我们更改了处理移动和删除资源的方式：</p>
            <ul>
                <li>已删除的资源：当在Assets或Assets Essentials中的链接文件夹内删除某个资源时，已删除的资源将保留在项目文档区域中。</li>
                <li>移动资源：当资源移到Assets或Assets Essentials中的链接文件夹之外时，移动的资源将保留在项目文档区域中。</li>
            </ul>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月21日</li>
                <li><span class="preview">适用于所有客户的生产版本： 2024年12月5日</span></li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            自定义表单中的部分现在可折叠和展开</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>将具有多个分区的自定义表单附加到对象时，您现在可以折叠和展开表单顶部默认分区以外的所有分区。 管理员也可以在表单设计器中预览表单时查看此功能。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年11月11日</li>
                <li>用于快速发布的生产：用于24.12版（2024年12月12日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-other-enhancements.md" class="MCXref xref" xrefformat="{para}">
            AI助手现在可以处理项目、任务和问题</a></p>
            [！BADGE In Production for Fast Release ]{type=Positive}
            <p>为了更便于在Workfront中管理您的工作项，我们更新了AI助手，以处理项目、任务和问题。 现在，AI助手可以根据您指定的标准找到项目、任务和问题。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本： 2024年10月31日</li>
                <li>用于快速发布的生产：用于24.11版（2024年11月14日）</li>
                <li>适用于所有客户的生产版本：使用25.1版本（2025年1月）</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>
            <p><a href="/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">
            在2025年第一季度期间的外观更新</a></p>
            <p>在2025年第一季度内，对Adobe Workfront应用程序各个区域的外观和工作方式进行了小幅更新。 查看各个发行说明以了解具体发行日期。</p>
        </td>
        <td>
            <p><b>在以下日期可用：</b></p>
            <ul>
                <li>预览版本：在整个2025年第一季度发布时间范围内</li>
                <li><span class="preview">生产版本：查看特定日期的发行说明</span></li>
            </ul>
        </td>
    </tr>                            
</tbody>
</table>

<!--
### Functionality soon to be removed from Workfront

The following functionality is soon to be removed from Workfront:
-->

## 公告

### Workfront Fusion增强

Workfront Fusion中的新增功能在2025年第一季度发布计划之外以一定节奏在“生产”环境中提供。 有关最新功能的详细信息，请参阅[Adobe Workfront Fusion发行活动](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)。

### Workfront规划增强功能

Workfront Planning中的新增功能已在生产环境中可用。 有关最新功能的详细信息，请参阅[Adobe Workfront计划2025年第一季度发布活动](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-25-q1.md)。

### Workfront Scenario Planner增强

此版本中目前没有Scenario Planner更新。 在有可用更新时，将更新此区域。

### Workfront Proof增强功能

此版本中目前没有Workfront Proof更新。 在有可用更新时，将更新此区域。

### Workfront目标增强功能

此版本中目前没有更新Workfront Goals。 在有可用更新时，将更新此区域。

### API版本19

对于API版本19，我们修改了一些资源和端点。 一些更改支持新功能，而其他更改使您能够更轻松地使用通过API获得的信息。

有关新增功能和更新的信息，请参阅[API版本19](/help/quicksilver/wf-api/api/new-api-version-19.md)中的新增功能。

有关API版本的信息，请参阅[API版本控制和支持计划](/help/quicksilver/wf-api/api/api-version-support-schedule.md)。

### Workfront 维护更新

有关2025年第一季度版本中所做维护更新的信息，请参阅[Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html)。

### 培训更新

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关详细信息，请参阅[WorkfrontTutorials页面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html)的“新增功能”部分。
