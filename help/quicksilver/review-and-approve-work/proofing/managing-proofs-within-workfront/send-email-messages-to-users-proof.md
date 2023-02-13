---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 通过校样向审阅人发送电子邮件
description: 在审阅和批准过程中，您可以向一个或所有审阅人发送关于校样的消息。 邮件是提醒审阅人完成校样审阅或提供与校样相关的其他信息的简便方法。
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# 通过校样向审阅人发送电子邮件

在审阅和批准过程中，您可以向一个或所有审阅人发送关于校样的消息。 邮件是提醒审阅人完成校样审阅或提供与校样相关的其他信息的简便方法。

您可以选择发送一般提醒电子邮件还是向与给定阶段关联的一个或多个用户发送自定义消息。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样角色</td> 
   <td>作者或审核者</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 通过校样向用户发送电子邮件

1. 查找包含要消息的用户的校样文档。
1. 将鼠标悬停在文档上，然后单击 **校对工作流**.

   ![](assets/proof-workflow-doc-list-350x92.png)

1. 要向舞台上的所有用户发送消息，请单击 **更多** 菜单，然后选择 **全部消息**.

   ![](assets/message-stage-350x122.png)

1. 要向个人用户发送消息，请单击 **更多** 菜单，然后选择 **消息**.

   ![](assets/message-user-350x121.png)

1. 在 **消息详细信息** ，请指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">通过电子邮件通知用户</td> 
      <td>无法取消选择此选项。 所有用户都会通过电子邮件收到该消息。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">放弃自定义消息</td> 
      <td> <p>单击 <strong>放弃自定义消息</strong> 如果您只想包含默认的电子邮件内容，请执行以下操作：</p> <p>默认提醒电子邮件包含以下信息：</p> 
       <ul> 
        <li>证明的个人链接<br>校样图像的缩略图<br></li> 
        <li>以下校样详细信息：校样名称、版本号、文件夹名称（如果适用），以及审阅人列表及其校样进度。</li> 
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

1. 单击 **发送。**
