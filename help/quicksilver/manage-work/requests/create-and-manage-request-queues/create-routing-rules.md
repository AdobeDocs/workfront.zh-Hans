---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建路由规则
description: 路由规则控制Adobe Workfront在将问题提交到请求队列时对问题执行的操作。 有关创建请求队列的更多信息，请参阅创建请求队列。
author: Alina
feature: Work Management
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# 创建路由规则

路由规则控制Adobe Workfront在将问题提交到请求队列时对问题执行的操作。 有关创建请求队列的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

路由规则将问题发送给最适合解决提交问题或请求的特定用户或作业角色。 路由规则通常与队列主题关联，队列主题用于控制将哪些路由规则应用于问题或请求。

## 访问要求

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请与Workfront管理员联系

## 创建路由规则

1. 转到要为请求添加路由规则的项目。
1. 单击 **路由规则** 中。 您可能需要单击 **显示更多**，则 **路由规则**.
1. 单击 **新路由规则** 以添加新规则。
1. 为路由规则指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名称</strong> </td> 
      <td> <p>路由规则的名称。 如果您有权查看项目中的此信息，则可以查看路由规则。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td>添加路由规则的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认受分派人*</strong> </td> 
      <td>添加应向其分配新问题的活动用户或活动作业角色。 此字段中只能有一个默认代理人。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认团队*</strong> </td> 
      <td>添加一个应将新问题分配给的活动团队。 此字段中只能有一个默认团队。

   <p><b>注释</b></p>

   提交问题后，您可以编辑其分配并分配其他用户、角色或团队。 有关信息，请参阅  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">分配问题 </a>.

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
   >*如果用户、作业角色或团队在与路由规则关联后被停用，则请求将继续被路由到他们。 您必须定期清点所有工艺路线规则，并将停用分配替换为有效分配。

   在将问题路由到某个项目时，对该问题具有权限的用户将收到该项目设置的权限。 有关设置项目权限的信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. 单击&#x200B;**保存**。

   此过程仅定义路由规则。 为确保问题在提交到请求队列时被路由，您必须在 **队列详细信息** 选项卡 **默认路由**.

   有关向请求队列添加默认路由的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   如果要将多个路由规则与请求队列关联，则必须创建多个队列主题，并将每个队列主题与一个单独的路由规则关联。 有关创建队列主题的更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
