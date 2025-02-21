---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 向审核者发送有关验证的电子邮件
description: 在审阅和批准过程中，您可以向验证上的一个或多个审阅人发送消息。 消息是一种提醒审阅人完成审阅验证或提供与验证相关的其他信息的简单方法。
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 1%

---

# 向审核者发送有关验证的电子邮件

在审阅和批准过程中，您可以向验证上的一个或多个审阅人发送消息。 消息是一种提醒审阅人完成审阅验证或提供与验证相关的其他信息的简单方法。

您可以选择发送通用提醒电子邮件，还是向与给定阶段关联的一个或多个用户发送自定义消息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">验证角色</td> 
   <td>作者或审查方</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 向用户发送有关验证的电子邮件

1. 查找包含要向其发送消息的用户的验证文档。
1. 将鼠标悬停在文档上，然后单击&#x200B;**校对工作流**。

   ![校对工作流](assets/proof-workflow-doc-list-350x92.png)

1. 若要向舞台上的所有用户发送消息，请单击舞台上的&#x200B;**更多**&#x200B;菜单，然后选择&#x200B;**全部发送消息**。

   阶段](assets/message-stage-350x122.png)上的![消息

1. 若要向单个用户发送消息，请单击该用户旁边的&#x200B;**更多**&#x200B;菜单，然后选择&#x200B;**消息**。

   ![消息用户](assets/message-user-350x121.png)

1. 在&#x200B;**消息详细信息**&#x200B;部分中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">通过电子邮件通知用户</td> 
      <td>无法取消选择此选项。 所有用户都通过电子邮件接收消息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">放弃自定义消息</td> 
      <td> <p>如果要仅包含默认电子邮件内容，请单击<strong>放弃自定义邮件</strong>。</p> <p>默认提醒电子邮件包含以下信息：</p> 
       <ul> 
        <li>证明的个人链接<br>证明图像的缩略图<br></li> 
        <li>以下验证详细信息：验证名称、版本号、文件夹名称（如果适用）以及查看者列表及其在验证中的进度。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">主题</td> 
      <td>键入消息主题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">消息</td> 
      <td>键入消息内容。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**发送。**
