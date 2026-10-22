---
title: 在GenStudio for Performance Marketing中启用Workfront规划Workspace
description: 如果您在Adobe Workfront Planning中已经有一个工作区，则可以为GenStudio for Performance Marketing启用它，而不是重新创建数据。
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 3f3f144e9cc7d3e64ed8e367a83c7c849b2f43b2
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# 在GenStudio for Performance Marketing中启用Workfront规划工作区

{{planning-important-intro}}

<!-- add to TOC and mini TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
除了Workfront Planning之外，如果贵公司还购买了Adobe GenStudio for Performance Marketing，那么当您的GenStudio实例与贵公司的Adobe Workfront实例集成时，GenStudio Planning中会提供Workfront工作区。

如果您在Workfront Planning中已经有一个工作区，则可以为GenStudio启用它，而不是重新创建数据。

启用工作区可将其链接到Adobe存储项目，并将其记录类型和字段映射到GenStudio工作区架构。 完成配置后，您可以在GenStudio中打开工作区的记录。

请考虑以下事项：

* 您必须同时具有Workfront Planning和GenStudio for Performance Marketing的访问权限。
* 您必须具有Adobe云存储项目才能链接到工作区。 组织管理员可以在Adobe Admin Console中创建一个。

  有关信息，请参阅[管理Adobe存储](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)。<!--ensure this site still works-->


## 在GenStudio中启用Workfront规划工作区

1. 在Workfront Planning中，打开要启用的工作区。
1. 单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**启用GenStudio**。

   **使工作区GenStudio**&#x200B;已启用框打开，包括以下步骤：

   1. **ACPC项目**：选择要与此工作区同步的&#x200B;**ACPC项目** （Adobe云存储项目），然后单击&#x200B;**下一步**。 用户通过此项目访问GenStudio中的工作区。

      ![启用工作区GenStudio - ACPC项目步骤](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **记录类型**：将工作区的记录类型映射到GenStudio所需的六种记录类型：

      * 营销活动
      * 产品
      * 用户画像
      * 渠道
      * 区域
      * 激活

      对于每个记录，请打开列表并选择匹配的Planning记录类型，或选择&#x200B;**添加新**&#x200B;以创建该记录，然后单击&#x200B;**下一步**。

      ![启用工作区GenStudio — 记录类型步骤](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **字段**：映射每个记录类型的字段。 使用对话框顶部的选项卡在记录类型之间移动。 对于每个字段，请选择匹配的Planning字段，或选择&#x200B;**添加新的**&#x200B;以创建它。

      对所有记录类型重复字段设置。

      ![启用工作区GenStudio — 字段步骤](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 查看并解决任何警告。

      例如，新字段可以成为记录类型的主字段，或者已使用的字段别名被重命名（如果您已经有一个名为“Regions”的字段，则导入的字段可能会变为“Regions 2”）。

      映射&#x200B;**状态**&#x200B;字段会添加所需选项。

   1. 单击&#x200B;**发布**。

      启用工作区后，将显示一条确认消息。 在工作区中标记映射的记录类型。

      映射到可从GenStudio访问的记录类型卡片上有一个新的&#x200B;**Adobe**&#x200B;图标。

      ![带有Adobe图标的促销活动记录类型](assets/campaigns-record-type-card-with-adobe-icon.png)

1. 打开GenStudio，选择&#x200B;**促销活动**，然后单击屏幕左下角最初为此设置配置的&#x200B;**ACPC项目**。 查看导入的记录类型和字段。

   >[!TIP]
   >
   >您只能看到ACPC项目成员资格允许的记录。
