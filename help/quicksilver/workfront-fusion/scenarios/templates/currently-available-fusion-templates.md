---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 当前可用的Adobe Workfront Fusion模板
description: Adobe Workfront Fusion中当前提供以下公共模板。
author: Becky
feature: Workfront Fusion
exl-id: 29d95b93-ab54-416d-b0d5-ff12634951b2
source-git-commit: 2b2424a26ba903cda8f03c468da733732bf6d434
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 0%

---

# 当前可用的Adobe Workfront Fusion模板

Adobe Workfront Fusion中当前提供以下公共模板。

您的团队或组织可能有其他团队创建的模板可用。

要查看可用的模板，请单击 **模板** 图标 ![](assets/fusion-template-icon.png) 在Fusion的侧面导航菜单中。

## Workfront模板

这些模板可自动化Workfront流程和工作流。

### Workfront — 从CSV创建项目

此自动化会根据您在CSV中指定的名称、Portfolio、状态、计划开始日期和模板详细信息在Workfront中创建新项目。

### Workfront — 清理请求，过去30天内未添加任何新注释

使用此模板对您的请求强制30天附注更新。 如果在30天内未更新请求，则其状态会在60天内更改并关闭。

### Workfront — 在100%完成时将项目状态更改为完成。

此自动化功能可将项目更新为“完成”状态，所有1005点完成的任务均在此状态。 具有未结问题、未结任务或项目批准的项目将收到更新，在解决后，项目将变为完成状态。

### Workfront — 警告并尝试关闭过时的项目

使用此方案有助于自动警告和关闭符合贵组织过时项目策略的项目。

### Workfront — 将来自源问题/请求的新注释和回复复制到已转换的项目或任务

使用此模板可将问题或请求的注释和回复复制到已转换的项目或任务中。

### Workfront — 将项目群自定义Forms和字段数据复制到关联的新项目

该自动化可监控具有自定义表单的程序中的新项目。 然后，它将这些项目群自定义表单和字段添加到新项目中。

### Workfront — 将Portfolio自定义Forms和字段数据复制到关联的新项目

该自动化功能可监控带有自定义表单的项目组合中的新项目。 然后，它将这些项目组合自定义表单和字段添加到新项目中。

### Workfront — 将批准的问题转化为项目

此模板将问题转化为项目。 您可以修改它以符合贵组织的标准。

### Workfront — 将文档从问题/请求复制到已转换的项目或任务

此灵活方案将问题或请求中的文档复制到以前转换的项目或任务中。

### 根据字段更改量身定制的通知

此模板根据某些独特事件（如字段值的更改），为处理Workfront项目的个人创建量身定制的更新（和相关通知）。 该场景会监视Workfront中指定字段在任务或问题中何时发生更改。 遇到时，场景将评估相关项目中的信息，并为分配给项目上特定角色的人员创建量身定制的更新。

### Workfront — 使用约定批量附加到项目名称

此批量更新模板可重命名符合搜索条件（属于项目组合）的所有项目，并使用标准格式重命名它们。

### Workfront — 按约定重命名项目

此模板可查找符合过滤器标准（属于项目组合）的所有项目，并以标准格式重命名它们。

### Workfront — 创建状态更改基线

此模板会在“切换”模块中记录的任何项目状态更改时捕获项目基线，并在更新流中创建更新以供日志记录。

### Workfront — 每周创建基线

此模板在每周的星期一早上6点按项目组合过滤的项目上捕获项目基线，并在更新流中创建更新以供日志记录。

### 查找未在策略时间内使用的项目模板并通知

每月使用您自己的策略查看一次项目模板，该策略与此易于管理的模板一起通知违反您策略的相应用户模板。

## Workfront - Workfront Proof模板

这些模板可自动执行将Workfront与Workfront Proof相结合的工作流。

### Workfront Proof > Workfront — 验证决策中的项目更新

当对直接添加到项目的验证做出决策时，此自动化会收集有关验证决策的信息（例如做出决策的人员），然后在相应的Workfront项目中作为更新反映此进度。

### Workfront Proof > Workfront — 根据验证决策更新并完成任务（如果已批准）

当单个验证绑定到单个任务时，此场景将在对验证做出审批决定时关闭关联的任务。 如果获得批准，它将完成任务并更新项目。

## HTTP - Workfront模板

这些模板从Web服务中检索信息，并将该信息导入Workfront。

>[!NOTE]
>
> 您必须拥有Workfront Fusion for Work Automation and Integration许可证才能在此部分中使用模板。

### 使用JWT（JSON Web令牌）建立连接

为客户端API建立JWT授权。

### APILayer > Workfront — 每日汇率更新(EUR)

此模板创建一个方案，该方案可自动在设定的时间点更新汇率。 此方案从APIlayers.com API中提取欧元(EUR)对美元(USD)的汇率并更新Workfront中的汇率。

## Workfront-Marketo模板

这些模板支持Workfront-Marketo集成。

>[!NOTE]
>
> 您必须拥有Workfront Fusion for Work Automation and Integration许可证才能在此部分中使用模板。

### 通过Workfront审批工作流审批您的Marketo Engage电子邮件草稿

这是Workfront与Marketo Engage之间的“审核和批准”集成的一部分。 此模板检测Workfront中的电子邮件验证是否已被批准，然后按照批准更新Marketo Engage中的相应电子邮件。

### 在Workfront中提出引入营销活动请求并在Marketo Engage中自动创建营销活动

此方案提供了一种以编程方式根据在Workfront中发出的请求在Marketo Engage中创建电子邮件和网络研讨会营销活动。 通过使用自动化来创建、组织和配置活动，团队可以提高效率。

### 在Workfront中查看Marketo Engage电子邮件草稿的电子邮件验证

此模板检测Workfront任务是否已设置为准备好审查状态，然后从Marketo Engage导出电子邮件草稿以将其保存为Workfront中的验证。

## Workfront-SharePoint模板

这些模板将Workfront与SharePoint连接起来。

>[!NOTE]
>
> 您必须拥有Workfront Fusion for Work Automation and Integration许可证才能在此部分中使用模板。

### 观看SharePoint文件夹更改

利用此模板，可查看SharePoint文件夹中是否有更改。


## Workfront-Anaplan模板

这些模板支持Workfront-Anaplan集成，并期待在Workfront中的Anaplan中进行特定配置。 有关这些模板及其所需配置的信息，请参阅各个模板的文章。

有关Workfront-Anaplan集成的详细信息，请参阅 [Adobe Workfront与Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

>[!NOTE]
>
> 您必须拥有Workfront Fusion for Work Automation and Integration许可证才能在此部分中使用模板。

### 支出优化工作流

* [发送 [!DNL Adobe Workfront] 的项目更新到 [!DNL Anaplan] 列表项](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [发送 [!DNL Adobe Workfront] 支出至 [!DNL Anaplan] 列表项](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
* [发送 [!DNL Adobe Workfront] 对的实际小时数更新 [!DNL Anaplan] 列表项](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

### 用于链接预算请求的工作流

* [创建 [!DNL Anaplan] 列表项来自 [!DNL Adobe Workfront] 预算请求](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 项目](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

### 用于链接营销活动请求的工作流

* [创建 [!DNL Anaplan] 列表项来自 [!DNL Adobe Workfront] 营销活动请求](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 活动请求或活动项目](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)


<!--[!BADGE New!]{type=Informative} -->