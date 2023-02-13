---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 在中管理校样版本 [!DNL Workfront Proof]
description: 管理作品的多个版本或修订版本之间的反馈可能是一项巨大的挑战。 [!DNL Workfront Proof] 通过允许您创建和比较多个版本的校样，简化了此过程。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# 在中管理校样版本 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

管理作品的多个版本或修订版本之间的反馈可能是一项巨大的挑战。 [!DNL Workfront Proof] 通过允许您创建和比较多个版本的校样，简化了此过程。

您可以创建校样的版本数没有限制。 因此，如果您需要与客户端进行许多修订以获得最终批准，则可以在中查看并轻松管理创建的所有版本 [!DNL Workfront Proof].

权限是特定于某个版本的，因此您可以为人员授予查看一个版本的权限，但不能查看另一个版本。 相反，如果您与人员共享较新版本，则他们将无法查看较早版本，除非您返回并明确将其添加到之前的版本。

要创建校样的新版本，您必须对校样具有编辑权限。

请参阅 [在中管理校样角色 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) 以获取有关谁对校样具有编辑权限的更多信息。 请参阅以了解有关创建版本的更多信息。

## 在校样查看器中查看校样版本

校样查看器的左上角将显示您正在查看的版本的完整名称。 校样的任何其他版本将仅显示为版本号。

1. 在校对查看器中打开校样，如 [在中打开校样 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. 在校样查看器中，单击校样名称右侧的版本号。
1. 要查看其他版本，请在单击版本号时显示的菜单中单击其名称。
1. 要比较两个版本，请单击 **[!UICONTROL 比较校样]** 图标。\
   ![Compare_Proods_button.png](assets/compare-proofs-button.png)\
   如果校样有多个版本，则可以通过单击比较模式拆分屏幕两侧的相关版本号来选择要比较的两个版本。

有关在校样查看器中查看校样的信息，请参阅 [查看验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## 通过校样详细信息页面访问校样版本

您可以通过校样详细信息页面访问校样的所有版本。

1. 打开校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. 单击页面顶部版本选项卡的选项卡，然后单击 **[!UICONTROL 转到校样]** 以在校样查看器中打开所需的版本。\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## 链接校样版本

如果您的校样具有多个版本，则校样的先前版本通常称为父校样。

如果您希望将父校样（以前的版本）更改为帐户中的其他校样，或将单个校样连接到帐户中的其他校样（作为其他校样的新版本），则可以按照以下步骤轻松完成：

1. 打开校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. 单击 **[!UICONTROL 更多]** > **[!UICONTROL 更改以前的版本]**.

1. 在 **[!UICONTROL 更改以前的版本]** 框中，选择要设置为父校样的校样（以前的版本）。\
   如果需要在列表上查找校样的帮助，可以通过单击列标题对列进行排序。

1. 单击 **[!UICONTROL 更改以前的版本]** 来连接版本。

>[!NOTE]
>
>将校样连接到帐户中的其他校样（作为新版本）时， [!DNL Workfront Proof] 锁定当前版本为以前的校样。

## 取消链接校样版本

您可以从其父校样（以前的版本）中取消链接当前正在查看的校样，而无需将其关联到帐户中的其他校样：

1. 打开校样的校样详细信息页面，如 [在中管理校样详细信息 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. 单击 **[!UICONTROL 更多]** > **[!UICONTROL 删除指向以前版本的链接]**.

   * 只能从整个版本集中取消链接（断开连接）最后一个版本。 然后，它将变成单一的证据。
   * 如果需要在两个现有版本之间插入版本，可以取消同一校样的所有版本的链接，并按正确的顺序重新链接它们。

## 关于版本集和校样限制

五个版本的每组都将计为一个验证，以符合总校样限制。

例如，如果您上传某个设计的五个版本（包括原始版本），则该设计将计为一次校样。 如果您上传某个设计的六个版本，则这计为两个校样。 11个版本将计为3个证据，依此类推。

对于音频可视文件，每个新版本都计为新校样。
