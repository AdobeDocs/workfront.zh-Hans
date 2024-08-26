---
title: Adobe Workfront Planning AI助手概述
description: 您可以使用AI助手根据当前页面上下文和记录结构生成、更新或删除记录。 用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: f9abcd9ff4c80376bed229a1d65e0efcbfc332b0
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---


# Adobe Workfront规划AI助手概述

{{planning-important-intro}}

您可以使用AI Assistant根据当前页面上下文和记录结构生成、更新或删除记录。

用户的命令和AI执行这些命令共同工作，以确保AI所做的更改准确反映在您的环境中。

## 关于AI助理的注意事项

* 必须先为贵组织启用AI助手，然后该助手才可供贵公司的用户使用。 有关信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。
* 在Workfront为贵组织启用AI助手后，主Workfront管理员可以使用该助手。 有关信息，请参阅[配置系统的基本信息](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* Workfront管理员必须为所有其他用户启用AI助手。 有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

* AI助手在每个页面的上下文中工作。 您为AI助手提交的请求必须引用您打开的页面中可用的功能。

* AI助手在“规划”区域中执行的操作将与Workfront规划权限和Workfront访问级别的上下文相关。 有关信息，请参阅以下文章：

   * [在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [使用Adobe Workfront Planning时的许可证类型概述](/help/quicksilver/planning/access/license-type-overview.md)

* AI助手代表用户所做的更改在记录的历史记录面板中进行跟踪。

* 您可以使用命令撤消操作。 例如，您可以键入“撤消上次更改”以恢复更改。

## 当前可用于AI助手的功能

目前，AI助手可在Workfront的“规划”区域访问以下页面：

* Workspace页面
* 记录类型页面
* 记录页面

此时可以使用AI助手执行以下操作：

* 搜索记录。 您可以按任何记录字段中包含的信息进行搜索。
* 创建记录。 创建记录后，将显示一个包含指向新记录的链接的ID。 您可以指定要在创建过程中更新的字段，如日期或说明。
* 根据上传的文档创建记录。 Workfront支持AI助理的以下文档格式：

  .pptx、.pdf、.docx、.xlsx、.ppt、.doc、.txt和大多数图像格式
* 更新您在屏幕上看到的记录的字段
* 删除记录
* 恢复您刚刚删除的记录

## 访问规划区的人工智能助理

1. 登录到Workfront，然后转到&#x200B;**计划**&#x200B;区域。

1. 单击&#x200B;**工作区信息卡**。

1. （可选）单击&#x200B;**记录类型卡片**。

1. （可选）单击&#x200B;**记录**&#x200B;以打开记录的&#x200B;**详细信息**&#x200B;页面。

1. 单击全局导航栏中屏幕右上角的&#x200B;**AI助手图标**。

   ![](assets/ai-assistant-icon-highlighted.png)

1. 在提供的空白处，开始输入AI Assistant的命令，然后在完成后单击Enter。

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   例如，您可以键入以下内容之一：

   * 创建开始日期为7月4日、结束日期为7月30日的营销活动
   * 更新夏季促销活动记录的描述字段，日期待定
   * 删除最后一个记录
   * 恢复记录

   当AI助手处理命令时，将显示一个视觉指示器，设置响应时间的期望值。

   收到成功响应后，请按照提供的链接或注意左侧的更改内容。
