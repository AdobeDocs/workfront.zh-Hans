---
title: 2026年第三季度发布时间框架内的其他增强功能
description: 2026年第三季度发布时间框架内的其他增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 937b49b44f102fee6c9847ab950eb2b274aee89b
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# 2026年第三季度发布时间框架内的其他增强功能

本页介绍了在2026年第三季度版本中对“预览”环境所做的增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第三季度发布周期中此时可用的所有更改列表，请参阅[2026年第三季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)。

## Workfront MCP连接器的更新

我们对Workfront MCP连接器进行了以下更新：

* 我们已扩展MCP服务器以使用EU<!-- and US instances that are not on AWS. Each MCP server can only connect to one instance, but are no longer limited to US instances on AWS-->中的实例。
* 为了扩展Workfront MCP连接器的灵活性，我们添加了连接Claude的功能。 现在，您可以在Claude的连接器列表中找到Workfront，或使用URL直接连接。

有关更多信息和说明，请参阅[配置Adobe Workfront MCP服务器](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)。


## 更新了评论通知电子邮件的外观

>[!NOTE]
>
>客户的生产版本：从2026年7月16日开始分阶段推出

更新区域评论的电子邮件通知具有新外观，与更广泛的Adobe电子邮件设计保持一致。

更新的电子邮件格式包括：

* 新的Adobe Workfront标题取代了以前的Workfront品牌。
* 着重于最新评论的简化版面。
* 主&#x200B;**在Workfront**&#x200B;按钮中查看以直接打开该项。

之前注释的线程不再包含在电子邮件正文中。 若要查看以前对该项目的评论，请使用&#x200B;**在Workfront中查看该项目**，以便在Workfront中打开对话。

此更改将分阶段向客户推出。 确认转出计划后，将更新此页面。

![已更新评论通知email.png](assets/email-look-and-feel-update.png)

## 使用Workfront MCP服务器将Workfront连接到您的AI工具

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

您团队的操作环境位于Workfront。 现在，使用Workfront MCP服务器，可以从您的团队已使用的AI工具中操作该上下文。

将Workfront连接到任何与MCP兼容的人工智能平台，包括Claude、ChatGPT、Copilot、Gemini等，并使用自然语言查找、创建、更新和管理Workfront项目，而无需离开您选择的人工智能工具。 询问您超期的任务、推送项目的完成日期、向审批者发送提醒、更新活动预算，并且您的AI平台可以在Workfront中为您工作。

借助Claude的人工智能技能和计划任务，您可以更进一步，自动执行针对Workfront实时数据主动运行的重复工作流。 例如，周一上午的项目简报、每周容量报告、每月营销活动运行状况检查 — 一次设置，AI会根据您的操作的整个上下文自动处理它。

这是智能工作管理系统的基础，在此系统中，人工智能以您最丰富的运营数据为基础，人与人工智能共同协作，使工作保持全速运行。

>[!IMPORTANT]
>
>目前，Workfront MCP服务器仅适用于美国地区的客户以及使用AWS的客户。

有关详细信息，请参阅[Adobe Workfront MCP服务器概述](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)。

## 增强的列表更新

>[!NOTE]
>
>预览： 2026年5月28日>生产快速发布： 2026年6月11日>适用于所有人的生产： 2026年7月16日

增强列表上的多个字段类型已更新，包括键盘导航和其他增强功能。

增强列表中的被分派人字段现在提供键盘导航：

* 使用键盘上的上下箭头在人员列表中移动。
* 按空格键以选择人员，或\&lt;Delete\>以删除选定的人员。

在增强列表中的单选和多选字段上：

* 字段交互现在可使用键盘。 这包括使用向上和向下箭头在标记、搜索选项和列表之间导航。 按空格键选择项目，或\&lt;Delete\>删除选定项目。
* 在未找到结果时，可以直接从编辑器创建新选项。 请注意，此功能可能并非在所有列表中都可用。

诸如预输入和外部查找字段之类的参考字段已获得一些界面增强。

此外，还以可视方式改进了拖放列（位于提供拖放功能的列表中）的体验。

有关详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。
