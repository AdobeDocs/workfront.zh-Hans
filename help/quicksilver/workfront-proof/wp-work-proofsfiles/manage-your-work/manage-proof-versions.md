---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 管理 [!DNL Workfront Proof]中的校对版本
description: 跨工作项的多个版本或修订版本管理反馈可能是一项巨大的挑战。 [!DNL Workfront Proof] 通过允许您创建和比较校对的多个版本来简化此过程。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中管理校对版本

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

跨工作项的多个版本或修订版本管理反馈可能是一项巨大的挑战。 [!DNL Workfront Proof]通过允许您创建和比较验证的多个版本简化了此过程。

您可以创建的验证版本数量没有限制。 因此，如果您需要通过客户端进行多个修订以获得最终批准，则可以在[!DNL Workfront Proof]内查看并轻松管理创建的所有版本。

权限特定于某个版本，因此您可以向人员授予查看某个版本的权限，但不能授予查看另一个版本的权限。 相反，如果您与某个人共享更高版本，则他们将看不到早期版本，除非您返回并将它们明确添加到这些早期版本。

要创建新版本的验证，您必须具有对验证的编辑权限。

请参阅[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)中管理验证角色，以获取有关谁具有验证编辑权限的更多信息。 请参阅以了解有关创建版本的更多信息。

## 在验证查看器中查看验证版本

您正在查看的版本的全名将显示在验证查看器的左上方。 该验证的任何其他版本都将仅显示为版本号。

1. 在验证查看器中打开验证，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md)中打开验证中所述。
1. 在验证查看器中，单击验证名称右侧的版本号。
1. 要查看其他版本，请在单击版本号时显示的菜单中单击其名称。
1. 要比较两个版本，请单击&#x200B;**[!UICONTROL 比较验证]**&#x200B;图标。\
   ![Compare_Proofs_button.png](assets/compare-proofs-button.png)\
   如果校对有多个版本，您可以通过单击比较模式分屏两侧的相关版本号，选择要比较的两个版本。

有关在验证查看器中查看验证的信息，请参阅[查看验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md)。

## 通过验证详情页面访问验证版本

您可以通过验证详细信息页面访问验证的所有版本。

1. 打开校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。
1. 单击页面顶部版本选项卡的选项卡，然后单击&#x200B;**[!UICONTROL 转到校对]**&#x200B;以在校对查看器中打开所需的版本。\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## 链接校对版本

如果您的校对具有多个版本，则以前版本的校对通常称为父校对。

如果您想要将父验证（以前的版本）更改为帐户中的另一个验证，或将单个验证连接到帐户中的另一个验证（作为另一个验证的新版本），您可以执行以下步骤来轻松完成此操作：

1. 打开校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 更改以前的版本]**。

1. 在出现的&#x200B;**[!UICONTROL 更改以前的版本]**&#x200B;框中，选择要设置为父校对（以前的版本）的校对。\
   如果您需要帮助才能在列表中查找校对，则可以通过单击列标题对列进行排序。

1. 单击框底部的&#x200B;**[!UICONTROL 更改以前的版本]**&#x200B;以连接版本。

>[!NOTE]
>
>当您将一个验证连接到帐户中的另一个验证（作为新版本）时，[!DNL Workfront Proof]将锁定当前为先前版本的验证。

## 取消链接校对版本

您可以取消当前查看的校对与其父校对（以前版本）的链接，而无需将其关联到帐户中的其他校对：

1. 打开校对的校对详细信息页面，如[在 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)中管理校对详细信息。
1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 删除指向以前版本]**&#x200B;的链接。

   * 只能从整个版本集中取消链接（断开连接）最后一个版本。 然后，它将成为一个单一的证明。
   * 如果您需要在两个现有版本之间插入一个版本，可以取消链接同一验证的所有版本，并按正确顺序重新链接它们。

## 关于版本集和验证限制

每组五个版本都将计为一份校对总校对限制的校对。

例如，如果您上传设计的五个版本（包括原始版本），则会计为一次验证。 如果上传设计的六个版本，则将被计为两个验证。 11个版本会计为三个校样，依此类推。

对于视听文件，每个新版本都计为新校对。
