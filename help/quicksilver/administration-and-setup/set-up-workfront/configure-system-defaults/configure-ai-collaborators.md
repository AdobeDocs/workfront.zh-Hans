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
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 2%
---
# 配置AI协作者

AI协作者是一种将AI代理加入您的项目和任务的方法。 您可以配置AI Collaborator，然后像分配用户一样分配它。

例如，您可以使用品牌指南配置审阅人类型的AI Collaborator，然后指定该协作者审阅文档。

可用的AI Collaborator类型包括：

* AI审阅者：使用品牌或Adobe Brand Intelligence创建协作者，然后将该协作者分配为资产审阅者。

  有关详细信息，请参阅[Workfront AI查看器入门](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。

* 工作代理：使用Copilot或Writer创建协作者，然后将协作者分配给任务以完成任务级工作。

  有关详细信息，请参阅[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


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
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

### 对于AI审阅者：

* 贵组织必须存档已签署的Adobe Gen AI协议。

  有关详细信息，请参阅Workfront中的AI Assistant一文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 您必须先在Workfront中配置品牌，然后才能将其用于AI审阅者。

  有关说明，请参阅[为AI审阅者创建和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。
* 要将Adobe Brand Intelligence用于AI审阅人，您的组织必须在Workfront中使用统一的审阅和批准体验。

  有关详细信息，请参阅[统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。

### 对于工作代理

必须先在Claude、Copilot Studio或Writer中配置代理，然后才能将其用作工作代理。

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

工作代理是可以分配给Workfront中任务的代理。 使用名称、访问级别和其他详细信息配置工作代理，并将其分配给任务，就像分配用户一样。

由于工作代理是代理，因此会在配置代理的位置配置其操作和功能。 目前，用作工作代理的代理可以在Copilot Studio、Claude或Writer中创建。

工作座席只能分配给任务，当前不能分配给问题。

有关创建代理以用作工作代理时的最佳实践列表，请参阅[为工作代理创建代理的最佳实践](#best-practices-for-creating-an-agent-for-a-work-agent)。

### 在Workfront中配置工作代理

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 选择&#x200B;**工作代理**，然后单击&#x200B;**继续**。
1. 在AI协作者名称字段中，输入协作者的名称。 这是出现在任务可用被分配人列表中的名称。
1. 在AI协作者说明字段中，输入对协作者用途或所执行操作的说明。
1. 在“访问级别”字段中，选择此协作者的访问级别。 此访问级别控制协作者可以执行的操作，与访问级别控制用户可以执行操作的方式相同。
1. 在&#x200B;**选择代理的来源**&#x200B;区域，选择您要连接在公共平台（如Copilot或Writer）中创建的代理，还是使用自定义代理。
1. （视情况而定）如果您使用的是来自公共平台的代理，请输入代理平台的身份验证详细信息：

   | 平台 | 所需的身份验证 |
   |---|---|
   | Copilot Studio | 网页渠道密码 |
   | Claude 托管代理 | 合成API密钥<br>代理ID<br>环境ID |
   | 作者 | API密钥<br>应用程序ID |

1. 单击&#x200B;**测试连接**。 这让您知道连接是否正确设置。
1. 在&#x200B;**协作器完成其工作后，它可以**&#x200B;区域中，切换您希望协作器执行的操作。
1. 单击&#x200B;**保存**。

有关工作代理的详细信息，包括如何将其分配给任务，请参阅[使用工作代理](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


### 为工作代理创建代理的最佳实践

您可能会发现以下最佳实践有助于在Workfront中创建要用作工作代理的代理。 要查看最佳实践，请单击要在其中创建代理的应用程序部分。

+++ 克劳德

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

>[!NOTE]
>
> 您可以将Writer代理用作工作代理，但不能将Writer行动手册用作工作代理。

创建在Writer中用作工作代理的代理时，我们建议使用以下工作流程。

有关创建代理的更多详细信息可在[Writer文档](https://dev.writer.com/no-code/introduction)中找到。

1. 在Writer AI Studio中创建无代码应用程序。
1. 添加单个文本输入字段。 您可以使用默认名称“文本输入”。
1. 将`@TextInput`添加到您的提示中。 在应用程序配置的提示部分中，确保提示模板引用了输入变量。 如果没有此操作，模型将永远不会看到任务数据。
1. 调整提示以立即生成输出。 删除在响应之前询问用户说明或其他上下文的任何说明。 例如：“收到输入时，将其视为内容生成请求并立即生成输出。 不要要求澄清。”
1. 复制API密钥和应用程序ID。 您需要他们在Workfront中配置工作代理。

   * 有关在Writer中设置API密钥的说明，请参阅Writer文档中的[快速入门](https://dev.writer.com/home/quickstart)。
   * 有关在Writer中设置应用程序ID的说明，请参阅Writer文档中的[通过API调用无代码代理](https://dev.writer.com/home/applications)。

1. 在Workfront中配置工作代理。 作为配置的一部分，输入API密钥和应用程序ID，然后单击&#x200B;**测试连接**&#x200B;以进行验证。
1. 将工作代理分配给Workfront任务。 当任务的所有前置任务完成时，工作代理开始工作。

+++

## 管理AI协作者

您可以编辑、复制和删除现有AI协作者。

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. （视情况而定）要编辑Collaborator，请单击要编辑的Collaborator的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要删除协作者，请单击要删除的AI协作者行中的“删除”图标![“删除”图标](assets/delete-collaborator-icon.png)，然后单击&#x200B;**删除**。
