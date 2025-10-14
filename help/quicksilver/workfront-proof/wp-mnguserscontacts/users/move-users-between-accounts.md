---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: 使用 [!DNL Workfront Proof]在帐户之间移动用户
description: 如果您是 [!DNL Workfront Proof] 管理员，并且有一个或多个附属帐户连接到您的主帐户，则可以在所有这些帐户之间移动用户。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 使用[!DNL Workfront Proof]在帐户之间移动用户

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

如果您是[!DNL Workfront]验证管理员，并且有一个或多个附属帐户连接到您的主帐户，则您可以在所有这些帐户之间移动用户。

## 在连接的帐户之间移动用户

1. 单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**。

1. 打开&#x200B;**[!UICONTROL 用户]**&#x200B;选项卡。
1. 单击&#x200B;**[!UICONTROL 移动用户]**&#x200B;图标(1)。 ![Move_user2.png](assets/move-user2-350x95.png)

1. 在出现的“移动用户”框中，确认要移动的用户(1)。
1. 从连接的帐户列表(2)中选择一个目标帐户。
1. 分配此用户对新帐户应具有的配置文件权限(3)。
1. 选择应拥有不会移动的项目的所有权的用户(4)。
这包括您将决定保留在旧帐户上的项目以及无法移动的项目（请参阅下面的[无法移动的项目](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved)）。

1. 如果要与用户一起移动校样(5)和文件(6)，请选中复选框。
1. 为文件夹(7)创建一个名称，所有移动的项目都将存放在该文件夹中。
1. 单击&#x200B;**[!UICONTROL 移动用户]** (8)以启动进程。
   ![Moving_users_popup.png](assets/moving-users-pop-up-350x380.png)

如果您选择移动没有验证和文件的用户，将立即执行此操作。 如果选择将用户及其验证和文件一起移动，则将立即重新分配用户的配置文件，但验证和文件将逐渐显示在目标帐户上，因为此操作需要时间来传输数据。

根据文件和校样的数量，移动过程可能需要几分钟到几小时不等。

>[!NOTE]
>
>如果您怀疑该过程花费的时间长于预期，或移动的验证和/或文件未出现在新帐户中，请联系我们的支持团队。

## 无法移动的项目

### 被移动的用户创建或拥有的文件夹

由于应用于文件夹及其内容的各种权限的性质（例如，它们可以与其他用户和帐户共享），我们无法与用户移动文件夹结构。

如果文件夹由移动的用户拥有，则所有权将在“移动用户”弹出窗口中转移给选定的用户(4)。

>[!NOTE]
>
>如果文件夹是由移动的用户创建的，则其仍将是创建者 — 只会转移所有权。 被移动的用户在其新帐户的侧边栏中仍可看到该文件夹。 被移动的用户对于放置在这些文件夹中的项目仍具有“只读”访问权限。

如果您不希望被移动的用户保留此类权限，或者被移动的用户不希望在old&amp;帐户上看到他们的旧文件夹，则此处的解决方案是按如下方式删除文件夹：

1. 在旧帐户上创建新文件夹。
1. 将移动用户文件夹中的所有项目移动到新创建的文件夹。
1. 删除被移动的用户留下的所有文件夹。

### 具有不同所有者的版本集

如果验证只有几个版本，并且每个版本都由不同的用户拥有，则移动用户拥有的版本将不会移动。 根据您在移动用户框中选择(4)，这些版本的所有权将转移给另一个用户。 （有关更多信息，请参阅。）

>[!NOTE]
>
>已移动的用户需要拥有集中的所有验证版本，才能同时移动验证。

### 组

组需要由移动的用户在其新帐户中重新创建。 有关详细信息，请参阅[使用 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md)创建验证组。

### 自定义视图

移动的用户需要在其新帐户上重新创建个人自定义视图。 有关详细信息，请参阅[在 [!DNL Workfront Proof] 验证](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)中创建和管理自定义视图。

### 自定义字段

无法移动自定义字段，且来自自定义字段的数据将丢失，因此请确保在移动之前生成所需项的报告。

### 自动化工作流模板

需要在新帐户上重新创建自动化工作流模板，但阶段将保留在使用模板创建的移动验证上。

### 评论操作

评论上的操作将保留在验证上，但无法再按它们进行过滤。 解决方案是在新帐户上创建匹配的操作，并在需要时使用新操作重新标记注释。
