---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置默认校样设置
description: 利用这些设置，可设置应用于用户创建的所有新校样的默认值。 但是，用户在创建校样时可以覆盖其中大多数设置。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# 配置默认校样设置

利用这些设置，可设置应用于用户创建的所有新校样的默认值。 但是，用户在创建校样时可以覆盖其中大多数设置。

## 配置新的校样默认设置

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置**.
1. 在左侧面板中，单击 **校样** > **校样设置**.
1. 在 **新校样默认值** ，请配置以下设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>收件人</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">需要登录</td> 
      <td> <p>审阅人必须使用其电子邮件和密码登录，然后才能查看在您组织的帐户中创建的校样。 启用后，用户将无法与来宾审阅人共享校样。</p> <p><b>重要信息</b>:启用后，所有新创建的校样都需要登录。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">从新版本的原始证明中复制所有者</td> 
      <td> <p>验证的第一个版本的所有者也是验证所有连续版本的所有者，无论是谁创建了这些版本。 默认情况下，此设置处于启用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许用户删除其验证注释</td> 
      <td>用户可以删除自己的评论。 默认情况下，此设置处于启用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">要求对决策进行电子签名 </td> 
      <td> <p>决策者在做出校样决策时，系统会提示输入其Workfront登录凭据。</p> <p><b>重要信息</b>:启用后，用户将无法与没有登录凭据的来宾审阅人共享校样。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>截止日期</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">设置默认截止时间</td> 
      <td> <p>系统将此截止日期应用于您帐户中没有自动工作流的所有新校样。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在举证前通知收件人有风险</td> 
      <td>根据上面指定的截止时间，在将校样视为有风险之前，会通过电子邮件通知收件人。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>电子邮件通知</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">当收件人被添加到证明中时通知他们</td> 
      <td>将收件人添加到校样时，会通过电子邮件通知他们。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

## 配置校样决策

用户可以使用校样决策来指示审阅后校样的状态。

>[!NOTE]
>
>如果存在多个不同级别的决策，则验证决策背后的逻辑用于计算验证工作流的整体状态。 “已批准”和“已通过更改批准”决策将触发自动工作流程的下一个阶段。

要配置校样决策，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置**.
1. 在左侧面板中，单击 **校样** > **校样设置**.
1. 在 **决策**&#x200B;部分，您可以

   1. **重命名决策**:单击决策框内的文本，然后开始键入新的决策标签。

      >[!TIP]
      >
      >在重命名决策时保留决策逻辑。 例如，可以将“已拒绝”的默认决策更改为 *需要新版本*，但不应将其更改为 *发送到打印机*.

      ![](assets/rename-decision-350x109.png)

   1. **重新排列决策顺序**:按照您希望决策框在校样查看器中显示的顺序拖动决策框。

      ![](assets/move-decision-350x110.png)

   1. **隐藏决策**:将鼠标悬停在决策框上，然后单击右上角的隐藏图标。

      ![](assets/hide-decision-350x109.png)

1. （可选）要返回到Workfront默认值，请单击 **还原默认值**.
1. 单击&#x200B;**保存**。
