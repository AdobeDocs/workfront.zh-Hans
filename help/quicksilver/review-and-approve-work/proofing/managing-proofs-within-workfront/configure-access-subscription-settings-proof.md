---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: 配置验证的访问和订阅设置
description: 您可以为各个验证配置某些访问和订阅设置，例如是否要求用户登录以及是否允许用户订阅验证。 您可以在创建验证时为其设置访问和订阅设置，也可以为Workfront中已存在的验证设置它们。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 7477b62cf0e2e61966f8e74cf268217e2ceb67ef
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# 配置验证的访问和订阅设置

您可以为各个验证配置某些访问和订阅设置，例如是否要求用户登录以及是否允许用户订阅验证。 您可以在创建验证时为其设置访问和订阅设置，也可以为Workfront中已存在的验证设置它们。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
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
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 创建验证时配置访问和订阅设置

要在创建验证时为其设置访问和订阅设置，请执行以下操作：

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;部分。
1. 单击右上角区域的&#x200B;**新增**。
1. 滚动到&#x200B;**新验证**&#x200B;页面右下角的&#x200B;**验证设置**&#x200B;部分。

1. 配置以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共URL或嵌入代码共享校对</strong> </td> 
      <td>选择此选项后，可以通过公共URL或嵌入代码共享验证。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共URL或嵌入代码订阅证明</strong> </td> 
      <td>选择此选项时，未明确添加到验证的用户可以订阅验证。 订阅验证的用户将获得您在以下设置中定义的角色和电子邮件：
       <ul>
        <li><p><strong>订阅者角色：</strong>分配给订阅了验证的所有审阅人的默认验证角色。 </p><p>重要提示：如果在Workfront Proof设置中将<strong>允许与</strong>共享设置为<strong>所有人</strong>以外的任何设置，则订阅仅适用于组织内的人员。 有关详细信息，请参阅<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中配置校对设置</a>。</p></li>
        <li><strong>订阅者的电子邮件警报设置：</strong>分配给订阅了验证的所有审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接访问验证所需的链接：</strong>配置订阅者是否收到包含验证链接的电子邮件。 您可以选择<strong>无电子邮件</strong> （访问验证不需要电子邮件链接）、<strong>仅验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，无需任何验证）或<strong>验证和验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，必须单击该链接才能访问验证，此选项旨在确保此人输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意：  如果验证已附加自动工作流，则所有订阅都将向验证所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 继续创建您的验证。

## 配置现有校对的访问和订阅设置

要为Workfront中已存在的验证设置访问和订阅设置，请执行以下操作：

1. 在“文档”区域中，选择包含要为其配置设置的校对的文档，然后单击&#x200B;**文档详细信息**。
1. 在左侧面板中，单击&#x200B;**校对查看器设置**。
1. 配置以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共URL或嵌入代码共享校样</strong><strong>e</strong> </td> 
      <td>选择此选项后，可以通过公共URL或嵌入代码共享验证。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>允许通过公共URL或嵌入代码订阅证明</strong> </td> 
      <td>选择此选项时，未明确添加到验证的用户可以订阅验证。 订阅验证的用户将获得您在以下设置中定义的角色和电子邮件：
       <ul>
        <li><p><strong>订阅者角色：</strong>分配给订阅了验证的所有审阅人的默认验证角色。 </p><p>重要提示：如果在Workfront Proof设置中将<strong>允许与</strong>共享设置为<strong>所有人</strong>以外的任何设置，则订阅仅适用于组织内的人员。 有关详细信息，请参阅<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中配置校对设置</a>。</p></li>
        <li><strong>订阅者的电子邮件警报设置：</strong>分配给订阅了验证的所有审阅人的默认电子邮件警报。</li>
       </ul><p>
        <ul>
         <li><strong>通过电子邮件链接访问验证所需的链接：</strong>配置订阅者是否收到包含验证链接的电子邮件。 您可以选择<strong>无电子邮件</strong> （访问验证不需要电子邮件链接）、<strong>仅验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，无需任何验证）或<strong>验证和验证通知电子邮件</strong> （订阅者通过电子邮件接收验证链接，必须单击该链接才能访问验证，此选项旨在确保此人输入了他们有权访问的正确电子邮件地址）。</li>
        </ul><p>注意：  如果验证已附加自动工作流，则所有订阅都将向验证所有者生成确认电子邮件，以便他们决定应将人员添加到哪个阶段。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。
