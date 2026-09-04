---
title: CX Co-worker提示和最佳做法
content-type: reference
description: 了解在Workfront中使用同事的最佳实践，并查看提示示例列表。
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 1%

---

# CX Co-worker提示和最佳做法

&lt;！ — 不要使用此 — 链接到MCP示例提示文章，确保它随最新版本的MCP一起更新 — >

>[!IMPORTANT]
>
>CX Co-worker目前不适用于医疗保健行业、金融行业或一些其他具有敏感数据的行业。 AI助手可供这些组织使用。 有关详细信息，请参阅[AI助手概述](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)。

有了CX Co-worker ，您可以使用自然语言与Workfront Workflow和Workfront Planning交互。

同事是Adobe Experience Cloud Agent Orchestrator的一部分。

有关Agent Orchestrator的详细信息，请参阅[Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/zh-hans/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator)。

## 访问权限要求

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>选择、Prime或Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>Standard或Light</p>
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td><p>对于基础技能之外的任何功能，您的组织必须已购买Adobe Agent Orchestrator。</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>您必须具有相应的权限才能通过同事与任何对象进行交互。</p> <p>例如，要通过同事接收有关项目的信息，您必须至少具有该项目的“查看”权限。</p></td>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 您的Workfront管理员必须为贵组织启用AI助手。

  有关详细信息，请参阅AI助手概述一文中的[AI助手先决条件](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)。
* 您的Workfront管理员必须已启用您访问级别的AI助手。

  有关详细信息，请参阅[启用或禁用AI助手](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md)。

## 注意事项

使用CX Co-worker时请考虑以下限制：

### 可逆性

某些操作可以撤销。 例如，如果创建了一个对象，则该创建可以撤销。

但是，某些操作（如对象删除）不能&#x200B;**撤销**。 我们建议在通过同事对您的数据执行操作时记住这一点。

### 数据/对象覆盖范围限制

* 对自定义字段的查询和报告处于早期阶段，并且某些技能（如基于API的查询帮助程序）尚未处理用于聚合和筛选的任意自定义字段。

### 交互/UX限制

* CX Co-worker目前不从单个用户的风格或偏好“学习”长期。 每次聊天仅使用当前的交谈和产品知识。
* 对话上下文保存在单个聊天会话中。 打开新页面或关闭助理将重置对话历史记录。
* 如果审批过程位于外部应用程序（如Confluence或SharePoint）中，并且仅通过URL字段链接，则同事当前不会获取这些页面并对其进行归因。

### 数据存储/客户管理的密钥

* 由于CX Co-worker是Adobe Experience Platform Agent Orchestrator的一部分，因此您与Co-worker交互的数据存储在Adobe Experience Platform中，而不是Workfront中。 因此，Workfront客户管理的密钥(BYOK)协议不涵盖此数据。

## 通用基础AI技能

>[!IMPORTANT]
>
>这些通用功能适用于其组织已签署文件上的Adobe AI协议的所有用户。

有关这些一般使用技能的最佳实践和提示，请参阅[AI助手提示和最佳实践](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md)。

<!--Follow up with Oznur-->

### 产品知识

CX Co-worker可以提供从Workfront文档中提取的说明或参考信息。

有关从Workfront文档提取信息的更多信息，请参阅[从AI助手获取帮助](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md)。

示例：如何更改任务持续时间类型？

### 项目、任务和问题摘要

CX Co-worker可以总结已上载到Workfront的项目、任务或问题<!--, or documents-->。

有关项目、任务和问题摘要的详细信息，请参阅[使用AI助手摘要](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md)。

示例：总结名为“Fall Campaign 2026”的项目。

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## Workfront中的CX Co-worker

* [项目、任务和问题信息](#project-task-and-issue-information)
* [项目和工作管理](#project-and-work-management)
* [内容和审批](#content-and-approvals)

### 项目、任务和问题信息

CX Co-worker可以为您提供有关项目、任务和问题的信息，包括摘要和项目状况。

在以下区域查看文档和资产审批的示例提示：

* [查找有关项目、任务或问题的信息](#find-information-about-projects-tasks-or-issues)
* [概述项目、任务或问题](#summarize-projects-tasks-or-issues)
* [显示项目、项目群或项目组合的项目运行状况](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### 查找有关项目、任务或问题的信息

* 项目
  * 显示品牌营销团队的所有活动项目
  * 需要第4季度营销活动组合中“数字”类别下的项目列表。
  * 向我显示由Creative Services公司中作为项目经理的用户管理的项目。
* 任务
  * 把所有任务都分派给我琼·哈里斯。
  * 显示分配给UX团队的“设计”类别中的任务。
  * 我需要在“假日促销活动”项目中向撰稿人分配任务。
* 问题
  * 在“技术”类别下显示“网站重新设计”项目中的所有问题。
  * 获取QA组报告的所有未解决的问题。
  * 我需要将问题分配给全球技术公司的开发人员。

#### 概述项目、任务或问题

* &quot;总结此项目&quot;
* “总结一下这个项目的最后一周”

#### 显示项目、项目群或项目组合的项目运行状况

>[!NOTE]
>
>您的组织必须注册Project Health测试版才能使用此功能。

* “向我显示我的活动项目的运行状况”
* “向我展示此计划的运行状况”

### 项目和工作管理

您可以使用CX Co-worker创建和管理项目，包括任务和分配。

在以下区域查看项目和工作管理的示例提示：

* [创建、更新或删除项目](#create-update-or-delete-projects)
* [根据用户提示确定正确的项目模板](#identify-the-right-project-template-based-on-user-prompt)
* [添加、编辑或自定义项目中的任务](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### 创建、更新或删除项目

您可以从头开始创建项目，也可以从模板创建项目，更新项目并删除项目。

* 从3月10日至4月30日创建一个名为“第2季度创新沙盒”的空白项目。 将我设置为所有者。
* 使用集成营销活动模板创建名为Lucent AI Launch - NA的项目。 从2月5日开始，并将其设置为“当前”。
* 从3月1日开始，到6月15日结束，创建一个名为“网站重新设计 — EMEA”的项目。 该课程由EMEA营销部所有，由营销部副总裁赞助，预算为25万美元，计划时数约为1,200小时，重点是欧洲，目标是提高转化率。
* 对于Lucent AI Launch - NA项目，请将其移至第二季度，更改目标以推动免费试用，将完成日期推迟到4月中旬，将预算增加到15万美元，并将其标记为紧急。
* 显示在第2季度完成的所有当前营销项目（高优先级或紧急优先级），按最早结束日期排序。

#### 添加或编辑任务

您可以在项目中添加或编辑任务，也可以自定义用于创建项目的模板的任务列表。

* 将称为登陆页面QA的新任务添加到项目中，并安排在4月22日至4月26日之间执行该任务。
* 更新设计审阅任务，使其在4月18日完成并将其分配给创意团队。
* 从项目中删除打印资产生产任务。
* 显示此项目中未完成并计划于4月1日至4月30日期间开始的所有任务。
* 将“法律审批”设置为营销活动启动任务的前置任务。
* 添加名为“最终复制抛光版”的新任务，计划从4月15日至4月16日，将复制审阅任务移至4月10日，删除额外审阅轮次任务，并将“最终复制抛光版”设置为“电子邮件构建”的前身。
* 在项目创建流程中，请尝试尽可能多地提供有关最好应成为项目下的任务的可交付结果的信息。

#### 创建、更新或删除分配

您可以创建、更新和删除用户或工作角色分配。

* 对于项目“产品上市的设计登陆页面”，为所有当前未分配的任务确定相应的工作角色和推荐的已计划小时数。
* 我有多个未分配任务，包括“为营销活动网站实施GA4跟踪”、“设置转化事件”和“验证分析数据”。 您能否为每个人提供正确的工作角色和估计小时数建议？
* 对于创意任务“为EMEA展示广告创建3个横幅变体”、“应用修订”和“导出最终资源”，分配最佳工作角色并估计每个任务所需的工作。
* 在项目“第2季度产品发布”、“网站重新设计 — EMEA”和“付费媒体营销活动 — NA”中，识别所有未分配任务并为每个任务分配适当的职位角色以及建议的计划小时数。

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### 内容和审批

CX Co-worker可帮助管理Workfront中的文档和资产批准。

处理文档和资产审批时，请考虑以下事项：

* 必须先为您的组织启用内容审批，然后才能在同事中使用此功能。
* AI不能代表人类批准或拒绝。 除Workfront AI审阅者外，决策依赖用户。

  有关Workfront AI审阅者的详细信息，请参阅[Workfront AI审阅者入门](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。
* 此功能存在于Workfront中，无法用于与外部工具或文档提供程序交互。
* 为获得最佳体验，请将此功能与统一审批体验结合使用。

  有关统一审批的详细信息，请参阅[统一审批概述](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)。

在以下区域查看文档和资产审批的示例提示：

* [添加或删除审批参与者](#add-or-remove-approval-participants)
* [提醒利益相关者等待审核的单个资产](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [添加、更新或应用单个资源的审批模板](#add-update-or-apply-approval-templates-for-a-single-asset)

#### 添加或删除审批参与者

* 将Sarah Chen和Miguel Alvarez添加为当前文档的批准者。
* 从此审批中删除Jennifer Otto。
* 移除尚未做出批准决策的任何人。
* 向spring-campaign.pdf中添加了一个名为“最终审阅”的新阶段。
* 在winter-campaign.pdf的第二阶段添加Mark和Sarah作为批准者，添加Phil作为审阅者
* 对于winter-campaign.pdf，第一阶段将截止时间定在今天下午5点，最终审核将截止时间定在明天下午5点
* 在fall-campaign.png中添加一个最终检查阶段，截止时间为星期四下午5点，并包括Jim和Pam作为批准者，Oscar作为审阅者
* 将Mark Jones作为审阅人添加到fall-campaign.png的第一阶段和最后阶段。
* 让我们获得针对fall-campaign.png的多阶段批准，包含3个阶段，1个设计2个撰写，3个法律。 每个阶段只需要一个决策。 将Mike、Sally、Jane添加到设计，将Chris、Richard、Mark添加到文案撰写，将Phil、Tom和Sarah添加到法律。

#### 提醒利益相关者等待审核的单个资产

* 向未响应资产“Spring Campaign视频”的批准者发送提醒。
* 提醒所有尚未批准此资产的“春季促销活动视频”。
* 谁尚未对资产“品牌指南PDF”做出决定？ 提醒他们。

#### 添加、更新或应用单个资源的审批模板

* 将“营销发布”审批模板应用于名为“春季促销活动视频”的资产。
* 创建具有3个阶段的新审批模板：Creative审核、法律和最终审批。
* 把朱莉娅·桑托斯和肖恩·贝克加到第一阶段。
* 编辑“产品发布”模板，将Elizabeth Peterson添加到最终批准阶段。
* 创建一个名为“紧急审核”的模板，该模板具有一个阶段，可分配给Olivia Kim。
* 通过删除Rick Kuvec并将Karen Sterling添加到第2阶段来更新“Creative Review”模板。


## Workfront规划中的CX同事

### 使用计划记录

* [创建、删除、复制或恢复记录](#create-delete-duplicate-or-restore-records)
* [将记录链接到其他记录](#link-records-to-other-records)
* [编辑、更新字段或将其附加到记录](#edit-update-or-append-a-field-to-a-record)
* [访问记录更改历史记录](#access-record-change-history)

#### 创建、删除、复制或恢复记录

* 创建新的营销活动记录，称为2026年夏季促销
* 添加名为Widget Pro且价格为299美元的新产品记录
* 能否为约翰·史密斯创建新的潜在客户记录？
* 删除名为“旧促销”的活动记录
* 删除我刚刚创建的测试记录
* 能否删除记录ID Rc123abc456？
* 复制Q1营销活动记录
* 能否复制此营销活动以创建新营销活动？
* 制作假日促销活动副本
* 恢复我意外删除的营销活动
* 能否恢复已删除的项目记录？
* 我意外删除了记录，你能恢复它吗？

#### 将记录链接到其他记录

* 将夏季促销活动记录链接到第2季度计划
* 能否将此产品关联到相关的营销活动？
* 我需要将这三个潜在客户与企业客户记录关联

#### 编辑、更新字段或将其附加到记录

* 将夏季促销活动中的预算字段更新为$75,000
* 您是否将此项目记录的状态更改为“已完成”？
* 将John Doe添加到此计划的团队成员字段

#### 访问记录更改历史记录

* 显示夏季促销活动记录的更改历史记录
* 能否显示谁修改了此项目以及更改了哪些内容？
* 我需要查看上周对此记录所做的所有更新

### 在Workfront Planning中使用System Designer

* [创建和配置工作区](#create-and-configure-workspaces)
* [定义记录类型](#define-record-types)
* [设计字段和公式字段](#design-fields-and-formula-fields)
* [构建自定义视图](#build-custom-views)


#### 创建和配置工作区

* 创建一个名为“2026年营销活动”的新规划工作区
* 更新我的产品计划工作区以将颜色更改为蓝色并添加说明
* 显示我有权访问的所有Planning工作区

#### 定义记录类型

* 在我的Planning工作区中创建一个名为营销活动的新记录类型
* 更新计划记录类型以更改其图标和描述
* 显示我的营销计划工作区中的所有记录类型

#### 设计字段和公式字段

* 将预算字段添加到我的计划营销活动记录类型（具有货币类型）
* 在Planning中创建一个公式字段，用于计算到市场活动结束日期的剩余天数
* 更新我的Planning工作区中的“优先级”字段以添加更多下拉选项

#### 构建自定义视图

* 在Planning中创建时间线视图，按开始日期和结束日期查看我的营销活动计划
* 向我的Planning计划添加一个新表格视图，该视图仅过滤活动状态
* 复制我的Planning活动营销活动视图，并修改排序。
