---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: 配置AI协作者
description: 作为Adobe Workfront管理员，您可以配置AI协作者，并将其分配给项目和任务。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '1993'
ht-degree: 1%
---
# 配置AI协作者

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。</span>

AI协作者是一种将AI代理载入项目、任务和问题的方式。 您可以配置AI Collaborator，然后像分配用户一样分配它。

例如，您可以使用品牌指南配置审阅人类型的AI Collaborator，然后指定该协作者审阅文档。

可用的AI Collaborator类型包括：

* AI审阅者：使用品牌或Adobe Brand Intelligence创建协作者，然后将该协作者分配为资产审阅者。

  有关详细信息，请参阅[Workfront AI查看器入门](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。

* 工作代理：创建由Adobe CX Coworker </span>提供支持的协作者<span class="preview">或从支持的外部平台连接代理，然后将协作者分配给任务或问题以完成工作项。

  有关详细信息，请参阅[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。

  有关Adobe CX Enterprise Coworker的更多信息，请参阅[Workfront中的CX Enterprise Coworker概述](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)。

AI协作者使用的许可证不收费。 如果贵组织拥有200个Workfront许可证并创建了一个AI协作器，则有201个许可证在使用中，但只计费200个。

* <span class="preview">项目协调员：开箱即用的协作器，用于监视项目状态并发送项目更新，而无需配置外部代理。</span>

  <span class="preview">有关详细信息，请参阅[使用项目协调器协作器](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md)。</span>


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>选择、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[!UICONTROL 标准版]</p>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]或组管理员</span></td> 
  </tr> 
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* [对于AI审阅者](#for-ai-reviewers)
* [对于工作代理](#for-work-agents)

### 对于AI审阅者：

* 贵组织必须存档已签署的Adobe Gen AI协议。

  有关详细信息，请参阅Workfront中的AI Assistant一文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 您必须先在Workfront中配置品牌，然后才能将其用于AI审阅者。

  有关说明，请参阅[为AI审阅者创建和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。
* 要将Adobe Brand Intelligence用于AI审阅人，您的组织必须在Workfront中使用统一的审阅和批准体验。

  有关详细信息，请参阅[统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

### 对于工作代理

<span class="preview">先决条件取决于代理的来源：</span>

* <span class="preview">Adobe Native：您的组织必须启用Adobe CX Coworker。 您不需要在外部平台中配置代理或提供外部平台凭据。</span>
* 外部平台或自定义代理：在Workfront中创建工作代理之前，在计划连接的平台上配置代理。

>[!NOTE]
>
>我们的目标是联系任何代理提供商，因此如果您使用的提供商当前与工作代理不兼容，请联系您的帐户团队寻求帮助。

## 创建新的AI审阅者

AI审阅者可配置为使用Workfront品牌或Adobe Brand Intelligence。

* **品牌**：品牌是在Workfront中创建的。 您可以通过上传包含品牌指南的PDF文件或手动输入品牌元素，在Workfront中创建品牌。
* **Adobe Brand Intelligence**：当AI协作者使用Adobe Brand Intelligence审阅资源时，您可以在Frame.io中查看AI审阅者所做的评论。


{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 单击&#x200B;**审阅者**，然后单击&#x200B;**继续**。
1. 在“协作者名称”字段中，输入协作者的名称。 这是出现在任务可用被分配人列表中的名称。
1. 选择协作者将使用品牌还是Adobe Brand Intelligence进行审阅。
1. （视情况而定）如果AI协作者将使用品牌，请选择它将使用的品牌和品牌指南。
1. 单击&#x200B;**保存**。

## 配置工作代理

<span class="preview">以下安装指南反映了Adobe本机支持和仍在预览中的基于原点的安装模型。</span>

工作代理是可以分配给Workfront中的任务或问题的代理。 使用名称、访问级别和其他详细信息配置工作代理，并将其分配给任务，就像分配用户一样。

由于工作代理是代理，因此会在配置代理的位置配置其操作和功能。 工作代理可以是<span class="preview">使用协同工作的本机工作代理，</span>，也可以来自受支持的外部平台，如Copilot Studio、Claude、OpenAI和IBM。

>可以将工作座席分配给任务或问题。

工作代理使用的许可证不收费。 如果贵组织拥有200个Workfront许可证并创建了一个工作代理，则有201个许可证在使用中，但只收取200个许可证。

有关创建代理以用作工作代理时的最佳实践列表，请参阅[为工作代理创建代理的最佳实践](#best-practices-for-creating-an-agent-for-a-work-agent)。

* [在Workfront中配置工作代理](#configure-a-work-agent-in-workfront)
* [为工作代理创建代理的最佳实践](#best-practices-for-creating-an-agent-for-a-work-agent)

### 在Workfront中配置工作代理

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 选择&#x200B;**工作代理**，然后单击&#x200B;**继续**。
1. 在AI协作者名称字段中，输入协作者的名称。 这是出现在任务可用被分配人列表中的名称。
1. 在AI协作者说明字段中，输入对协作者用途或所执行操作的说明。
1. 在“访问级别”字段中，选择此协作者的访问级别。 此访问级别控制协作者可以执行的操作，与访问级别控制用户可以执行操作的方式相同。
1. （可选）在“组”字段中，选择要与工作代理关联的组。

   >[!NOTE]
   >
   >如果您是组管理员，则此字段仅显示您是其管理员的组。 组管理员必须至少选择一个组。

1. 在&#x200B;**选择代理的来源**&#x200B;区域，选择是要<span class="preview">使用Adobe Native</span>，连接在Copilot等公共平台中创建的代理，还是使用自定义代理。
1. <span class="preview">（视情况而定）如果您选择Adobe Native，请确认已为您的组织启用Adobe CX Coworker，并且您想要使用现成的Adobe Native代理。</span>
1. （视情况而定）如果您使用的是来自公共平台的代理，请输入代理平台的身份验证详细信息：

   | 平台 | 所需的身份验证 |
   |---|---|
   | Copilot Studio | 网页渠道密码 |
   | Claude 托管代理 | 合成API密钥<br>代理ID<br>环境ID |
   | OpenAI 代理 | API密钥<br>代理ID |
   | IBM Watsonx Orchestrate | 服务URL<br>API密钥<br>代理ID |

1. 单击&#x200B;**测试连接**。 这让您知道连接是否正确设置。
1. 在&#x200B;**协作器完成其工作后，它可以**&#x200B;区域中，切换您希望协作器执行的操作。

   * 发送通知：代理在更新流中发表评论，标记请求工作、已分配代理或拥有项目的用户。
   * 上载基于文本的文档
   * 将任务标记为已完成
   * 写入任务字段：选择座席可以写入的表单和字段。
   * 写入项目字段：选择代理可以写入的表单和字段。

1. 单击&#x200B;**保存**。

有关工作代理的详细信息，包括如何将其分配给任务，请参阅[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。

### 为工作代理创建代理的最佳实践

您可能会发现以下最佳实践有助于在Workfront中创建要用作工作代理的代理。 要查看最佳实践，请单击要在其中创建代理的应用程序部分。

+++ Claude

1. 导航到[platform.claude.com](https://platform.claude.com/)上的Claude控制台。
1. 创建API密钥。
   1. 在“API密钥”下，单击右上角的&#x200B;**创建密钥**。
   1. 提供名称和到期日期。
   1. 复制密钥并将其保存在安全的地方。 您需要此密钥才能在Workfront中配置工作代理。

1. 创建环境。
   1. 在&#x200B;**托管代理** > **环境**&#x200B;下，单击右上角的&#x200B;**创建环境**。
   1. 提供适用的名称和托管类型。
   1. 根据需要配置共享包和元数据。 环境可以跨多个代理重用，并允许共享包和元数据。
      环境ID显示在左上角的环境名称下方。

1. 创建代理。
   1. 在托管代理>代理下，单击右上角的&#x200B;**创建代理**。
   1. 提供适用的名称、型号、系统提示、技能和工具。 是描述性的，因为工作代理将任务上下文传递给此代理，然后执行工作。
      代理ID显示在左上角的代理名称下方。

1. 在Workfront中配置工作代理。
   1. 输入您的API密钥、环境ID和代理ID
   1. 单击&#x200B;**测试连接**&#x200B;进行验证。

1. 将工作代理分配给Workfront任务。
   1. 工作代理在所有前置任务完成后触发。

+++
<!--
+++ Copilot Studio


+++
-->
+++ 作者



>[!IMPORTANT]
>
>Writer已弃用代理。 使用Writer代理配置的工作代理在10月9日之后不再工作。 2026.
>
>有关弃用的信息，请参阅Writer文档中的[代理库迁移和弃用](https://support.writer.com/articles/8335689949-migrating-no-code-agents)。


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

+++

<div class="preview">

## 配置项目协调器

项目协调员是一个开箱即用的协作者，负责监控项目状态并帮助使工作按计划进行。 与工作代理不同，项目协调器不要求您配置外部代理。

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 选择&#x200B;**项目协调器**，然后单击&#x200B;**继续**。
1. 在&#x200B;**AI协作器名称**&#x200B;字段中，输入项目协调器的名称。 这是作为协作者显示在项目中的名称。
1. （可选）在&#x200B;**AI Collaborator描述**&#x200B;字段中，输入项目协调器的功能或其用途的描述。
1. 在&#x200B;**访问级别**&#x200B;字段中，选择项目协调器的访问级别。 此访问级别控制协作者在项目上可以执行的操作，与访问级别控制用户可以执行操作的方式相同。
1. （可选）在&#x200B;**组**&#x200B;字段中，选择项目协调员将关联的组。

   >[!NOTE]
   >
   >如果您是组管理员，则此字段仅显示您是其管理员的组。 组管理员必须至少选择一个组。

1. 在&#x200B;**协调器操作**&#x200B;区域中，指定项目协调器发送项目更新的方式。 项目协调器必须具有执行这些操作的权限。 项目协调员还可以对项目及其任务进行评论。

   项目更新可以包括进度摘要、项目运行状况、逾期或存在风险的任务或审批以及缺少字段或分配。

   * 在&#x200B;**节奏**&#x200B;字段中，选择项目协调器是每天发送更新还是每周发送更新。
   * （视情况而定）如果您选择每周，请在&#x200B;**天**&#x200B;字段中，选择在一周中发送更新的日期。
   * 在&#x200B;**时间**&#x200B;字段中，选择发送更新的时间。
   * 在&#x200B;**时区**&#x200B;字段中，选择更新时间的时区。
   * 在&#x200B;**谁获取更新**&#x200B;字段中，选择更新是发送给项目所有者还是项目利益相关者。 默认值为项目所有者。

1. 单击&#x200B;**保存**。

保存项目协调员后，将&#x200B;**项目协调员**&#x200B;字段添加到用户使用的布局模板中的项目标头。 在该字段在标题中可用之前，用户无法将项目协调员分配给项目。

有关说明，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

有关项目协调器的详细信息，包括如何将其分配给项目，请参阅[使用项目协调器协作器](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md)。

</div>

## 管理AI协作者

您可以编辑、复制和删除现有AI协作者。

>[!NOTE]
>
>组管理员只能查看与其作为管理员的组相关联的AI协作者并与之交互。 如果其他组也与给定的AI Collaborator相关联，则组管理员可以查看但不能编辑它。

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. （视情况而定）要编辑Collaborator，请单击要编辑的Collaborator的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要删除协作者，请单击要删除的AI协作者行中的“删除”图标![“删除”图标](assets/delete-collaborator-icon.png)，然后单击&#x200B;**删除**。
