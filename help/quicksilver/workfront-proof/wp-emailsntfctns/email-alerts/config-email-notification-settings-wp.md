---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 在 [!DNL Workfront Proof]中配置电子邮件通知设置
description: 从Workfront Proof生成的电子邮件通知会通知协作者最近有关验证的活动，如评论、回复或决策。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2065'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中配置电子邮件通知设置

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

电子邮件通知会通知协作者最近有关验证的活动，例如评论、回复或决策。

您可以在以下区域为审阅人设置电子邮件通知：

可以在新验证页面[!UICONTROL 新版本]页面上设置查看者的电子邮件通知，并在[!UICONTROL 验证详细信息]页面的[!UICONTROL 工作流]部分中进行管理。 有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证

* 新验证页面
* [!UICONTROL 新版本]页面
* [!UICONTROL 校对详细信息]页面的[!UICONTROL 工作流]部分。

有关详细信息，请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证


* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)中生成验证

* [在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。


每个用户还可以设置自己的电子邮件警报设置，如果协作者拥有自己的偏好或帐户管理员拥有对警报频率的推荐，则在与他们共享验证时，会自动应用这些设置。 可在用户详细信息页面上将此项设置为验证默认值。

每个用户也可以设置自己的电子邮件警报设置，当与其共享验证时，将自动应用这些设置。<!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>当用户创建验证并添加这些协作者时，建议使用这些设置。 但是，这些只是建议，因此在审阅过程中可随时调整这些建议，并且所做的更改适用于更改后进行的所有活动。 验证默认设置由验证级别的设置覆盖。

具有[!UICONTROL 管理员]或[!UICONTROL 计费管理员]配置文件的用户还可以在“帐户”设置中为帐户中的其他用户设置验证默认值。

有关配置文件的信息，请参阅 [!DNL Workfront Proof][&#128279;](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)中的验证权限配置文件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">产品</td> 
   <td>Workfront Proof Standalone</td> 
  </tr> 
</table>

+++

## 在个人设置中配置校对默认值（仅限[!DNL Workfront Proof]个用户）

您可以为创建的验证配置验证设置。

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. 单击右上角的个人资料图片，然后单击&#x200B;**[!UICONTROL 个人设置]**。

1. 单击&#x200B;**[!UICONTROL 校对默认值]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 默认电子邮件通知设置]**&#x200B;以展开它。
1. 在下面两个设置右侧的下拉列表中，选择下表说明的选项之一。

   * **[!UICONTROL 默认电子邮件警报]**：影响与您共享的每个验证。 可以在验证级别覆盖此设置。
   * **[!UICONTROL 新来宾审阅人的默认电子邮件警报]**：影响以前不作为联系人存在于您帐户中的审阅人。

   >[!NOTE]
   >
   >如果您未选择以下选项之一，[!DNL Workfront Proof]将向您发送有关校样活动的每日摘要。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 所有活动]</td> 
      <td>每次验证上发生任何活动（如新评论、回复或决策）时，[!UICONTROL Workfront]都会向查看者发送电子邮件。 <p>这是管理校对流程的人员的最佳选项，因为它允许他们查看活动发生的情况。 </p><p>用户不会收到有关其活动的电子邮件警报。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 回复我的评论]</td> 
      <td>只有当某人明确回复其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着如果验证中的某人发表新评论，则不会通知查看者。<p>建议向验证上的客户使用此设置，以便他们不会收到有关验证的任何其他评论的通知，并且只会在回复他们自己的评论时收到通知。</p><p>虽然具有此电子邮件警报设置的查看者不会收到有关其他新评论的通知，但他们仍然可以在验证查看器中查看有关验证的所有评论。</p><p>有关评论的信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校对评论</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 决策]</td> 
      <td>[!DNL Workfront] 仅当有人作出决定时向审阅人发送电子邮件。<p>这对于管理审批流程的人员（如项目经理）非常有用，他们需要监控验证进度并查看哪些用户做出了决定。</p><p>除非您在提交决策时选择了电子邮件确认选项，否则不会通知您自己的决策。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 最终决定]</td> 
      <td>[!DNL Workfront] 当验证的最后一位审批者做出决定时会发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审核讨论。 当做出最终决定时，设计人员会收到通知，然后可以对任何必要的更改执行操作。</p><p>此警报对于需要仅在审核流程完成后才收到通知的部门领导也很有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 小时摘要]</td> 
      <td>[!DNL Workfront] 每小时向查看者发送一封电子邮件，其中包含该小时发生的所有评论、回复和决策的摘要。<p>仅当过去一小时内发生除您自己的活动以外的活动时，才会发送电子邮件。 </p><p>此警报非常适合用于查看项目概述。</p><p>此摘要的示例用例是高级查看者，他需要项目概述，但不需要立即收到有关验证中所有活动的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 每日摘要]</td> 
      <td>[!DNL Workfront] 仅当您有其他活动时，才会发送一封电子邮件，其中包含列出的所有评论、回复和决策。<p>此警报非常适合用于查看项目摘要，而不会在一天之内出现多次更新。</p><p>此摘要的示例用例是一个部门领导，他想要监控项目的整体进度。</p><p>有关详细信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理证明评论和决策的通知</a>。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 无电子邮件]</td> 
      <td>[!DNL Workfront] 不发送任何电子邮件警报。<br>这对于仅供参考而添加到验证中且不需要收到任何更改通知的人员非常有用。<p>系统默认值为[!UICONTROL Daily summary] （也称为[!UICONTROL 未设置]）。 如果您或您的审阅人没有进行任何其他更改，则您的所有验证均具有此设置。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 更改以下任一项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 验证就绪时电子邮件确认]</td> 
      <td>指定在创建验证时是否要接收[!UICONTROL Proof maked]电子邮件。 有关详细信息，请参阅<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">已做出[!UICONTROL 校对]电子邮件</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 发送给我的电子邮件格式] </td> 
      <td> <p>在HTML样式电子邮件和纯文本电子邮件之间进行选择。 </p> <p><b>注释</b></p>
      <p>校对默认设置被校对级别的设置覆盖。 但是，如果在[!UICONTROL 帐户]设置中为整个帐户禁用了验证电子邮件通知，那么即使未在验证中选择[!UICONTROL 禁用的电子邮件警报]，也不会向协作者发送电子邮件警报。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在&#x200B;**[!UICONTROL 消息设置]**&#x200B;下，更改以下任一设置：

   | 校对模板 | 描述 |
   |---|---|
   | **[!UICONTROL 校对主题模板]** | 显示在新验证页面、新版本页面、消息页面和提醒页面上。 可以在发送之前进行编辑。 |
   | **[!UICONTROL 校对消息模板]** | 显示在新验证页面、新版本页面、消息页面和提醒页面上。 可以在发送之前进行编辑。 |

## 更改收件人的电子邮件警报

您可以在批处理操作中更改特定收件人的电子邮件警报。

1. 单击左侧导航面板中的&#x200B;**[!UICONTROL 联系人]**。
1. 单击收件人的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多菜单](assets/more-button-small.png)，然后在下拉菜单中单击&#x200B;**[!UICONTROL 查看成员详细信息]**。

1. 打开&#x200B;**[!UICONTROL 共享项]**&#x200B;部分。
1. 选中要更改其电子邮件警报的每个项目左侧的复选框。
1. 单击共享项目列表上方的&#x200B;**[!UICONTROL 更多]**，然后在下拉菜单中单击&#x200B;**[!UICONTROL 更改电子邮件警报]**。

1. 更改电子邮件警报，然后单击&#x200B;**[!UICONTROL 提交]**。

## 为用户配置校对默认值

如果您是[!DNL Workfront Proof]管理员，则可以设置帐户中用户的验证默认值。

1. 单击屏幕顶部的&#x200B;**[!UICONTROL 帐户设置]**。

1. 打开&#x200B;**[!UICONTROL 用户]**&#x200B;选项卡。
1. 打开用户名右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多_button_small.png](assets/more-button-small.png)。

1. 在下拉菜单中单击&#x200B;**[!UICONTROL 查看用户详细信息]**。
1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;下，单击&#x200B;**[!UICONTROL 默认电子邮件警报设置]**&#x200B;以展开它。

1. 在下列两个设置右侧的下拉列表中，选择下表说明的选项之一：

   * **[!UICONTROL 默认电子邮件警报]**：影响与您共享的每个验证。 可以在验证级别覆盖此设置。
   * **[!UICONTROL 新来宾审阅人的默认电子邮件警报]**：影响以前不作为联系人存在于您帐户中的审阅人。

   >[!NOTE]
   >
   >如果您没有为用户选择以下选项之一，[!DNL Workfront Proof]会向用户发送有关其验证活动的每日摘要。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL 所有活动]</td>
      <td>[!DNL Workfront] 每次在验证上发生任何活动（如新评论、回复或决策）时，向查看者发送电子邮件。 <p>这是管理校对流程的人员的最佳选项，因为它允许他们查看活动发生的情况。 </p><p>用户不会收到有关其活动的电子邮件警报。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 回复我的评论]</td>
      <td>只有当某人明确回复其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着如果验证中的某人发表新评论，则不会通知查看者。<p>建议向验证上的客户使用此设置，以便他们不会收到有关验证的任何其他评论的通知，并且只会在回复他们自己的评论时收到通知。</p><p>虽然具有此电子邮件警报设置的查看者不会收到有关其他新评论的通知，但他们仍然可以在验证查看器中查看有关验证的所有评论。</p><p>有关评论的信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校对评论</a>。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 决策]</td>
      <td>[!DNL Workfront] 仅当有人作出决定时向审阅人发送电子邮件。<p>这对于管理审批流程的人员（如项目经理）非常有用，他们需要监控验证进度并查看哪些用户做出了决定。</p><p>除非您在提交决策时选择了电子邮件确认选项，否则不会通知您自己的决策。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 最终决定]</td>
      <td>[!DNL Workfront] 当验证的最后一位审批者做出决定时会发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审核讨论。 当做出最终决定时，设计人员会收到通知，然后可以对任何必要的更改执行操作。</p><p>此警报对于需要仅在审核流程完成后才收到通知的部门领导也很有用。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 小时摘要]</td>
      <td>[!DNL Workfront] 每小时向查看者发送一封电子邮件，其中包含该小时发生的所有评论、回复和决策的摘要。<p>仅当过去一小时内发生除您自己的活动以外的活动时，才会发送电子邮件。 </p><p>此警报非常适合用于查看项目概述。</p><p>此摘要的示例用例是高级查看者，他需要项目概述，但不需要立即收到有关验证中所有活动的通知。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL 每日摘要]</td>
      <td>[!DNL Workfront] 仅当您有其他活动时，才会发送一封电子邮件，其中包含列出的所有评论、回复和决策。<p>此警报非常适合用于查看项目摘要，而不会在一天之内出现多次更新。</p><p>此摘要的示例用例是一个部门领导，他想要监控项目的整体进度。</p><p>有关详细信息，请参阅<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理证明评论和决策的通知</a>。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL 无电子邮件]</td>
      <td>[!DNL Workfront] 不发送任何电子邮件警报。<br>这对于仅供参考而添加到验证中且不需要收到任何更改通知的人员非常有用。<p>系统默认值为[!UICONTROL Daily summary] （也称为[!UICONTROL 未设置]）。 如果您或您的审阅人没有进行任何其他更改，则您的所有验证均具有此设置。</p></td>
     </tr>
    </tbody>
   </table>

1. 在其余&#x200B;**[!UICONTROL 默认电子邮件警报设置]**&#x200B;中，更改以下任一设置：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 验证就绪时电子邮件确认]</td> 
      <td>指定在创建验证时是否要接收[!UICONTROL Proof maked]电子邮件。 有关详细信息，请参阅<a href="https://support.workfront.com/hc/en-us/article">已做出[!UICONTROL 校对]电子邮件。</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 发送给我的电子邮件格式] </td> 
      <td> <p>在HTML样式电子邮件和纯文本电子邮件之间进行选择。 </p> <p><b>注释</b></p> <p>校对默认设置被校对级别的设置覆盖。 但是，如果在[!UICONTROL 帐户]设置中为整个帐户禁用了验证电子邮件通知，那么即使未在验证中选择[!UICONTROL 禁用的电子邮件警报]，也不会向协作者发送电子邮件警报。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
