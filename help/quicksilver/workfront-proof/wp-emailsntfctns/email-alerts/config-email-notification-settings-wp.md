---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: 在中配置电子邮件通知设置 [!DNL Workfront Proof]
description: 电子邮件通知会向协作者告知有关校样（如评论、回复、决策）的最近活动。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# 在中配置电子邮件通知设置 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

电子邮件通知会向协作者告知有关校样（如评论、回复、决策）的最近活动。

可以在New proof页面上为审阅人设置电子邮件通知， [!UICONTROL 新版本] 页面，并在中管理 [!UICONTROL 工作流] 部分 [!UICONTROL 校样详细信息] 页面。 有关更多信息，请参阅 [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [在中生成校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

每个用户还可以设置自己的电子邮件警报设置，当与他们共享校样时，该设置将自动应用。 如果协作者有其偏好，或帐户管理员有其警报频度推荐。 这可以设置为用户详细信息页面上的校样默认值。

>[!NOTE]
>
>当用户创建校样并添加这些协作者时，建议使用这些设置。 但是，这些只是建议，因此可以在审核过程中随时对其进行调整，这些更改适用于更改后进行的所有活动。 校样默认设置由校样级别的设置覆盖。

具有 [!UICONTROL 管理员] 或 [!UICONTROL 帐单管理员] 用户档案还可以在“帐户”设置中为其帐户中的其他用户设置校样默认值。

有关用户档案的信息，请参阅 [中的校样权限配置文件 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [在个人设置中配置校样默认值([!DNL Workfront Proof] 仅限用户)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [更改收件人的电子邮件警报](#change-email-alerts-for-a-recipient)
* [为用户配置校样默认值](#configure-proof-defaults-for-a-user)

## 在个人设置中配置校样默认值([!DNL Workfront Proof] 仅限用户)

您可以为创建的校样配置校样设置。

有关校样设置的信息，请参阅 [!DNL Workfront] 管理员或 [!DNL Workfront Proof] 管理员可以配置，请参阅。

1. 单击 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**.

1. 单击 **[!UICONTROL 校对默认值]** 选项卡。
1. 单击 **[!UICONTROL 默认电子邮件通知设置]** 来扩展。
1. 在以下两个设置右侧的下拉列表中，选择下表中介绍的选项之一。

   * **[!UICONTROL 默认电子邮件警报]**:影响与您共享的每个校样。 可以在校样级别覆盖此设置。
   * **[!UICONTROL 新来宾审阅人的默认电子邮件警报]**:影响以前不作为帐户联系人存在的审阅人。

   >[!NOTE]
   >
   >如果不选择以下选项之一， [!DNL Workfront Proof] 会向您发送有关校样活动的每日摘要。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All activity]</td> 
      <td>每当校样中存在任何活动（如新评论、回复或决定）时，[!UICONTROL Workfront]都会向审阅人发送电子邮件。 <p>对于管理校对流程的人员而言，这是一个非常好的选项，因为它允许他们查看所发生的活动。 </p><p>用户不会收到有关其自身活动的电子邮件警报。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL对我的评论的回复]</td> 
      <td>仅当某人明确回复了其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着，如果校样上的某人做出新评论，则不会通知审阅人。<p>建议您的客户在验证时使用此设置，以便他们不会收到关于验证的任何其他评论的通知，并且仅会收到对其自己评论的回复通知。</p><p>虽然具有此电子邮件警报设置的审阅人不会收到有关其他新注释的通知，但审阅人仍然可以在校样查看器中查看校样上的所有注释。</p><p>有关注释的信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校样评论</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL决策]</td> 
      <td>[!DNL Workfront] 仅当有人作出决定时，才向审阅人发送电子邮件。<p>这对于管理审批流程的人员（例如项目经理）和需要监控校样进度并查看哪些用户做出了决策的人员非常有用。</p><p>在提交您的决定时，您不会收到有关自己决定的通知，除非您选择了电子邮件确认选项。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL最终决定]</td> 
      <td>[!DNL Workfront] 当校样的最后审批者做出决定时，会发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审阅讨论。 当做出最终决策时，系统会通知设计人员，然后可以对任何必要的更改采取操作。</p><p>此警报对于只有在审核过程完成后才需要通知的部门负责人也非常有用。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL每小时摘要]</td> 
      <td>[!DNL Workfront] 每小时向审阅人发送一封电子邮件，其中包含该小时内发生的所有评论、回复和决策的摘要。<p>仅当您自己的活动之外的其他活动在过去一小时内发生时，才会发送电子邮件。 </p><p>此警报是查看项目概述的好方法。</p><p>本摘要的一个用例示例是高级审阅人，他需要项目概述，但不需要立即收到校样上所有活动的通知。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL每日摘要]</td> 
      <td>[!DNL Workfront] 发送一封电子邮件，其中仅列出在您自己的活动之外的几天内列出的所有评论、回复和决策。<p>此警报是您查看项目摘要的好方法，不会在一天中出现多次更新。</p><p>此摘要的一个示例用例是部门负责人，他希望监控项目的整体进度。</p><p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校样注释和决策通知</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL无电子邮件]</td> 
      <td>[!DNL Workfront] 不发送任何电子邮件警报。<br>对于仅出于参考目的而添加到校样且无需接收任何更改通知的人员，此功能非常有用。<p>系统默认值为[!UICONTROL每日摘要]（也称为[!UICONTROL未设置]）。 如果您或您的审阅人没有进行任何其他更改，则所有校样都具有此设置。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 更改以下任一项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！校样就绪时UICONTROL电子邮件确认]</td> 
      <td>指定您是否希望在创建校样时收到[!UICONTROL校样]电子邮件。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">[!UICONTROL校样]电子邮件</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL发送给我的电子邮件格式]</strong> </td> 
      <td> <p>在HTML样式电子邮件和纯文本电子邮件之间进行选择。 </p> <p>注意： 校样默认设置由校样级别的设置覆盖。 但是，如果在[!UICONTROL帐户]设置中为整个帐户禁用了校样电子邮件通知，则即使未在校样中选择[!UICONTROL禁用的电子邮件警报]，也不会向协作者发送电子邮件警报。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **[!UICONTROL 消息设置]**，请更改以下任意内容：

   | **[!UICONTROL 校样主题模板]** | 显示在“新校样”页、“新版本”页、“消息”页和“提醒”页。 可在发送前进行编辑。 |
   |---|---|
   | **[!UICONTROL 校样消息模板]** | 显示在“新校样”页、“新版本”页、“消息”页和“提醒”页。 可在发送前进行编辑。 |

   {style=&quot;table-layout:auto&quot;}

## 更改收件人的电子邮件警报

您可以在批量操作中更改特定收件人的电子邮件警报。

1. 单击 **[!UICONTROL 联系人]** 中。
1. 单击 **[!UICONTROL 更多]** （三个圆点）菜单，然后单击 **[!UICONTROL 查看成员详细信息]** 中。

1. 打开 **[!UICONTROL 共享项目]** 中。
1. 选中要更改其电子邮件警报的每个项目左侧的复选框。
1. 单击 **[!UICONTROL 更多]** 在共享项目列表上方，然后单击 **[!UICONTROL 更改电子邮件警报]** 中。

1. 更改电子邮件警报，然后单击 **[!UICONTROL 提交]**.

## 为用户配置校样默认值

如果您是 [!DNL Workfront Proof] 管理员，您可以为帐户中的用户设置校样默认值。

1. 单击 **[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**.

1. 打开 **[!UICONTROL 用户]** 选项卡。
1. 打开 **[!UICONTROL 更多]** 菜单。 ![More_button_small.png](assets/more-button-small.png)

1. 单击 **[!UICONTROL 查看用户详细信息]** 中。
1. 在 **[!UICONTROL 设置]**，单击 **[!UICONTROL 默认电子邮件警报设置]** 来扩展。

1. 在以下两个设置右侧的下拉列表中，选择下表中介绍的选项之一：

   * **[!UICONTROL 默认电子邮件警报]**:影响与您共享的每个校样。 可以在校样级别覆盖此设置。
   * **[!UICONTROL 新来宾审阅人的默认电子邮件警报]**:影响以前不作为帐户联系人存在的审阅人。

   >[!NOTE]
   >
   >如果您没有为用户选择以下选项之一， [!DNL Workfront Proof] 会向用户发送有关其校样活动的每日摘要。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL All activity]</td>
      <td>[!DNL Workfront] 每当校样存在任何活动（如新评论、回复或决定）时，都会向审阅人发送电子邮件。 <p>对于管理校对流程的人员而言，这是一个非常好的选项，因为它允许他们查看所发生的活动。 </p><p>用户不会收到有关其自身活动的电子邮件警报。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL对我的评论的回复]</td>
      <td>仅当某人明确回复了其评论时，才会向审阅人发送电子邮件（这不包括他们自己对评论的回复）。 这意味着，如果校样上的某人做出新评论，则不会通知审阅人。<p>建议您的客户在验证时使用此设置，以便他们不会收到关于验证的任何其他评论的通知，并且仅会收到对其自己评论的回复通知。</p><p>虽然具有此电子邮件警报设置的审阅人不会收到有关其他新注释的通知，但审阅人仍然可以在校样查看器中查看校样上的所有注释。</p><p>有关注释的信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">查看和回复校样评论</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL决策]</td>
      <td>[!DNL Workfront] 仅当有人作出决定时，才向审阅人发送电子邮件。<p>这对于管理审批流程的人员（例如项目经理）和需要监控校样进度并查看哪些用户做出了决策的人员非常有用。</p><p>在提交您的决定时，您不会收到有关自己决定的通知，除非您选择了电子邮件确认选项。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL最终决定]</td>
      <td>[!DNL Workfront] 当校样的最后审批者做出决定时，会发送电子邮件。<p>此警报通常由设计人员使用，他们通常不需要参加实际的审阅讨论。 当做出最终决策时，系统会通知设计人员，然后可以对任何必要的更改采取操作。</p><p>此警报对于只有在审核过程完成后才需要通知的部门负责人也非常有用。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL每小时摘要]</td>
      <td>[!DNL Workfront] 每小时向审阅人发送一封电子邮件，其中包含该小时内发生的所有评论、回复和决策的摘要。<p>仅当您自己的活动之外的其他活动在过去一小时内发生时，才会发送电子邮件。 </p><p>此警报是查看项目概述的好方法。</p><p>本摘要的一个用例示例是高级审阅人，他需要项目概述，但不需要立即收到校样上所有活动的通知。</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL每日摘要]</td>
      <td>[!DNL Workfront] 发送一封电子邮件，其中仅列出在您自己的活动之外的几天内列出的所有评论、回复和决策。<p>此警报是您查看项目摘要的好方法，不会在一天中出现多次更新。</p><p>此摘要的一个示例用例是部门负责人，他希望监控项目的整体进度。</p><p>有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">管理校样注释和决策通知</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL无电子邮件]</td>
      <td>[!DNL Workfront] 不发送任何电子邮件警报。<br>对于仅出于参考目的而添加到校样且无需接收任何更改通知的人员，此功能非常有用。<p>系统默认值为[!UICONTROL每日摘要]（也称为[!UICONTROL未设置]）。 如果您或您的审阅人没有进行任何其他更改，则所有校样都具有此设置。</p></td>
     </tr>
    </tbody>
   </table>

1. 在 **[!UICONTROL 默认电子邮件警报设置]**，请更改以下任意内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！校样就绪时UICONTROL电子邮件确认]</td> 
      <td>指定您是否希望在创建校样时收到[!UICONTROL校样]电子邮件。 有关更多信息，请参阅 <a href="https://support.workfront.com/hc/en-us/article">[!UICONTROL校样]电子邮件。</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL发送给我的电子邮件格式]</strong> </td> 
      <td> <p>在HTML样式电子邮件和纯文本电子邮件之间进行选择。 </p> <p>注意： 校样默认设置由校样级别的设置覆盖。 但是，如果在[!UICONTROL帐户]设置中为整个帐户禁用了校样电子邮件通知，则即使未在校样中选择[!UICONTROL禁用的电子邮件警报]，也不会向协作者发送电子邮件警报。<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
