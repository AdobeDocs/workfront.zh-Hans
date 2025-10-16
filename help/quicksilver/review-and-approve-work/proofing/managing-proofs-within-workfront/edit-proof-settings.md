---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: 编辑校对设置
description: 在创建验证后，您可以随时编辑验证设置。
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 9%

---

# 编辑校对设置

在创建验证后，您可以随时编辑验证设置。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准</p>
   <p>工作或计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样角色</td> 
   <td>作者或审查方</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 编辑校对设置

如果Workfront管理员在帐户级别禁用了某些设置，则这些设置可能会被锁定。

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;选项卡。
1. 将鼠标悬停在校样上，然后单击&#x200B;**文档详细信息**。
1. 在左侧面板中，单击&#x200B;**校对查看器设置**。
1. 调整以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">需要登录。此证明无法与其他访客用户共享</td> 
      <td> <p>如果您的审阅和批准流程需要更高级别的安全性，则可以使用需要登录到验证。 这意味着只有Workfront用户才能添加到验证中。 用户必须先输入其电子邮件和密码，然后才能访问它。</p> <p>注意： <em style="font-style: normal;">如果启用了需要登录，则无法启用订阅。</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名</td> 
      <td> <p>您可以要求任何对证明做出决定的审阅人的电子签名。 当审核者作出决定时，将出现一条提示，要求他们输入电子邮件和密码并确认其决定。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">作出所有必需的决策时锁定验证</td> 
      <td> <p>您可以将验证状态设置为在最终审批者做出决定时锁定。 如果要确保审阅人无法返回验证并添加其他评论或更改其决策，则此功能非常有用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许下载原文件</td> 
      <td> <p>您可以允许验证上的查看者下载从中创建验证的原始文件。 默认情况下启用此功能。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共 URL 或嵌入代码共享证明</td> 
      <td>您可以允许用户与公共URL或嵌入代码共享验证。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许通过公共 URL 或嵌入代码订阅证明</td> 
      <td> <p>启用验证订阅允许尚未明确添加到验证的用户订阅验证（即，将自己添加到验证）。 然后，将为他们分配您在订阅设置中为他们选择的角色和电子邮件警报。</p> <p>如果对验证启用了订阅，则以下字段将变为活动状态：</p> 
       <ul> 
        <li><strong>需要订阅者验证</strong> — 订阅者必须单击电子邮件中的链接才能访问校样<br>选择此选项意味着订阅者将无法立即访问校样，但会通过电子邮件获得指向校样的链接。 订阅者验证的目的是确保用户输入的电子邮件地址正确无误。</li> 
        <li><strong>新订阅者的默认角色 — </strong>这是将分配给订阅了验证的所有审阅人的默认验证角色。</li> 
        <li><strong>新订阅者的默认电子邮件警报</strong> — 这是将分配给所有订阅了验证的审阅人的默认电子邮件警报。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

 
