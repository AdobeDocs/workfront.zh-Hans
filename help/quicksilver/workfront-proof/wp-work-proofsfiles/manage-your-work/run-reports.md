---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在 [!DNL Workfront Proof]中运行报告
description: Workfront Proof允许您查看报表，以便跟踪团队的工作进度和效率。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中运行报告


>[!IMPORTANT]
>
>* <span class="previe">报告功能在[!DNL Workfront Proof]中不再可用。 仍显示“报表”选项卡，但数据不准确。</span>
> 
>* 本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

Workfront Proof允许您查看报表，以便跟踪团队的工作进度和效率。

您可以轻松查看在[!DNL Workfront Proof]帐户中创建的验证数量、与每个验证关联的版本数、周转时间等。

## 先决条件

报告是否可用取决于您的[!DNL Workfront Proof]帐户类型和用户权限级别。

* [帐户先决条件](#account-prerequisites)
* [用户先决条件](#user-prerequisites)

### 帐户先决条件 {#account-prerequisites}

报表信息仅适用于Premium计划。

### 用户先决条件 {#user-prerequisites}

报表信息仅适用于对您帐户中的所有验证具有完全访问权限的用户（即 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中至少有[个验证权限配置文件的用户）。

在此面板中，您可以

* 控制显示的数据的时间范围
* 分析一段时间内的量度变化
* 将鼠标悬停在选定时间点上以检查该时间点的详细信息
* 检查在选定时间范围内创建的验证总数
* 检查完成的验证集中包含的平均版本数

## 查看报表 {#viewing-reports}

1. 转到&#x200B;**[!UICONTROL 仪表板]**&#x200B;页面。
1. 单击&#x200B;**[!UICONTROL 报表]**&#x200B;选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 在&#x200B;**[!UICONTROL 时间范围]**&#x200B;下拉菜单中，选择您要显示有关过去24小时、7天、30天、90天或自定义时段内创建的验证的信息。\
   如果选择自定义时间段，请选择开始日期和结束日期，然后单击&#x200B;**[!UICONTROL 应用]**。\
   将显示所选时段的以下信息：\
   **创建的校对：**&#x200B;在选定时间段内创建的校对数。\
   **每个验证的版本：**&#x200B;选定时间段内所有已完成的验证（已批准或已批准更改）的每个验证的平均版本数。\
   **周转时间：**&#x200B;从创建第一个版本到对最终版本做出决策的平均时间。\
   **首次活动时间：**&#x200B;从创建验证时到验证上首次活动时的平均时间。\
   **延迟的校样：**&#x200B;在选定时间段内至少有一个延迟版本的已完成校样（“已批准”或“已批准但有更改”）的平均百分比。\
   **评论和回复：**&#x200B;所选时段内对所有验证所做的平均评论和回复数。

1. （可选）选择或取消选择&#x200B;**[!UICONTROL 显示最小值 — 最大值范围]**&#x200B;选项以确定是否在图形中显示最小值和最大值。\
   选择此选项时，在最小和最大记录值之间显示蓝色底纹。

1. （可选）您可以过滤显示的数据，如[过滤报表](#filtering-reports)中所述。

## 过滤报表 {#filtering-reports}

默认情况下，报表中显示的数据包含来自[!DNL Workfront Proof]系统的所有信息。 您可以使用过滤器仅显示与您的需求相关的信息。

要筛选报表信息，请执行以下操作：

1. 转到&#x200B;**[!UICONTROL 仪表板]**&#x200B;页面。
1. 单击&#x200B;**[!UICONTROL 报表]**&#x200B;选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 运行报告，如[查看报告](#viewing-reports)中所述。
1. 单击&#x200B;**[!UICONTROL 筛选器]**。

1. 在页面的左侧，从以下筛选器选项中选择：\
   **[!UICONTROL 校对类型]：**&#x200B;选择要包含在报告中的校对类型。\
   **[!UICONTROL 决策]：**&#x200B;选择选项以确定是否只做出了包含特定决策的验证。\
   **[!UICONTROL 收件人]：**&#x200B;选择单个用户以查看与与所选用户共享的验证相关的信息。\
   **[!UICONTROL 校对所有者]：**&#x200B;选择单个用户以查看与所选用户拥有的校对相关的信息。\
   **[!UICONTROL 校对创建者]：**&#x200B;选择单个用户以查看与所选用户创建的校对相关的信息。\
   **[!UICONTROL 帐户]：**&#x200B;选择要包含在报告中的帐户。

1. 单击&#x200B;**[!UICONTROL 应用]**。
1. （可选）选择或取消选择&#x200B;**[!UICONTROL 显示最小值 — 最大值范围]**&#x200B;选项以确定是否在图形中显示最小值和最大值。\
   选择此选项时，在最小和最大记录值之间显示蓝色底纹。

## 打印报告

1. 转到&#x200B;**[!UICONTROL 仪表板]**&#x200B;页面。
1. 单击&#x200B;**[!UICONTROL 报表]**&#x200B;选项卡，然后单击&#x200B;**[!UICONTROL 打印]**。\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. 从可用的各种打印选项中进行选择。\
   根据您使用的浏览器和浏览器版本，打印选项会有所不同。
