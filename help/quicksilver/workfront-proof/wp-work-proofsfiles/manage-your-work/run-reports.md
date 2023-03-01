---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中运行报告 [!DNL Workfront Proof]
description: Workfront Proof使您能够查看报告，以便您可以跟踪团队的工作进度和效率。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 342f9282-b6f5-425e-a7ef-e23bd011d284
source-git-commit: a0d76692f9e9d12ed0d538c1344638dbc208d625
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# 在中运行报告 [!DNL Workfront Proof]


>[!IMPORTANT]
>
>* <span class="previe">报告功能在中不再可用 [!DNL Workfront Proof]. 仍会显示“报表”选项卡，但数据并不准确。</span>
> 
>* 本文介绍了独立版产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参见 [校对](../../../review-and-approve-work/proofing/proofing.md).


Workfront Proof使您能够查看报告，以便您可以跟踪团队的工作进度和效率。

您可以轻松地查看在中创建的验证数量 [!DNL Workfront Proof] 帐户、与每个验证关联的版本数、周转时间等。

## 先决条件

报告是否可用取决于您的类型 [!DNL Workfront Proof] 帐户和用户权限级别。

* [帐户先决条件](#account-prerequisites)
* [用户先决条件](#user-prerequisites)

### 帐户先决条件 {#account-prerequisites}

报表信息仅适用于Premium计划。

### 用户先决条件 {#user-prerequisites}

报表信息仅适用于对您帐户上的所有验证具有完全访问权限的用户（即至少拥有以下权限的用户） [中的校对权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md))。

在此面板中，您可以

* 控制显示数据的时间范围
* 分析一段时间内量度的变化
* 将鼠标悬停在选定时间点上以检查该时间点的详细信息
* 检查在选定时间范围内创建的验证总数
* 检查完成的验证集中包含的平均版本数

## 查看报表 {#viewing-reports}

1. 转到 **[!UICONTROL 仪表板]** 页面。
1. 单击 **[!UICONTROL 报告]** 选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 在 **[!UICONTROL 期限]** 下拉菜单中，选择是否要显示有关过去24小时、7天、30天、90天或自定义时段内创建的验证的信息。\
   如果选择自定义时间段，请选择开始日期和结束日期，然后单击 **[!UICONTROL 应用]**.\
   将显示所选时段的以下信息：\
   **已创建校对：** 在所选时段内创建的验证数。\
   **每个校对的版本：** 所选时段内所有已完成的验证（“已批准”或“已批准但有更改”）的每个验证的平均版本数。\
   **时间周转：** 从创建第一个版本到对最终版本做出决策的平均时间。\
   **首次活动时间：** 从创建验证时到验证上第一个活动时的平均时间。\
   **验证延迟：** 在所选时段内至少有一个版本延迟的已完成校样（“已批准”或“有更改的已批准”）的平均百分比。\
   **评论和回复：** 所选时段内对所有校对作出的评论和回复的平均数量。

1. （可选）选择或取消选择 **[!UICONTROL 显示最小值 — 最大值范围]** 用于确定最小值和最大值是否显示在图形中的选项。\
   选择此选项时，蓝色阴影会显示在最小值和最大记录值之间。

1. （可选）您可以过滤显示的数据，如中所述 [筛选报表](#filtering-reports).

## 筛选报表 {#filtering-reports}

默认情况下，报表中显示的数据包含来自以下对象的所有信息： [!DNL Workfront Proof] 系统。 您可以使用过滤器仅显示与您的需求相关的信息。

要筛选报表信息，请执行以下操作：

1. 转到 **[!UICONTROL 仪表板]** 页面。
1. 单击 **[!UICONTROL 报告]** 选项卡。\
   ![proof_reports.png](assets/proof-reports-350x193.png)

1. 运行报表，如中所述 [查看报表](#viewing-reports).
1. 单击 **[!UICONTROL 筛选条件]**.

1. 在页面的左侧，从以下筛选器选项中选择：\
   **[!UICONTROL 校对类型]：** 选择要包含在报告中的验证类型。\
   **[!UICONTROL 决策]：** 选择选项以确定是否仅做出了包含特定决策的验证。\
   **[!UICONTROL 收件人]：** 选择单个用户以查看与所选用户共享的验证相关的信息。\
   **[!UICONTROL 校对所有者]：** 选择单个用户以查看与所选用户拥有的验证相关的信息。\
   **[!UICONTROL 校对创建者]：** 选择单个用户以查看与所选用户创建的验证相关的信息。\
   **[!UICONTROL 帐户]：** 选择要包含在报表中的帐户。

1. 单击 **[!UICONTROL 应用]**.
1. （可选）选择或取消选择 **[!UICONTROL 显示最小值 — 最大值范围]** 用于确定最小值和最大值是否显示在图形中的选项。\
   选择此选项时，蓝色阴影会显示在最小值和最大记录值之间。

## 打印报告

1. 转到 **[!UICONTROL 仪表板]** 页面。
1. 单击 **[!UICONTROL 报告]** 选项卡，然后单击 **[!UICONTROL 打印]**.\
   ![proof_reports_print.png](assets/proof-reports-print-350x191.png)

1. 从可用的各种打印选项中进行选择。\
   根据您使用的浏览器和浏览器版本，打印选项会有所不同。
