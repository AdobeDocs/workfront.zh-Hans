---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中查看校样的进度和状态 [!DNL Workfront Proof]
description: 校样进度表示从您向审阅人发送校样到他们决定校样时对校样所做的工作。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# 在中查看校样的进度和状态 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

## 了解校样进度

校样进度表示从您向审阅人发送校样到他们决定校样时对校样所做的工作。

* [进度图标](#progress-icons)
* [验证进度级别](#levels-of-proof-progress)

### 进度图标 {#progress-icons}

进度图标S、O、C和D显示在进度条中，用于指示校样进度。

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

它们指示有关校样的以下信息：

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
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>已发送</strong>. 校样已发送给审阅人。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>已打开</strong>. 审阅人已打开校样详细信息页面或在校样查看器中打开校样本身。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>注释</strong>. 审阅人（可以发表评论的用户）对校样做出了评论。</p> <p>如果没有为校样指定审阅人，则不会显示此图标。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>决定</strong>. 审阅人已经对证据作出决定。</p> <p>如果未为校样指定批准者（决策者），则不会显示此图标。 </p> </td> 
  </tr> 
 </tbody> 
</table>

这些图标可以以下列颜色显示，以指示有关校样进度的特定信息：

* **绿色**. 完成.
* **白色**. 未完成。
* **橙色**. 未完成，截止时间少于24小时。
* **红色**. 没有完成，而且已经过期。

### 验证进度级别 {#levels-of-proof-progress}

Workfront校样使用进度图标跟踪校样在以下每个级别的进度：

* 对于每个审阅人，根据该人在校样上的活动。
* 对于每个阶段，根据校样过程中最落后的阶段上的审阅者的进度。 有关更多信息，请参阅 [自动化工作流阶段概述](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* 对于校样，基于校样过程中最落后的阶段（审阅人组）的进度。

有关如何 [!DNL Workfront Proof] 使用最落后的审阅人或阶段确定进度，假设有三个审核人需要做出决策。 如果其中两人已经作出决定，但第三人没有作出决定，则证明进度条不会因未决决定而绿色显示D。

如果 [!UICONTROL 主要决策者] 在校样上选择设置，主决策者提交决策，校样进度栏中的D对于所有审阅者变为绿色，因为不需要其他决策。

同样，如果 [!UICONTROL 只需要一个决定] 在校样上选择了设置，并且任何审阅人都提交了决策，则校样进度栏中的D对于所有审阅人而言将变为绿色，因为无需其他决策。

## 了解校样状态

校样状态显示校样所需决策的状态。

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
标准状态选项包括：

* 待定
* 已批准
* 有更改的审批
* 所需更改
* 不相关

如果您的帐户中配置了自定义决策，则状态选项将反映您的自定义决策设置。

校样的状态由“最坏大小写”参与者驱动。 例如，假设有三项关于证据的决定：两个的状态为 **已接受** 一个的状态为 **被拒绝**. 被拒绝的“最坏情况”决定对其他决定和证据的整体状态超规则显示为 **被拒绝**.

## 查看进度和状态 {#viewing-progress-and-status}

您可以查看每个阶段的校样、阶段和审阅人的进度和状态。

* [校样摘要](#proof-summary)
* [暂存操作菜单](#stage-actions-menu)
* [在 [!UICONTROL 概要] 部分中，您还可以访问审阅人操作菜单，前提是您对校样具有编辑权限。 有关更多信息，请参阅Workfront校样中的校样权限配置文件和Workfront校样中的管理校样角色。 的 [!UICONTROL 审核者操作] 菜单(1)，在您将鼠标悬停在审阅人的详细信息上时，该菜单允许您：](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [“校样操作”菜单](#proof-actions-menu)

### 校样摘要 {#proof-summary}

文件夹中的每个校样都有一个可扩展的摘要，通过该摘要，您可以快速查看和编辑校样的详细信息。

要展开或折叠摘要，请执行以下操作：

1. 在功能板或任何列表视图中单击校样左侧的箭头。

![Summary_expandable.png](assets/summary-expandable-350x68.png)

摘要包括以下内容：

* 工作流(2)
* 版本(3)
* 文件夹(4)
* 州(5)\
   ![summary_2.png](assets/summary-2-350x160.png)

在摘要中，您可以查看和编辑校样的以下详细信息：

* 验证进度(1)
* 每个阶段(2)的进展
* 为阶段(3)设定的截止日期
* 审阅人详细信息：

   * 每个审阅人的评论和回复数(4)
   * 每个审阅人的进度(5)
   * 决策（如果决策包含电子签名，则决策旁会显示一个图标，指示这一点。） (6)
   * 在证明上的作用(7)
   * 电子邮件警报设置(8)

>[!NOTE]
>
>您编辑校样详细信息的能力取决于您对校样的权限(请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![summary_details_3.png](assets/summary-details-3-350x160.png)

### [!UICONTROL 暂存操作] 菜单  {#stage-actions-menu}

工作流的每个阶段都有一个单独的菜单，允许您执行与该阶段的审阅人相关的批量操作。

的 [!UICONTROL 暂存操作] 将鼠标悬停在Stage部分(1)上时，会显示菜单，并允许您

* [!UICONTROL 全部消息] (2)
* [!UICONTROL 共享] (3)
* [!UICONTROL 删除阶段] (4)

>[!NOTE]
>
>这些选项的可用性取决于您对校样的权限(请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

在“摘要”部分中，您还可以访问审阅人操作菜单，前提是您对校样具有编辑权限。 有关更多信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). 当您将鼠标悬停在审阅人的详细信息上时，将显示“审阅人”操作菜单(1)，并允许您：

* 向审阅人发送消息(2)
* 编辑审阅人的详细信息(3) — 允许您编辑该审阅人的显示名称、校样角色和电子邮件警报
* 让他们成为证据的所有者(4)
* 使他们成为主要决策者（五）
* 从校样(6)中删除

>[!NOTE]
>
>这些选项的可见性取决于您对校样的权限(请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### “校样操作”菜单 {#proof-actions-menu}

每个校样还有一个菜单(1)，用于执行以下操作：

* 您可以访问校样详细信息页面(2)
* 与他人分享证据（三）
* 向审阅人发送邮件(4)
* 创建校样的新版本(5)
* 复制校样(6)
* 下载原始文件(7)
* 共享校样链接(8)
* 打印评论(9)
* 请求校样的Excel摘要(10)
* 锁定校样(11)
* 删除校样(12)

![Proof_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>这些选项的可用性取决于您对校样的权限(请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 和 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md))。

有关在中查看校样进度和状态的信息 [!DNL Workfront]，请参阅 [查看进度和状态](#viewing-progress-and-status).

有关在桌面校对查看器中查看进度和状态的信息，请参阅 [在校样查看器中查看工作流](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
