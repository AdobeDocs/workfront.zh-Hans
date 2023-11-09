---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 编辑校样阶段和审阅者
description: 了解如何编辑校样阶段和审阅者。
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# 编辑校样阶段和审阅者

如果您是验证所有者或创建者或者您分配了正确的验证角色，则可以在验证中编辑阶段和查看者详细信息。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关验证不同计划的访问权限的详细信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">验证角色</td> 
   <td>作者或审查方 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

## 编辑阶段

1. 在包含该文档的文档列表中，将鼠标悬停在包含该文档的行上，然后单击 **校对工作流**.

   或

   在独立的Workfront Proof中，单击 **更多** （三个点）菜单位于验证右侧，然后单击 **查看校对详细信息**.

1. 在中进行以下任何更改 **工作流** 部分：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">编辑截止日期</td> 
      <td> <p>选择日期，然后在显示的日历中选择一个新日期。 要完全删除截止日期，请选择日期，然后选择 <strong>清除</strong> 在显示的日历下方。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除审阅人</td> 
      <td> <p>选择 <strong>更多</strong> 查看者名称右侧的菜单，然后单击 <strong>移除</strong> （在下拉菜单中）。 单击 <strong>确认</strong> 在显示的框中，从验证中移除查看者。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除多个审阅人</td> 
      <td>选中名称旁边的复选框，然后单击 <strong>删除</strong> 图标（位于舞台部分的右上角附近）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">向所有审阅人发送消息</td> 
      <td>选择 <strong>更多</strong> 菜单，然后选择 <strong>发送消息给所有人</strong>. 配置消息，然后选择 <strong>发送</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">向阶段添加审阅者</td> 
      <td>选择 <strong>更多</strong> 菜单，然后选择 <strong>共享</strong>. 添加用户并配置其角色和电子邮件警报，然后根据需要重复此操作。 完成后，单击 <strong>共享</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除阶段</td> 
      <td> <p>选择 <strong>更多</strong> 菜单，选择 <strong>删除</strong> 暂存。</p> <p>注意：如果只有一个阶段，则无法删除该阶段。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 编辑审阅者详细信息

1. 在Workfront中，将鼠标悬停在验证上，然后单击 **校对详细信息** 以打开验证详细信息页面。
1. 在 **工作流** 部分，单击 **更多** 菜单 ![](assets/more-button-small.png) 查看者名称右侧，然后单击 **编辑** 在出现的下拉菜单中。

1. 在 **编辑审阅者** 框中，编辑以下任何详细信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">显示名称*</td> 
      <td> <p>要更改校样上查看者的显示名称，请单击文本字段并内联编辑其名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">角色</td> 
      <td>要更改查看者在验证中的角色，请打开下拉菜单并选择首选角色。 有关详细信息，请参阅。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">电子邮件警报</td> 
      <td>要更改验证上查看者的电子邮件警报，请打开下拉菜单并选择首选电子邮件警报。 有关更多信息，请参阅文章中的 <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">验证评论和决策通知概述</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">决定*</td> 
      <td> <p>要更改查看者在验证上的决策，请打开下拉菜单并选择首选决策。 请注意，您代表其他用户做出的任何决策都记录在验证的活动部分中。 仅当审核做出决定时才会显示此选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段</td> 
      <td>无法在阶段之间移动审阅人。 但是，您可以删除并重新添加具有不同截止时间的审阅人。</td> 
     </tr> 
    </tbody> 
   </table>

   &#42; 您必须是校对创建者或所有者才能编辑此字段。

1. 单击&#x200B;**保存**。
