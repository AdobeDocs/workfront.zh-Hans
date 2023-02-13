---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 配置校样的访问和订阅设置
description: 您可以为单个校样配置某些访问和订阅设置，例如是否要求用户登录以及是否允许用户订阅校样。 您可以在创建校样时为校样设置访问和订阅设置，也可以为已存在于Workfront中的校样设置它们。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 3%

---

# 配置校样的访问和订阅设置

您可以为单个校样配置某些访问和订阅设置，例如是否要求用户登录以及是否允许用户订阅校样。 您可以在创建校样时为校样设置访问和订阅设置，也可以为已存在于Workfront中的校样设置它们。

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
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 创建校样时配置访问和订阅设置

要在创建校样时设置校样的访问权限和订阅设置，请执行以下操作：

1. 转到要校样的项目、任务或问题，然后单击 **文档** 中。
1. 单击 **新增** 在右上角。
1. 滚动到 **校样设置** 的 **新校样** 页面。

1. 配置以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共 URL 或嵌入代码共享证明</strong> </td> 
      <td>选择此选项后，可通过公共URL或嵌入代码共享校样。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共 URL 或嵌入代码订阅证明</strong> </td> 
      <td>选择此选项后，尚未明确添加到校样的人员可订阅校样。 在以下设置中，校样订阅者将获得您定义的角色和电子邮件：
       <ul>
        <li><p><strong>订阅者角色：</strong> 分配给所有订阅校样的审阅人的默认校样角色。 </p><p>重要信息：如果 <strong>允许与共享</strong> 设置为 <strong>每个人</strong> 在Workfront校样设置中，订阅仅适用于组织内的人员。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校样中配置校样设置</a>.</p></li>
        <li><strong>订阅者的电子邮件警报设置：</strong> 分配给所有订阅校样的审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接进行校样访问时，需要满足以下条件：</strong> 配置订阅者是否收到包含校样链接的电子邮件。 您可以选择 <strong>无电子邮件</strong> （访问校样不需要电子邮件链接）、 <strong>仅校样通知电子邮件</strong> （订阅者通过电子邮件接收指向校样的链接，且未进行任何验证）或 <strong>验证和校样通知电子邮件</strong> （订阅者会通过电子邮件收到指向校样的链接，并且必须单击该链接才能访问校样，此选项旨在确保用户输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意： 如果校样附加了自动工作流，则所有订阅都会向校样所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 继续创建校样。

## 配置现有校样的访问和订阅设置

要设置校样的访问权限和订阅设置，请执行以下操作：Workfront

1. 在“文档”区域中，选择包含要为其配置设置的校样的文档，然后单击 **文档详细信息**.
1. 在左侧面板中，单击 **校对查看器设置**.
1. 配置以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共URL或嵌入代码共享校样</strong><strong>e</strong> </td> 
      <td>选择此选项后，可通过公共URL或嵌入代码共享校样。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共 URL 或嵌入代码订阅证明</strong> </td> 
      <td>选择此选项后，尚未明确添加到校样的人员可订阅校样。 在以下设置中，校样订阅者将获得您定义的角色和电子邮件：
       <ul>
        <li><p><strong>订阅者角色：</strong> 分配给所有订阅校样的审阅人的默认校样角色。 </p><p>重要信息：如果 <strong>允许与共享</strong> 设置为 <strong>每个人</strong> 在Workfront校样设置中，订阅仅适用于组织内的人员。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校样中配置校样设置</a>.</p></li>
        <li><strong>订阅者的电子邮件警报设置：</strong> 分配给所有订阅校样的审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接进行校样访问时，需要满足以下条件：</strong> 配置订阅者是否收到包含校样链接的电子邮件。 您可以选择 <strong>无电子邮件</strong> （访问校样不需要电子邮件链接）、 <strong>仅校样通知电子邮件</strong> （订阅者通过电子邮件接收指向校样的链接，且未进行任何验证）或 <strong>验证和校样通知电子邮件</strong> （订阅者会通过电子邮件收到指向校样的链接，并且必须单击该链接才能访问校样，此选项旨在确保用户输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意： 如果校样附加了自动工作流，则所有订阅都会向校样所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
