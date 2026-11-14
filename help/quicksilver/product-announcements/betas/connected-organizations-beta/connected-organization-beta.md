---
product-area: betas
title: “连接的组织”功能Beta项目
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 8f8f4e7962bfde525470842caecd49f03b758b29
workflow-type: tm+mt
source-wordcount: '2241'
ht-degree: 1%
---
# 互联组织功能测试版计划

>[!IMPORTANT]
>
>“连接的组织”功能目前处于封闭的测试阶段，面向少量客户。
>
>Beta测试将持续到2026年底。
>
>如有疑问，请联系您的Adobe Beta项目经理。

利用“连接的组织”功能，公司及其合作伙伴可以在两个组织都购买了Adobe Workfront时协作处理工作。

例如，客户公司可以向其提供商公司提交关于待完成工作的请求。

每个公司都可以继续使用自己的Workfront实例，以及自己的用户、权限和工作流。

工作对象在两个实例之间镜像，只有双方同意共享的数据才会同步。

结果是共享请求、状态和决策的视图，而无需其他访客登录、重复许可证或长电子邮件线程。

## 当今多组织工作流程概述

当两家企业都投资于Workfront时，它们应该能够在不支付两倍费用或进入对方体系的情况下开展合作。

今天，当两家公司在两个不同的系统中工作时，他们的协作可能包括以下一些工作流：

* 请求和简讯会通过难以遵循的电子邮件线程传送。

* 移交是手动进行的，几乎没有可审计性。

* 在另一个公司的系统中工作意味着访客登录、额外的许可证，或两者兼而有之。

* 文件有多个副本在传播，没有人知道哪个是真实来源。

* 状态很难跟踪，因此客户经理会花时间构建平台并安排更新会议。

## “连接的组织”解决方案概述

当您使用“已连接”组织功能时，两家公司将继续在两个不同的系统中工作，它们的协作将包括以下一些工作流：

* 这两个组织都不会访问另一个实例中的对象。
* 对象（例如来自客户端组织的请求）将复制并发布到提供商的实例中。
* 只有为同步配置的元数据才会在两个副本之间保持最新。
* 每个公司都管理其自己的用户、权限和超出该对象的工作流。

指导原则是共享完成工作所需的最低限度，并保密其他所有内容。

<table>
<tbody>
<tr class="odd">
<td><strong>共享内容</strong></td>
<td><strong>哪些内容保持隐私</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>简报和请求详细信息</p></li>
<li><p>商定的截止日期和里程碑</p></li>
<li><p>查看评论</p></li>
<li><p>批准决定</p></li>
<li><p>最终批准的资产</p></li>
</ul></td>
<td><ul>
<li><p>与其他客户或其他机构的关系</p></li>
<li><p>财务状况、费率，以及对客户的收费</p></li>
<li><p>资源规划和能力</p></li>
<li><p>内部项目结构、任务和未选择共享的任何字段</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Beta版中可用的功能

Beta计划的第一阶段允许您连接两个实例并启动工作。

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **功能** | **它的功能** |
| **连接的组织** | 链接两个组织之间的两个Workfront实例。 在Beta测试期间，Adobe会配置连接。 目前正在开发自助设置。 |
| **请求表单** | 客户公司通过表单的“共享”设置创建请求表单并发布它，然后与提供商公司共享。 |
| **AI辅助请求摄取** | 客户端的请求者可以使用AI表单填写功能键入提示并附加文件，而不是填写长表单。 系统将该内容映射到表单字段，并显示映射以供审阅。 请求者接受结果并提交表单。 |
| **镜像请求** | 提交的请求将作为只读副本显示在提供商公司的请求区域中，包括自定义字段值。 |
| **请求到项目的转换** | 提供商将请求转化为项目并选择项目组合、项目和模板以开始工作。 提供程序实例中的新对象链接回客户端的原始请求。 请求公司看不到提供商方面的实际工作的详细信息。 |
| **双向评论** | 双方都能看到关于该请求的评论，并且几乎立即收到这些评论，因此双方可以在一个地方达成一致意见。 |
| **请求接受** | 一旦双方同意，提供商就会接受请求，客户就可以看到请求已被接受。 |
| **AI草稿状态更新** | 当请求者在评论中请求状态时，提供者可以使用AI命令快速且一致地生成草稿回复。<br> 草稿包含与请求相关的对象信息，例如计划完成日期、条件和根据计划小时数记录的小时数。<br> 它是最重要的信息的摘要，而不是逐字段导出。 在向客户发送响应之前，人员会对其进行审查和编辑。 |

## 参与Beta

与您的Adobe测试版项目经理联系，参加测试版。

### 我们对参与者的要求

* 加入每周反馈呼叫。

* 每周留出大约一小时用于自行实际测试。 通话中的实时工作会话是一个选项。

* 在可能的情况下，将合作伙伴的观点带入会议。

* 确定要连接的Workfront环境，并为少数Adobe工程师配置管理员帐户，以便他们能够验证连接。

### 我们想要了解的内容

* 镜像对象并仅同步选定的数据是否为正确的共享模型？ 它是否对每一方都有足够的灵活性？

* 阶段排序正确吗？还是应该更早提供后续功能？

* 协作中缺少哪些接触点？

* 字段命名和映射在两个实例之间应如何工作？

  现在，表单和请求由客户端拥有，并且提供商将看到带有客户端字段名称的只读表单。

* IT需要批准和管理什么连接？

## 端到端工作流程

本节介绍参与此集成的两个当事方的工作流。

我们使用客户端和提供程序工作流作为示例。

该工作流包含以下步骤：

1. [创建实例连接](#1-create-an-instance-connection)
1. [确认连接](#2-acknowledge-the-connection)
1. [与连接的组织共享请求表单](#3-share-a-request-form-with-the-connected-organization)
1. [提交请求](#4-submit-a-request)
1. [查看请求并创建项目](#5-review-the-request-and-create-a-project)
1. [跨公司对话中的协作](#6-collaborate-in-the-cross-company-conversation)

### 开始之前

* 您必须是系统管理员，才能在这两个实例中完全访问&#x200B;**安装程序**&#x200B;区域。
* 请求实例需要接收实例的唯一客户&#x200B;**GUID**。
* 必须发布您要共享的表单。

### &#x200B;1. 创建实例连接

在请求实例（客户端）中设置以下内容：

1. 登录到客户端环境，然后转到&#x200B;**设置** > **实例连接**。 该页面列出了所有连接，如果尚不存在任何连接，则该页面为空。
1. 单击&#x200B;**创建连接**。
1. 在&#x200B;**创建连接**&#x200B;框中，添加&#x200B;**接收实例GUID**。 它是必填字段。
1. （可选）设置&#x200B;**到期日期**。 在此日期之后，连接将停止工作。
1. 单击&#x200B;**创建连接**。

   新连接显示在状态为&#x200B;**挂起**&#x200B;的连接列表中。
1. 选择新连接以查看其详细信息。

   >[!TIP]
   >
   >挂起的连接不共享任何内容。 接收实例必须首先确认它。


### &#x200B;2. 确认连接

在接收实例（提供程序）中设置以下内容：

1. 登录到提供程序的实例，然后转到&#x200B;**主菜单** > **设置** > **实例连接**。
1. 单击名称以打开来自接收实例的连接。 横幅显示以下消息： **实例要连接到您的实例。 至少选择一个符合条件的收件人，然后确认连接。 在您执行操作之前不共享任何内容。**
1. 在&#x200B;**符合条件的收件人**&#x200B;下，打开&#x200B;**搜索组和用户**&#x200B;列表，然后选择可从请求实例接收工作的人员。 您可以选择组和单个用户。<!--asking Anna K if this should be teams and users, instead of groups; it's groups in the UI-->
1. 单击&#x200B;**确认**&#x200B;接受连接，或单击下列选项之一：

   * **拒绝**&#x200B;以拒绝连接。
   * **关闭**&#x200B;以使其处于待处理状态。

   出现“更改已保存”消息，并且连接状态更改为&#x200B;**活动**。 该列表现在显示符合条件的收件人、创建日期和到期日期。

   >[!TIP]
   >
   >**Acknowledge**&#x200B;在至少选择一个符合条件的收件人之前保持灰色。

### &#x200B;3. 共享来自请求组织的请求表单

从客户端的Workfront实例中：

1. 转到&#x200B;**主菜单** > **请求**，然后单击&#x200B;**请求表单**。
1. 打开要共享的已发布表单。
1. 单击&#x200B;**共享**。

   注意&#x200B;**共享**&#x200B;框中的以下选项卡：

   * **内部共享**
   * **公共共享**
   * **连接的组织**
1. 打开&#x200B;**连接的组织**&#x200B;选项卡。
1. 在&#x200B;**组织**&#x200B;字段中，选择连接的提供商的实例。
1. 在&#x200B;**用户和组**&#x200B;字段中，选择该组织中可以使用表单的人员。 添加用户和组。
1. 单击&#x200B;**保存**。

**您的更改已成功保存**&#x200B;消息确认共享。<!--need to submit a UI text change - remove "successfully"-->

### &#x200B;4. 提交请求

作为客户端实例中的用户，通过执行以下操作提交请求：

1. 登录客户端的Workfront实例，然后转到&#x200B;**主菜单** > **请求**。

   **提交新请求**&#x200B;页面列出了最近的表单，包括您刚刚共享的表单。

   顶部的注释显示&#x200B;**跨公司请求：使用此表单提交的请求对连接组织可见。**
1. 手动填写表单，或使用&#x200B;**填写表单**&#x200B;让AI为您执行此操作。
1. （可选）要使用填写表单，请执行以下操作：

   1. 单击&#x200B;**填写表单**。
   1. 描述您的请求，粘贴相关电子邮件，或单击&#x200B;**附加文件**&#x200B;以上传文件。 AI查找相关详细信息并将其应用到表单。
   1. 单击&#x200B;**应用到表单**。 进度条显示&#x200B;**正在填写表单**，同时生成字段值。
   1. 要跳过AI步骤，请单击&#x200B;**跳过**。
1. 查看生成的值并编辑任何需要更改的内容。
1. 单击&#x200B;**提交**&#x200B;提交请求。

   已成功提交的&#x200B;**请求**&#x200B;消息显示有&#x200B;**查看您的请求**&#x200B;链接。

   新请求将添加到请求列表中，其表单名称和状态在客户端和提供商的实例上均为&#x200B;**New**。

   >[!TIP]
   >
   >AI响应可能不准确。 提交之前，请始终仔细检查已填充的值。

   创建的请求在提供商的实例上是只读的。

### &#x200B;5. 查看请求并创建项目

1. 登录提供程序的Workfront实例，然后转到&#x200B;**主菜单** > **请求**。

传入请求将显示在列表中。

请求的&#x200B;**Type**&#x200B;标记为&#x200B;**External： &lt;客户端实例的名称>**，这将其标记为来自连接的组织。

1. 打开请求。 标题旁边显示一个&#x200B;**共享对象： &lt;客户端实例的名称>**&#x200B;徽章，评论面板显示以下&#x200B;**跨公司对话**&#x200B;注意事项： **此讨论对&lt;客户端组织的名称>.**&#x200B;可见
1. 查看请求信息和表单答案。
1. 单击请求名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**创建对象**。
1. 在&#x200B;**创建对象**&#x200B;对话框中，更新以下字段：
   * **操作**：从菜单中选择操作。 例如，**创建单个项目**
   * **项目模板**：选择可用的模板。
   * **项目所有者**：添加项目所有者。
   * **模块**：选择要显示对象的产品。 如果选择&#x200B;**工作流**，则会在Workfront的提供程序实例中创建项目。
   * **自定义表单**：根据需要附加自定义表单。
   * **Portfolio**&#x200B;和&#x200B;**计划**：为新项目添加项目组合或计划。
1. 单击&#x200B;**创建**。

   提供程序实例中的请求现在链接到新项目，如果项目处于“当前”状态，则请求的状态将更改为&#x200B;**进行中**。 客户端的请求实例会在自己的请求副本中看到状态更改。

### &#x200B;6. 跨公司对话中的协作

两个组织中的用户都可以对其各自的请求进行评论。 **跨公司对话**&#x200B;横幅提醒其他组织可以看到此处编写的所有内容。

执行下列操作之一：

1. 要从客户端实例请求更新，请执行以下操作：

   1. 打开请求，然后转到&#x200B;**评论**&#x200B;面板。
   1. 单击&#x200B;**新评论**，键入您的消息，然后单击&#x200B;**提交**。

1. 要更新来自提供程序实例的请求，请执行以下操作：

   1. 打开请求。 新评论以&#x200B;**新**&#x200B;标签突出显示。
   1. 单击&#x200B;**回复**，编写回复，然后单击&#x200B;**提交**。

1. 要从客户端的实例进行跟进，请执行以下操作：

   1. 打开请求。 提供商的回复会显示在原始注释下。
   1. 单击&#x200B;**赞**&#x200B;确认它，或单击&#x200B;**添加回复**&#x200B;继续讨论。




<!--
### Client's workflow

As a requestor in the client's organization, you can do the following:  

1. Create or ask an administrator to create a request form, publish it, and share it with the connected provider's organization.

2. Open the published form from the Requests area, enter a prompt, and attach any files.

3. Review how the content maps to the form fields, accept, and submit.

### Provider's workflow

As a work manager in the provider's organization, do the following: 

1. Receive the request in your Requests area as a read-only copy.

2. Discuss the request through comments until both sides are aligned, then accept it.

3. Convert the request into a project, choosing the portfolio, program, and template, if needed.

4. Choose which project fields are mirrored back to the client's request. 

5. Answer status questions in comments, or generate a draft status update, review it, and publish to your request. It will also display on the client's original request. 

    From that point on, the request on the provider's side acts as a replica of the client's original request, so comments and agreed-upon data stay in sync.
-->

## 安全和治理

保护每个组织的数据是一项核心设计要求。

我们希望Beta版建立的一个基准是IT和安全团队可以多么轻松地批准和管理实例之间的连接。

以下是已连接组织工作流的好处：

* **无跨实例访问**：您的实例中不需要合作伙伴组织的用户，因此没有来宾登录和额外的许可证。

* **最低必要共享**：仅共享为同步配置的数据。 其他所有内容都保留在其原始实例中。

* **独立控件**：每个组织保留自己的用户、权限和工作流。

* **团队级别范围**：请求旨在使用现有的Workfront访问控制，仅联系设置为与该客户一起工作的代理团队。

## 路线图展望

以下阶段介绍了我们当前的开发和发布计划。 根据我们在Beta测试阶段学到的内容，排序可能会发生变化。 后来的阶段不是承诺。

<table>
<tbody>
<tr class="odd">
<td><strong>阶段</strong></td>
<td><strong>重点和计划的功能</strong></td>
<td><strong>状态</strong></td>
</tr>
<tr class="even">
<td><strong>阶段1</strong></td>
<td>连接实例并启动工作：请求表单、AI辅助接收、镜像请求、项目转换、评论和状态起草。</td>
<td>测试版</td>
</tr>
<tr class="odd">
<td><strong>阶段2</strong></td>
<td><ul>
<li><p>使用框架和统一的审阅和批准体验进行审阅和批准</p></li>
<li><p>无论利益相关者从事什么工作，待定审核都会显示在Workfront或Frame中</p></li>
<li><p>注释始终与工作文件绑定，因此创意团队可以在一个位置查看反馈</p></li>
</ul></td>
<td>计划</td>
</tr>
<tr class="even">
<td><strong>阶段3</strong></td>
<td><ul>
<li><p>除了请求之外，基于任务的工作分派</p></li>
<li><p>更多自动化状态，通过共享或非共享字段告知</p></li>
<li><p>新的交付项对象类型，其中元数据在简报期间定义并由最终批准的资产继承</p></li>
<li><p>将获得批准的最终资产直接投放到品牌的AEM中，减少了手动元数据输入</p></li>
</ul></td>
<td>计划</td>
</tr>
<tr class="odd">
<td><strong>阶段4</strong></td>
<td><ul>
<li><p>合作伙伴之间共享的上下文</p></li>
<li><p>在审阅前使用Adobe Brand Intelligence <!--by the agency-->，其访问权限由团队控制</p></li>
<li><p>上下文相关的功能，例如估计</p></li>
</ul></td>
<td>长期</td>
</tr>
</tbody>
</table>






<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->