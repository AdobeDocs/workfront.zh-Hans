---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 编辑校样设置
description: 您可以在创建校样后随时编辑校样设置。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 7%

---

# 编辑校样设置

您可以在创建校样后随时编辑校样设置。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
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

## 编辑校样设置

如果Workfront管理员在帐户级别禁用了某些设置，则这些设置可能会被锁定。

1. 转到要校样的项目、任务或问题，然后单击 **文档** 选项卡。
1. 将鼠标悬停在校样上，然后单击 **文档详细信息**.
1. 在左侧面板中，单击 **校对查看器设置**.
1. 调整以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录。此证明无法与其他访客用户共享</td> 
      <td> <p>如果您的审阅和批准流程需要更高级别的安全性，则可以使用要求登录校样。 这意味着只能将Workfront用户添加到校样中。 用户必须输入其电子邮件和密码，才能访问。</p> <p>注意： <em style="font-style: normal;">如果启用了“需要登录”，则无法启用“订阅”。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td> <p>您可以要求对证明做出决策的任何审阅人的电子签名。 当审阅人做出决策时，会出现一条提示，要求他们输入其电子邮件和密码并确认其决定。 <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在做出所有必需的决策时锁定验证</td> 
      <td> <p>您可以设置校样状态，以在最终审批者做出决策时将其锁定。 如果您希望确保审阅人无法返回到校样并添加其他注释或更改其决策，则此功能非常有用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许下载原文件</td> 
      <td> <p>您可以允许校样的审阅人下载从中创建校样的原始文件。 默认情况下，此设置处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共 URL 或嵌入代码共享证明</td> 
      <td>您可以允许用户与公共URL或嵌入代码共享校样。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共 URL 或嵌入代码订阅证明</td> 
      <td> <p>启用校样订阅功能后，尚未明确添加到校样的用户便可以订阅校样（即将自己添加到校样中）。 然后，会为他们分配您在订阅设置中为其选择的角色和电子邮件警报。</p> <p>如果校样已启用订阅，则以下字段将变为活动字段：</p> 
       <ul> 
        <li><strong>需要订阅者验证</strong>  — 订阅者必须单击电子邮件中的链接才能访问校样<br>选择此选项意味着订阅者无法立即访问校样，但会在电子邮件中获得指向校样的链接。 订阅者验证的目的是确保用户输入了他们有权访问的正确电子邮件地址。</li> 
        <li><strong>新订阅者的默认角色 — </strong> 这是默认的校样角色，将分配给所有订阅校样的审阅人。</li> 
        <li><strong>新订阅者的默认电子邮件警报</strong>  — 这是默认的电子邮件警报，将分配给所有订阅校样的审阅人。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

 
