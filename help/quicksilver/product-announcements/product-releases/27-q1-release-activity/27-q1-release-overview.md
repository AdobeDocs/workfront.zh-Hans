---
title: 2027年第一季度发行版概述
description: 本页介绍了2027年第一季度版本中包含的功能信息。 这些增强功能计划本季度在“生产”环境中提供。
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 3c6235a01af5a18a6ab4b2b80bbdea2c447009aa
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 4%
---

# 2027年第一季度发行版概述

本页介绍了计划于2027年1月发布的2027年第一季度版本中包含的功能。

此页面上的增强功能在“预览”环境中可用。 在2027年第一季度版本接近其计划发布的生产版本时，此页面将进行额外的增强。

>[!IMPORTANT]
>
>
>除非另有说明，否则每月和季度发行计划于当月第二整周的星期四提供。
>
>| 每月发布 | 季度发布 |
>|----|----|
>| <ul><li>2026.11（2026年11月12日）</li><li>2026.12（2026年12月17日）</li><li>2027.01（2027年1月21日）</li></ul> | <ul><li>2027.01（2027年1月21日）</li></ul> |
>
>有关快速发布过程的详细信息，请参阅[启用或禁用快速发布过程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。

## Adobe Workfront增强功能

* [项目增强功能](#project-enhancements)


### 项目增强功能

<table>
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
                <p><a href="/help/quicksilver/product-announcements/product-releases/27-q1-release-activity/27-q1-projects.md">将线程固定到更新顶部</a></p>
                <p>您现在可以将最重要的线程固定到项目、任务、问题或请求的更新区域顶部，以便关键信息对团队可见。</p>
            </td>
            <td><p>2026年10月15日</p></td>
            <td><p>2026年11月12日</p></td>
            <td><p>2027年1月21日</p></td>
        </tr>
    </tbody>
</table>

## 其他区域的发行说明

* [Adobe Workfront Fusion发布活动](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/fusion-release-activity/fusion-release-activity)。
* [Adobe Workfront计划发布活动](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md)。

在这个版本中，以下内容暂无更新：

* 场景计划器
* 校样
* 目标

## 桌面校对查看器更新

### 版本2.3.0

>[!NOTE]
>
>预览： 2026年10月27日
>适用于所有客户的生产版本： 2026年10月28日

桌面校对查看器已更新至版本2.3.0。 此更新包括以下更改：

* 解决了交互式验证的问题：当移动多个版本时，单击屏幕快照下的链接会在多个选项卡中打开页面。 现在，该链接会在单个选项卡中打开页面。

* 将基础框架(Electron)更新到在Chrome版本156上运行的最新版本，以提高性能和安全性。

有关下载和更新桌面验证查看器的信息，请参阅[更新桌面验证查看器](https://experienceleague.adobe.com/zh-hans/docs/workfront/using/review-and-approve-work/proofing/use-the-desktop-proofing-viewer/update-the-desktop-proofing-viewer)。

## 公告

### 弃用工作角色列表视图中的旧版计费和成本率字段

随着时间的推移，我们引进了增强的速率管理能力和专门的工作角色体验，为维护速率信息提供了更完整且可扩展的方法。 因此，费率管理正转向这些专用体验，而不是基于列表的管理工作流。

从2027年1月版开始，旧版字段&#x200B;**每小时计费**&#x200B;和&#x200B;**每小时成本**&#x200B;将不再在Workfront API或工作角色列表视图中可用，包括筛选器/视图/分组配置（直接引用和文本模式计算列）。

作为报告中的替换，您可以使用建议的文本模式代码（根据需要使用`costRates`或`billingRates`）：

    &grave;&grave;
    displayname=Test
    listdelimiter=&lt;br>
    listmethod=nested(costRates)。lists
    type=iterate
    valueexpression=CONCAT({startDate}，&quot; - &quot;，{endDate}，&quot;： &quot;，{value})
    valueformat=HTML
    &grave;&grave;

要管理和审查工作角色费率，请使用专门的费率管理体验：

* 直接从“工作角色”>“费率”页面访问和管理工作角色费率。
* 使用费率报表可以跨工作角色复查、分析和报告费率信息。

无需执行任何操作即可为更改做好准备。 但是，当前在工作角色列表视图中显示&#x200B;**每小时计费**&#x200B;和&#x200B;**每小时成本**&#x200B;字段的管理员应更新其工作流，以使用上述推荐的费率管理体验。

有关工作角色费率的信息，请参阅[创建和管理工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)。

<!--

### Workfront Maintenance Updates

For information about the maintenance updates made during the First Quarter 2027 release, see [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=zh-Hans).

-->

### 培训更新

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关详细信息，请参阅[Workfront教程页面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=zh-Hans)的“新增功能”部分。
