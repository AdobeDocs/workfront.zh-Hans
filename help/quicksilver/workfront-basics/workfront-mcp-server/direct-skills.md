---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: 适用于直接安装的技能
description: Workfront提供了一些可直接在LLM中安装的技能。
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# 适用于直接安装的技能

Adobe Workfront提供了一些可直接在LLM中安装的技能。 技能指南可指导如何将这些工具用于特定任务，并且已内置正确的步骤。

您可以在Adobe Skills GitHub存储库中将这些技能作为文件找到。 此存储库包含用于各种Adobe产品的文件。 下载这些文件并将其复制到Claude时，Claude可以使用文件中描述的技能。

例如，Planning解决方案架构师的技能允许Claude回答有关的问题并在Workfront Planning中执行某些操作。

在将这些技能复制到LLM后，您不需要调用或触发这些技能。 相反，您可以像往常一样与LLM进行交互，以自然语言提问，LLM会使用技能中描述的信息和适合对话的操作。

>[!NOTE]
>
>目前，这些技能仅适用于Claude。
>有关使用Adobe设置克劳德的说明，请参阅Adobe Developer文档中的[快速入门](https://developer.adobe.com/adobe-for-creativity/getting-started/)。

## 将技能从Workfront GitHub存储库安装到Claude

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
