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
source-git-commit: 1894bbb5ec7f44f93468c202fb9c07fa656a83cf
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 1%

---

# 配置AI协作者


<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在发布到“预览”版之后，启用了“快速发布”的客户的生产环境中每月还会提供相同的功能。</span>


AI协作者是一种将AI代理加入您的项目和任务的方法。 您可以配置AI Collaborator，然后像分配用户一样分配它。

例如，您可以使用品牌指南配置审阅人类型的AI Collaborator，然后指定该协作者审阅文档。

可用的AI Collaborator类型包括：

* 查看者：使用品牌或Adobe Brand Intelligence创建协作者，然后将协作者分配为资产查看者。

  有关详细信息，请参阅[开始使用Workfront内容审阅者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。

* 任务协作者：使用Copilot或Writer创建协作者，然后将协作者分配给任务以完成任务级工作。

  有关详细信息，请参阅[使用任务协作者](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


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
* 您必须先在Workfront中配置了一个品牌，然后才能将其用于审阅人类型的AI协作者。

  有关说明，请参阅[为内容查看者创建和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。
* 要将Adobe Brand Intelligence用于审阅人AI协作者，您的组织必须在Workfront中使用统一的审阅和批准体验。</span>

  有关详细信息，请参阅[统一审查和批准入门](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)。</span>

<div class="preview">

### 对于任务协作者

必须先在Claude、Copilot Studio或Writer中配置代理，然后才能将其用作任务协作器。

</div>

## 创建新的审阅人类型的AI协作者

可以将Reviewer AI协作者配置为使用Workfront品牌或Adobe Brand Intelligence。

* **品牌**：品牌是在Workfront中创建的。 您可以通过上传包含品牌指南的PDF文件或手动输入品牌元素，在Workfront中创建品牌。
* **Adobe Brand Intelligence**：当AI协作者使用Adobe Brand Intelligence查看资源时，您可以在Frame.io中查看查看查看者所做的评论。 </span>


{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 单击&#x200B;**审阅者**，然后单击&#x200B;**继续**。
1. 在“协作者名称”字段中，输入协作者的名称。 这是出现在任务可用被分配人列表中的名称。
1. 选择协作者将使用品牌还是Adobe Brand Intelligence进行审阅。
1. （视情况而定）如果AI协作者将使用品牌，请选择它将使用的品牌和品牌指南。
1. 单击&#x200B;**保存**。

<div class="preview">

## 配置任务协作者

任务协作者是可以分配给Workfront中的任务的MCP代理。 可以使用名称、访问级别和其他详细信息配置任务协作器，并将其分配给任务，就像分配用户一样。

由于任务协作者是MCP代理，因此其操作和功能会在您配置代理的位置进行配置。 目前，可以在Copilot Studio、Claude或Writer中创建用作任务协作者的代理。

任务协作者只能分配给任务，当前不能分配给问题。

有关创建代理以作为任务协作者使用的最佳实践列表，请参阅[为任务协作者创建代理的最佳实践](#best-practices-for-creating-an-agent-for-a-task-collaborator)。

### 在Workfront中配置任务协作者

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 选择&#x200B;**任务代理**，然后单击&#x200B;**继续**。
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

有关任务协作者的详细信息，包括如何将其分配给任务，请参阅[使用任务协作者](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)。


### 为任务协作者创建代理的最佳实践

您可能会发现，在创建代理以在Workfront中用作任务协作者时，以下最佳实践很有帮助。 要查看最佳实践，请单击要在其中创建代理的应用程序部分。

+++ 克劳德

1. 导航到[platform.claude.com](https://platform.claude.com/)上的Claude控制台。
1. 创建API密钥。
   1. 在“API密钥”下，单击右上角的&#x200B;**创建密钥**。
   1. 提供名称和到期日期。
   1. 复制密钥并将其保存在安全的地方。 您需要此密钥才能在Workfront中配置任务协作器。

1. 创建环境。
   1. 在&#x200B;**托管代理** > **环境**&#x200B;下，单击右上角的&#x200B;**创建环境**。
   1. 提供适用的名称和托管类型。
   1. 根据需要配置共享包和元数据。 环境可以跨多个代理重用，并允许共享包和元数据。
      环境ID显示在左上角的环境名称下方。

1. 创建代理。
   1. 在托管代理>代理下，单击右上角的&#x200B;**创建代理**。
   1. 提供适用的名称、型号、系统提示、技能和工具。 描述性的，因为任务协作者将任务上下文传递给此代理，然后该代理执行工作。
      代理ID显示在左上角的代理名称下方。

1. 在Workfront中配置任务协作器。
   1. 输入您的API密钥、环境ID和代理ID
   1. 单击&#x200B;**测试连接**&#x200B;进行验证。

1. 将任务协作者分配给Workfront任务。
   1. 任务协作器在完成所有前置任务后触发。

+++
<!--
+++ Copilot Studio



+++
-->
+++ 作者

>[!NOTE]
>
> 您可以将Writer代理用作任务协作者，但不能将Writer行动手册用作任务协作者。

在Writer中创建用作任务协作者的代理时，我们建议使用以下工作流。

有关创建代理的更多详细信息可在[Writer文档](https://dev.writer.com/no-code/introduction)中找到。

1. 在Writer AI Studio中创建无代码应用程序。
1. 添加单个文本输入字段。 您可以使用默认名称“文本输入”。
1. 将`@TextInput`添加到您的提示中。 在应用程序配置的提示部分中，确保提示模板引用了输入变量。 如果没有此操作，模型将永远不会看到任务数据。
1. 调整提示以立即生成输出。 删除在响应之前询问用户说明或其他上下文的任何说明。 例如：“收到输入时，将其视为内容生成请求并立即生成输出。 不要要求澄清。”
1. 复制API密钥和应用程序ID。 您需要任务协作者才能在Workfront中配置任务协作者。

   * 有关在Writer中设置API密钥的说明，请参阅Writer文档中的[快速入门](https://dev.writer.com/home/quickstart)。
   * 有关在Writer中设置应用程序ID的说明，请参阅Writer文档中的[通过API调用无代码代理](https://dev.writer.com/home/applications)。

1. 在Workfront中配置任务协作器。 作为配置的一部分，输入API密钥和应用程序ID，然后单击&#x200B;**测试连接**&#x200B;以进行验证。
1. 将任务协作者分配给Workfront任务。 当任务的所有前置任务完成时，协作者开始工作。

+++

</div>

## 管理AI协作者

您可以编辑、复制和删除现有AI协作者。

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. （视情况而定）要编辑Collaborator，请单击要编辑的Collaborator的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要复制Collaborator，请单击要复制的AI Collaborator行中的“复制”图标![复制图标](assets/copy-ai-collaborator.png)，单击副本的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要删除协作者，请单击要删除的AI协作者行中的“删除”图标![“删除”图标](assets/delete-collaborator-icon.png)，然后单击&#x200B;**删除**。
