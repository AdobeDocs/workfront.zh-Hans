---
title: AI Assistant概述
content-type: reference
description: AI Assistant概述
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: a4e403abadc0268b919ce8105989ef6c912f33a4
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 1%

---

# AI Assistant概述

Workfront的AI助手通过提供应用程序内信息和自然语言对话建议，帮助您完成工作。 AI助手可以通过以下方式为您提供更流畅的工作体验

* 汇总工作项或文档
* 查找工作流程的说明或参考材料
* 为计算字段生成或检查公式

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>新建：任何</p>
       <p>或</p>
       <p>当前：不可用</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：不可用</p></td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## AI助理的先决条件

要为您的组织启用AI助手，必须应用以下所有的&#x200B;**所有**：

* 您的组织必须已迁移到Adobe IMS (Identity Management System)
* 必须启用Adobe Unified Experience
* 您的组织必须具有Select、Prime或Ultimate Workfront计划
* Adobe必须具有已签署的Adobe Gen AI协议

  有关签署协议的更多信息，请参阅本文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## 关于AI Assistant的注意事项

* AI Assistant与您已打开的页面上下文相关。 例如，在项目页面上输入“此项目摘要”到AI助手将返回特定项目的摘要。
* Workfront管理员必须为贵组织中的用户启用AI助手。 通过访问级别启用AI助手。

  有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

* Workfront Planning AI助手具有与Workfront AI助手不同的功能。

  有关Workfront规划中的AI助手的详细信息，请参阅[Adobe Workfront规划AI助手概述](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)。

* AI助手当前只有英文版。


## AI助手中可用的功能

AI助手当前提供以下功能：

* 汇总项目、任务、问题或文档。

  有关详细信息，请参阅[使用AI助手汇总](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)。

* 在Adobe Experience League上提供从Workfront文档提取的说明或参考信息。

  有关详细信息，请参阅[从AI助手获取帮助](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)。

* 在Workfront中查找特定项目。

  有关详细信息，请参阅[使用AI助手处理项目、任务和问题](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md)。

* 为已计算的自定义字段生成或优化公式。

  >[!NOTE]
  >
  >此功能仅适用于Prime或Ultimate Workfront计划中的组织。

  有关详细信息，请参阅[使用AI助手生成或修订计算字段公式](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md)。

* 在下列时间范围内总结项目的更新、上传文档和其他显着更改：优先级中的24小时、3天、7天。

有关详细信息，请参阅[在优先级中更新工作](/help/quicksilver/workfront-basics/priorities/catch-me-up.md)。


## AI助手可用的对象类型

如果用户在Workfront中拥有有效权限，则AI Assistant可以查询与以下对象类型关联的数据：

* 项目组合
* 项目群
* 项目
* 任务
* 问题
* 自定义表单
* 用户
* Workfront Planning记录


## 访问AI助手

1. 在任何Workfront页面顶部，单击AI助手图标![AI助手图标](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)。
1. 在屏幕右侧的面板中键入您的问题或提示。

   如果您无法在此面板中键入，则表明贵组织没有已签署的Adobe Gen AI文件协议。

1. 如果AI助手未提供您所需的答案，请优化您的提示并重试。

## 签署Adobe Gen AI协议

如果贵组织在文件中没有已签署的Adobe Gen AI协议，则无法为贵组织启用AI助手。

如果用户在Adobe Gen AI协议未签署时尝试使用AI助手，他们会看到一条消息：

* 用户：将通知用户尚未为其组织启用AI助手，用户可以联系Workfront管理员为其组织请求启用。
* 管理员：管理员将收到通知，告知他们没有已签署的Adobe Gen AI协议，可以请求发送协议副本以供签署。

要请求Adobe Gen AI协议，请执行以下操作：

1. 作为Workfront管理员，单击AI助手图标![AI助手图标](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)。
1. 开始在AI助手面板中键入。
1. 出现Adobe Gen AI协议消息时，单击&#x200B;**审阅协议**。
1. 输入贵组织内将签署Adobe Gen AI协议的人员的姓名和电子邮件地址。

   协议将发送给此人签署。 签署并返回协议后，Adobe会审核协议，然后为您的组织启用AI助手。

## 在AI助手中创建提示的提示

在提示中使用以下关键字，以提供上下文并帮助查找正确的信息。 关键字不区分大小写。

输入提示时，请包含短语`using (keyword)`。

| 关键词 | 效果 |
|---|---|
| `workfront` | 与Workfront交互。 |
| `planning ` | 与Workfront Planning交互。 |
| `help` | 从Experience League文档返回信息。 |
| `formula` | 检查并返回用于Planning、设置或自定义表单的公式。 |
| `health` | 使用项目运行状况顾问检查项目运行状况。 |
| `summarize` | 汇总项目，例如在上传文件或汇总项目时。 |

>[!NOTE]
>
> 并非所有关键字在所有区域都可用。
>
>* `formula`关键字仅在Planning、设置和自定义表单生成器中可用。
>* `planning`关键字仅在Workfront Planning中可用。





