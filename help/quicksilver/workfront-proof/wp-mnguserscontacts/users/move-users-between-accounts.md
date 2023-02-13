---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: 使用在帐户之间移动用户 [!DNL Workfront Proof]
description: 如果您是 [!DNL Workfront Proof] 管理员，并且您有一个或多个与主帐户连接的卫星帐户，则可以在所有这些帐户之间移动用户。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 使用在帐户之间移动用户 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您是 [!DNL Workfront] 校样管理员和您的一个或多个卫星帐户连接到您的主帐户，您可以在所有这些帐户之间移动用户。

## 在连接的帐户之间移动用户

1. 单击 **[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**.

1. 打开 **[!UICONTROL 用户]** 选项卡。
1. 单击 **[!UICONTROL 移动用户]** 图标(1)。 ![Move_user2.png](assets/move-user2-350x95.png)

1. 在显示的移动用户框中，确认要移动的用户(1)。
1. 从连接的帐户列表(2)中选择目标帐户。
1. 分配此用户在新帐户上应具有的配置文件权限(3)。
1. 选择应拥有不会移动的项目所有权的用户(4)。
这包括您决定保留在旧帐户上的项目以及无法移动的项目(请参阅 [无法移动的项目](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) )。

1. 如果要随用户一起移动校样(5)和文件(6)，请勾选复选框。
1. 为文件夹(7)创建一个名称，在该文件夹中所有被移动的项目都将放在新帐户上。
1. 单击 **[!UICONTROL 移动用户]** （八）启动程序。
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

如果您选择移动用户而不带有其校样和文件，则会立即执行此操作。 如果您选择移动用户及其校样和文件，则用户的用户档案将立即重新分配，但校样和文件将逐渐显示在目标帐户上，因为此操作需要时间传输数据。

根据文件和校样移动过程的数量，可能需要几分钟到几小时的时间才能完成任何操作。

>[!NOTE]
>
>如果您怀疑该过程比预期的时间长，或者已移动的校样和/或文件未显示在新帐户中，请联系我们的支持团队。

## 无法移动的项目

### 已移动用户创建或拥有的文件夹

由于对文件夹及其内容应用的各种权限的性质（例如，这些权限可能与其他用户和帐户共享），我们无法与用户一起移动文件夹结构。

如果被移动的用户拥有文件夹，则在“移动用户”弹出窗口中，所有权将转移给选定的用户(4)。

>[!NOTE]
>
>如果已移动的用户创建了文件夹，文件夹的创建者仍将是文件夹的创建者，只有所有权才会被转移。 被移动的用户在其新帐户的侧栏中仍可以看到文件夹。 被移动的用户仍将对放置在这些文件夹中的项目具有“只读”访问权限。

如果您不希望被移动的用户保留此类权限，或者被移动的用户不希望在旧帐户上看到其旧文件夹，则此处的解决方案将删除这些文件夹，如下所示：

1. 在旧帐户上创建新文件夹。
1. 将所有项目从已移动用户的文件夹移到新创建的文件夹中。
1. 删除已移动用户所剩的所有文件夹。

### 具有不同所有者的版本集

如果校样具有几个版本，并且每个版本都由不同的用户拥有，则移动的用户拥有的版本将不会随之移动。 根据您在“移动”用户框中的选择(4)，此类版本的所有权将转移给其他用户。 （有关更多信息，请参阅。）

>[!NOTE]
>
>已移动的用户需要拥有集中的所有校样版本，才能随之移动校样。

### 组

移动的用户需要在其新帐户上重新创建群组。 有关更多信息，请参阅 [使用创建校对组 [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### 自定义视图

移动的用户需要在其新帐户上重新创建个人自定义视图。 有关更多信息，请参阅 [在中创建和管理自定义视图 [!DNL Workfront Proof] 校样](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### 自定义字段

无法移动自定义字段，并且自定义字段中的数据将丢失，因此请确保在移动之前生成有关所需项目的报表。

### 自动化工作流模板

需要在新帐户上重新创建自动工作流模板，但使用模板创建的移动校样中将保留阶段。

### 对注释的操作

对评论的操作将保留在校样中，但无法再按这些操作进行过滤。 解决方案是在新帐户上创建匹配的操作，并在需要时使用新操作重新标记注释。
