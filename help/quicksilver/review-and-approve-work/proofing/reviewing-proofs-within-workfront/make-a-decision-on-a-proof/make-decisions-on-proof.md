---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 在验证查看者中做出验证决策
description: 您可以直接在验证查看器中对验证做出决定。
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# 在验证查看者中做出验证决策

您可以直接在验证查看器中对验证做出决定。

## 访问要求

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
   <td>审批者、查看者和审批者、作者、审查方</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

## 在验证查看者中做出验证决策

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 找到所需的校对，然后单击&#x200B;**打开校对**。

1. 单击验证查看器顶部中央的&#x200B;**做出决策**。

1. 在出现的&#x200B;**验证决策**&#x200B;框中，单击以下决策之一：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">已审批</td> 
      <td>验证已准备好进入自动工作流的下一个阶段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">已批准（附加更改）</td> 
      <td>验证需要做一些更改，但在它进入自动工作流的下一个阶段之前，您不需要查看修订版。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">所需的更改</td> 
      <td>验证需要更改，并且您需要查看另一个修订，然后才能将其移至自动工作流的下一个阶段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不相关</td> 
      <td>该证明与您无关，您无需做出决定。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义决策</td> 
      <td> <p>在Select和Premium计划中，Workfront管理员或Workfront Proof管理员可以重命名、重新排序和隐藏决策。 有关详细信息，请参阅<a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">在Workfront Proof中配置批准决策选项</a>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果Adobe Workfront管理员或Workfront Proof管理员添加了原因部分，请为您的决策选择任何适用的原因。 有关管理员如何配置决策原因的更多信息，请参阅  [在Workfront Proof中配置批准决策选项](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md)。
1. （可选）选择&#x200B;**向我发送电子邮件确认函**，以接收您决策的电子邮件确认函。
1. 单击&#x200B;**做出决定**。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
