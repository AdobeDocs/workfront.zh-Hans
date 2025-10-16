---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 搜索来自 [!DNL Adobe Workfront] 的 [!DNL Slack]项
description: 您可以从已安装的 [!DNL Adobe Workfront] 应用搜索 [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 项目。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 6%

---

# 从[!DNL Adobe Workfront]搜索[!DNL Slack]项

如果您的[!DNL Adobe Workfront]实例安装了[!DNL Slack]应用，则可以从[!DNL Slack]搜索[!DNL Workfront]项。

有关使用[!DNL Workfront]配置[!DNL Slack]的详细信息，请参阅[为 [!DNL Adobe Workfront] 配置 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>任何</p>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在从[!DNL Workfront]中搜索[!DNL Slack]项之前，您必须

* 为[!DNL Workfront]配置[!DNL Slack]\
   有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 从[!DNL Workfront]搜索[!DNL Slack]项：

1. 从[!DNL Slack]登录到[!DNL Workfront]实例并登录到[!DNL Slack]。\
   有关从[!DNL Workfront]登录到[!DNL Slack]的详细信息，请参阅[!DNL Workfront]访问[!DNL Slack]从[中的“从 [!DNL Adobe Workfront] 登录到 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)”部分。

1. 从任何渠道中，开始在消息字段中键入以下任一命令：

   `/workfront search <keyword>`

   或

   `/wf search <keyword>`

   >[!NOTE]
   >
   >命令区分大小写。 该关键字不区分大小写，并且输入时必须不含括号或引号。

1. 在显示的字段中，从以下选项中选择一种对象类型：

   * 项目
   * 任务
   * 问题
   * 报表
   * 人员
   * 模板
   * 文档
   * 组合
   * 项目群
   * 功能板
   * 公司
   * 注释

     一次只能选择一个对象类型。\
      将显示与搜索条件匹配的项目列表。

1. 单击项目的名称，以在新浏览器选项卡的[!DNL Workfront]中将其打开。
