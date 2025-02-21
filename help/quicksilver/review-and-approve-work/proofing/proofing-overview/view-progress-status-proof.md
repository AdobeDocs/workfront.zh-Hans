---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 校对进度和状态概述
description: 您可以查看有关验证如何在审核过程中进展的信息，并在文档区域查看验证决策状态的整体摘要。
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 1%

---

# 校对进度和状态概述

您可以查看有关验证如何在审核过程中进展的信息，并在文档区域查看验证决策状态的整体摘要。

## 校对进度概述

验证进度指示对验证完成的工作，从您向收件人发送验证到他们对验证做出决定为止。 进度图标S、O、C和D显示在验证名称旁边，并提供有关验证进度的信息。

![人编辑现有进度](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>进度图标</strong> </p> </td> 
   <td> <p><strong>描述</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>已发送</strong> </p> </td> 
   <td> <p>校对已发送给分配的收件人。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>已打开</strong> </p> </td> 
   <td> <p>所有分配的收件人都会打开验证或验证详细信息页面。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>个评论</strong> </p> </td> 
   <td> <p>所有分配的收件人至少对验证进行一项评论。</p> <p>如果没有审阅人分配到校对，则进度条中不会显示<strong>C</strong>图标。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>决策已做出</strong> </p> </td> 
   <td> <p>所有分配的审批者对验证做出决定，所有分配的审批者对验证做出决定，除非验证创建者仅指定了一个决定。</p> <p>如果没有为验证指定的审批者（决策者），则进度条中不会显示<strong>D</strong>图标。 </p> </td> 
  </tr> 
 </tbody> 
</table>

进度图标可以以下列颜色显示，以指示有关校对进度的某些信息：

* **绿色**：完成。
* **白色**：未完成。
* **橙色**：未完成且截止日期不到24小时。
* **红色**：未完成且已超过截止日期。

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## 校对状态概述

验证状态显示验证所需的决策的状态。 证明的状态由“最坏情况”参与者决定。 例如，假设对验证有三个决定：两个决定的状态为&#x200B;**已接受**，另一个决定的状态为&#x200B;**已拒绝**。 **已拒绝**&#x200B;的“最坏情况”决策优先于其他决策，证明的整体状态显示为&#x200B;**已拒绝**。 

![校对编辑现有进度](assets/proof-edit-existing-progress-350x62.png)

标准状态选项如下：

* 待定
* 已审批
* 已批准（附加更改）
* 需要更改
* 不相关

如果您在帐户中配置了自定义决策，则状态选项将反映您的自定义决策设置。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
