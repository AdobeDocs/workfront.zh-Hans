---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: 搜索来自 [!DNL Slack]的 [!DNL Adobe Workfront] 项
description: 您可以从已安装的 [!DNL Slack], if your instance of Slack has had the [!DNL Workfront] 应用搜索 [!DNL Adobe Workfront] 项目。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 85821f21-d4fd-4f28-bd7a-0c109a4433a8
TQID: https://experienceleague.adobe.com/JulYq173XQa6mG93qzUwfBDn4TPVEafD2OVpcIAXxi8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 208
ht-degree: 15%

---

# 从[!DNL Slack]搜索[!DNL Adobe Workfront]项

如果您的[!DNL Slack]实例安装了[!DNL Workfront]应用，则可以从[!DNL Slack]搜索[!DNL Adobe Workfront]项。

有关使用[!DNL Slack]配置[!DNL Workfront]的详细信息，请参阅[为 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)配置 [!DNL Adobe Workfront] 。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>“任一”</p>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在从[!DNL Slack]中搜索[!DNL Workfront]项之前，您必须

* 为[!DNL Slack]配置[!DNL Workfront]\
   有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 从[!DNL Slack]搜索[!DNL Workfront]项：

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。\
   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

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
   * 报告
   * 人员
   * 模板
   * 文档
   * 项目组合
   * 项目群
   * 仪表板
   * 公司
   * 注释

     一次只能选择一个对象类型。\
      将显示与搜索条件匹配的项目列表。

1. 单击项目的名称，以在新浏览器选项卡的[!DNL Workfront]中将其打开。
