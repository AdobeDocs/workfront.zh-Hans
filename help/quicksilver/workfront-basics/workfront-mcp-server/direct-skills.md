---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 适用于直接安装的技能
description: Workfront提供了一些可直接在LLM中安装的技能。
author: Becky
feature: Get Started with Workfront
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# 适用于直接安装的技能

Workfront提供了一些可直接在LLM中安装的技能。 技能指南可指导如何将这些工具用于特定任务，并且已内置正确的步骤。

您可以在Adobe Skills GitHub存储库中找到这些技能。

>[!NOTE]
>
>目前，这些技能仅适用于Claude。
>有关使用Adobe设置克劳德的说明，请参阅Adobe Developer文档中的[快速入门](https://developer.adobe.com/adobe-for-creativity/getting-started/)。

## 将技能从Workfront GitHub存储库安装到Claude。

1. 转到GitHub上的[Adobe Workfront技能存储库](https://github.com/adobe/skills/tree/main/plugins/workfront)。
1. 下载要使用的技能文件夹。
1. 将文件夹复制到您的克劳德技能库中。

   * Claude Desktop： `~/Library/Application Support/Claude/skills/` (macOS)或等效项。
   * 克劳德代码： `~/.claude/skills/`。

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## 当前可用的技能

| 技能/文件夹链接 | 技能描述 | 可用于 |
|---|---|---|
| [Planning解决方案架构师](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | 配置Workfront规划工作区以满足您的需求，并回答有关Workfront规划的问题。 | 克劳德 |
