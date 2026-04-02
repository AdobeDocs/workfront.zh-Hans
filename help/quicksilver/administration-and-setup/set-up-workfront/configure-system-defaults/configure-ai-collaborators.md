---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 配置AI协作者
description: 作为Adobe Workfront管理员，您可以配置AI协作者，并将其分配给项目和任务。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25c4d4435cc3507ab2d163600a8c42be66efd4c2
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 3%

---

# 配置AI协作者

{{highlighted-preview-article-level}}

AI协作者是一种将AI代理加入您的项目和任务的方法。 您可以配置AI Collaborator，然后像分配用户一样分配它。

例如，您可以使用品牌指南配置审阅人类型的AI Collaborator，然后指定该协作者审阅文档。

可用的AI Collaborator类型包括：

* 审阅者：使用品牌或品牌脑创建协作者，然后将协作者指定为资产的审阅者。

  有关详细信息，请参阅[开始使用Workfront内容审阅者](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)。

  >[!NOTE]
  >
  >目前，查看者是唯一可用的AI Collaborator类型。 未来将提供更多的AI协作器功能。


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>Standard、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件



* 贵组织必须存档已签署的Adobe Gen AI协议。

  有关详细信息，请参阅Workfront中的AI Assistant一文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。
* 您必须先在Workfront中配置了一个品牌，然后才能将其用于审阅人类型的AI协作者。

  有关说明，请参阅[为内容查看者创建和管理品牌](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)。

## 创建新的审阅人类型的AI协作者

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. 单击屏幕右上角的&#x200B;**新建Collaborator**。
1. 单击&#x200B;**审阅者**，然后单击&#x200B;**继续**。

   >[!NOTE]
   >
   >目前，仅审阅者类型可用。 未来将提供更多的人工智能协作器类型。

1. 在“协作者名称”字段中，输入协作者的名称。 这是出现在任务可用被分配人列表中的名称。
1. 选择协作者将使用品牌还是品牌大脑进行审阅。
1. （视情况而定）如果AI协作者将使用Brand Brain，请选择它将使用的租户。
1. （视情况而定）如果AI协作者将使用品牌，请选择它将使用的品牌和品牌指南。
1. 单击&#x200B;**保存**。

## 管理AI协作者

您可以编辑、复制和删除现有AI协作者。

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**AI协作者**。
1. （视情况而定）要编辑Collaborator，请单击要编辑的Collaborator的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要复制Collaborator，请单击要复制的AI Collaborator行中的“复制”图标![复制图标](assets/copy-ai-collaborator.png)，单击副本的名称，在“编辑Collaborator”窗口中进行任何编辑，然后单击&#x200B;**保存**。
1. （视情况而定）要删除协作者，请单击要删除的AI协作者行中的“删除”图标![“删除”图标](assets/delete-collaborator-icon.png)，然后单击&#x200B;**删除**。
