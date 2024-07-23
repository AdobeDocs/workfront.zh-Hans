---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 配置个人校对默认值
description: 您可以定义适用于您创建的验证的个人验证默认设置。 每次在Workfront中生成首次验证或上传新验证版本时，都会应用这些默认值。
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# 配置个人校对默认值

您可以定义适用于您创建的验证的个人验证默认设置。 每次在Workfront中生成首次验证或上传新验证版本时，都会应用这些默认值。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或更高版本</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 配置个人校对默认值

{{step1-to-proofing}}

1. 单击右上角的头像，然后选择&#x200B;**个人设置**。
1. 选择&#x200B;**校对默认值**&#x200B;选项卡，然后指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>默认电子邮件通知设置</strong> </td> 
     </tr> 
     <tr> 
      <td>默认电子邮件警报</td> 
      <td>选择用户接收电子邮件更新的频率。 选择“所有活动”、“回复我的评论”、“决策”、“最终决策”、“每小时摘要”、“每日摘要”或“已禁用”。</td> 
     </tr> 
     <tr> 
      <td>新访客审阅人的默认电子邮件警报</td> 
      <td>选择来宾审阅人接收电子邮件更新的频率。 选项与默认电子邮件警报的选项相同。</td> 
     </tr> 
     <tr> 
      <td>新验证通知</td> 
      <td>选择在您被添加到验证时接收通知。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>消息设置</strong> </td> 
     </tr> 
     <tr> 
      <td>校对主题模板</td> 
      <td>键入您希望用户在与他们共享验证时，在电子邮件的主题中看到的内容。</td> 
     </tr> 
     <tr> 
      <td>验证消息模板</td> 
      <td>键入您希望用户在与他们共享验证时在电子邮件正文中看到的内容。</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>默认校对设置</strong> </td> 
     </tr> 
     <tr> 
      <td>作出所有决策时锁定校对</td> 
      <td>选择以在做出所有决策后自动锁定验证以防止进一步更改。</td> 
     </tr> 
     <tr> 
      <td>只需一个决策</td> 
      <td>选择仅要求对验证做出一个决定。</td> 
     </tr> 
     <tr> 
      <td>需要登录</td> 
      <td> <p>选择使该验证仅对具有Workfront Proof登录凭据的用户可用。</p> <p>注意：Workfront Proof凭据可能与您的Workfront凭据不同，除非您的公司用户使用SSO。 我们建议仅在您的公司用户使用SSO时才使用此功能。</p> </td> 
     </tr> 
     <tr> 
      <td>已启用订阅</td> 
      <td>允许组织外部的审阅人通过公共URL或嵌入代码注册验证。 如果选择该选项，订阅者必须单击电子邮件中的链接才能访问校对。 选择此选项可要求外部查看者单击电子邮件中的链接以访问验证。 如果选择了“公共共享”选项，则此选项默认处于启用状态，并应用于此用户创建的所有验证。 </td> 
     </tr> 
     <tr> 
      <td>新来宾审阅人的默认角色</td> 
      <td>为访客审阅人选择默认验证角色。 选项与默认验证角色中的选项相同。</td> 
     </tr> 
     <tr> 
      <td>阻止下载原始文件</td> 
      <td>选择以阻止用户下载原始文件。 </td> 
     </tr> 
     <tr> 
      <td>我的默认验证角色</td> 
      <td>选择您的默认校对角色。 </td> 
     </tr> 
     <tr> 
      <td>我的默认标记颜色</td> 
      <td>选择您的默认标记颜色。 </td> 
     </tr> 
    </tbody> 
   </table>
