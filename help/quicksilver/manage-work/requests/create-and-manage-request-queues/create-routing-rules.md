---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建路由规则
description: 路由规则可控制Adobe Workfront在将问题提交到请求队列时对问题执行的操作。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 46c86c1a5e4bb5379409c46669a348ddb53e260b
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# 创建路由规则

<!-- Audited: 12/2023 -->

路由规则可控制Adobe Workfront在将问题提交到请求队列时对问题执行的操作。 有关创建请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

路由规则将问题发送给最适合解决已提交问题或请求的特定用户或工作角色。 路由规则通常与队列主题相关联，这些主题用于控制将哪个路由规则应用于问题或请求。

一旦创建，您就无法将路由规则从一个项目移动到另一个项目。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划</p></td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新许可证： Standard </p> 
   或
   <p>当前许可证：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建路由规则

1. 转到要在其中为请求添加路由规则的项目。
1. 单击左侧面板中的&#x200B;**路由规则**。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**路由规则**。
1. 单击&#x200B;**新建路由规则**&#x200B;以添加新规则。 将打开&#x200B;**新路由规则**&#x200B;框。

   ![新路由规则框](assets/new-routing-rule-box.png)
1. 为传送规则输入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名称</strong> </td> 
      <td>路由规则的名称。 如果您有权查看有关项目的此信息，则可以查看路由规则。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td>添加路由规则的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认被分派人*</strong> </td> 
      <td>添加应将新问题分配给的活动用户或活动工作角色。 此字段只能有一个默认被分配人。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认团队*</strong> </td> 
      <td>添加应将新问题分配给的活动团队。 此字段只能有一个默认团队。

   <p><b>注释</b></p>

   提交问题后，可编辑其分配并分配其他用户、角色或团队。 有关信息，请参阅<a href="../../../manage-work/issues/manage-issues/assign-issues.md">分配问题</a>。

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>项目路由</strong> </td> 
      <td>这是添加问题的项目。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*如果用户、工作角色或团队在与路由规则关联后停用，请求将继续路由到这些用户、工作角色或团队。 您必须定期清点所有路由选择规则，并将已停用的分配替换为有效分配。

   将问题路由到项目时，拥有该问题权限的用户将获得在该项目上设置的权限。 有关设置项目权限的信息，请参阅[在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

1. 单击&#x200B;**保存**。

   此过程仅定义路由规则。 为确保问题在提交到请求队列时得到路由，您必须在&#x200B;**默认路由**&#x200B;下的&#x200B;**队列详细信息**&#x200B;选项卡上选择路由规则。

   有关将默认路由添加到请求队列的信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

   如果要将多个传送规则与请求队列关联，则必须创建多个队列主题，并将每个主题与单独的传送规则关联。 有关创建队列主题的详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。
