---
title: 跨工作区记录类型概述
description: 您可以将记录类型设置为全局或可连接。 全局记录类型可以从Adobe Workfront Planning中的中央或主工作区添加到多个工作区，而可连接的记录类型可以从其自身以外的其他工作区连接到。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: f88b6ec019963ff6256e35b9c94eb4d1b7e99730
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---


# 跨工作区记录类型概述

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以在Adobe Workfront Planning中为记录类型启用跨工作区功能。 可以从多个工作区引用或访问跨工作区记录类型。

>[!IMPORTANT]
>
>增强了Workfront包要求，以便能够为系统中的记录类型启用跨工作区功能。 有关信息，请参阅[Adobe Workfront计划访问概述](/help/quicksilver/planning/access/access-overview.md)。


以下是记录类型的跨工作区功能：

* <span class="preview">**全局记录类型**：用户可以将全局记录类型添加到其管理的其他工作区。</span>

* **可连接的记录类型**：用户可以从其他工作区连接到此记录类型。

本文概述跨工作区记录类型。 有关定义记录类型的跨工作区功能的信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。

<div class="preview">

## 全局记录类型概览

全局记录类型可以从Workfront Planning中的中央或主工作区添加到多个工作区。

在使用通用工作流为多团队组织实施Workfront Planning时，您可能需要为关键记录类型（如营销活动或交付项）定义一个凝聚结构和元数据，这些记录类型可以添加到每个团队的工作区中以捕获和管理其工作。

此外，您可能需要每个团队的工作汇总到一个中心级别。

在此类工作流中，您可以确保团队以一致的方式捕获他们的工作，同时解锁跨团队的可见性，而无需将所有内容添加到一个工作区，或组织中的每个人都添加到每个工作区。 您可以使用全局记录类型来实现这一点。

要使用全局记录类型，请执行以下操作：

1. 在您管理的工作区中，将记录类型配置为全局。

   工作区管理员可以为具有Standard许可证的用户或团队、组、角色和公司授予权限，以将所选记录类型添加到他们管理的工作区。

   原始记录类型将存在于其原始工作区中，但将在其他工作区中可见。

   有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。
1. 从已配置为全局记录类型的现有工作区向辅助工作区添加记录类型。

   记录类型将存在于以下工作区中：

   * 它的原始工作区，在工作区中，它被指定为全局记录类型。
   * 辅助工作区。

   有关信息，请参阅[从另一个工作区添加现有记录类型](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)。

   以下各节介绍了有关全局记录类型以及它们在其原始工作区或辅助工作区中如何工作的注意事项。

### 有关其原始工作区中全局记录类型的注意事项

配置为全局的记录类型具有以下属性：

* 其所有信息（外观、原始字段）只能在原始工作区中进行编辑。

* 您可以从全局记录类型的原始工作区对其执行以下操作：

   * 编辑它

     编辑全局记录类型包括编辑其外观、跨工作区功能以及在原始工作区中创建的所有字段。
   * 创建和管理请求表单
   * 创建和管理自动化

* 仅当全局记录类型尚未添加到辅助工作区时，才能将其删除。 必须先从辅助工作区中删除它（通过删除它），然后才能从原始工作区中删除它。

  有关详细信息，请参阅[删除记录类型](/help/quicksilver/planning/architecture/delete-record-types.md)。
* 您添加到全局记录类型的记录仅对具有对其所添加的工作区的查看权限的用户可见。
* 从辅助工作区添加的记录将汇总并显示在原始工作区中。 原始工作区的所有成员都将获得对其的“查看”权限。
* 将原始全局记录类型添加到多个辅助工作区时，存在以下情况：

   * 原始工作区的成员将自动获得从任何工作区添加的所有记录的查看权限，即使他们不是这些工作区的成员。
   * 辅助工作区成员只能查看其所属工作区的记录。
* 全局记录类型的已连接记录类型将可用于从添加此记录类型的工作区进行连接。

  例如，如果您的Campaign全局记录类型与区域记录类型相关联，并且您将Campaign记录类型添加到辅助工作区，则区域将从辅助工作区变为可跨工作区连接。 辅助工作区成员现在可以创建营销活动并将它们链接到区域。

* 从原始工作区中为全局记录类型创建的字段在添加该记录类型的所有工作区中均可见。 您只能从原始工作区中编辑字段设置。 在原始工作区中创建的字段设置对于所有成员在辅助工作区中都是只读的，无论这些成员在辅助工作区中拥有什么权限。 辅助工作区管理员无法修改在原始工作区中配置的字段的字段设置。 只有原始工作区的工作区管理员才能修改原始工作区中的字段设置。

### 有关辅助工作区中全局记录类型的注意事项

* 辅助工作区参与者将获得对其团队工作区中的全局记录类型的参与权限。 他们可以从辅助工作区添加和管理其中的记录。

* 辅助工作区查看器获得对其团队工作区中全局记录类型的查看权限。 他们不能在其中添加和管理记录。

* 辅助工作区管理员可以对从辅助工作区中的全局记录类型添加的记录类型执行以下操作：

   * 删除它。

     从辅助工作区中删除记录类型只会将其从辅助工作区中删除。 从辅助工作区添加到该工作区的记录和字段也会被删除。 这不会从其原始工作区或已添加记录类型的任何其他辅助工作区中删除该记录类型。

     有关详细信息，请参阅[删除记录类型](/help/quicksilver/planning/architecture/delete-record-types.md)。
   * 共享记录类型的视图。

     <!-- when they will be able to add fields to the secondary space, this bullet will need this extra information: 
         After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added. -->

  <!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
    * Add new fields
        Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
    * Share it
    * Add request forms to it
    * Add automations to it-->

* 任何用户都不能对辅助工作区中的全局记录类型执行以下操作：

   * 编辑它

     不能编辑其外观、跨工作区功能或从原始工作区添加的字段。
   * 共享
   * 创建和管理请求表单
   * 创建和管理自动化

* 只有在您具有辅助工作区的“查看”或更高权限时，才可以看到从以下工作区添加到辅助工作区的记录：

   * 在其中添加它们的辅助工作区。
   * 全局记录类型的原始工作区。
   * 添加全局工作区的所有其他工作区。

* 在辅助工作区中创建的记录存在以下情况：

   * 如果您对原始工作区具有“管理”权限，而对辅助工作区没有权限，则可以查看从原始工作区中的辅助工作区添加的记录，但无法从原始工作区管理这些记录。
   * 如果您对辅助工作区具有管理权限，则可以从全局记录类型的原始工作区以及添加这些记录的辅助工作区中管理记录。
   * 您只能在添加全局记录类型的附加辅助工作区中查看记录，但前提是您对这些工作区具有查看权限。

### 访问全局记录类型的连接

连接到原始工作区中全局记录类型的记录类型在添加全局记录类型的其他工作区中变得可见，并且可用于添加全局记录类型的辅助工作区的连接。

### 全局记录类型的API访问

使用Workfront Planning API从辅助工作区将记录添加到全局记录类型时，系统会检查用户是否有权在全局记录类型的原始工作区中创建记录。

存在以下情况：

* 如果用户具有访问权限，则会在全局记录类型的原始工作区中创建记录。

* 如果用户没有访问权限，则用户会收到一个错误，表明他们无权访问全局记录类型的原始工作区，并且他们需要提供他们有权创建记录的工作区ID。

</div>

## 可连接记录类型概述

您可以从您管理的任何工作区连接到已定义为可连接的记录类型。

您的团队可能需要将其记录链接到来自其他工作区的记录类型，或查看从属于其他工作区中记录的记录中捕获的信息。 通过将记录类型指定为可连接，可以实现此配置。

要使用可连接的记录类型，请执行以下操作：

1. 将记录类型配置为可在特定工作区中连接。

   工作区管理员可以选择指定的记录类型可以连接到哪些工作区。

   原始记录类型将存在于其原始工作区中，并且可从其他工作区访问它以连接到。

   有关信息，请参阅[为记录类型配置跨工作区功能](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)。
1. 从您管理的另一个工作区连接到指定为可连接的记录类型。

   有关信息，请参阅[连接记录类型](/help/quicksilver/planning/architecture/connect-record-types.md)。
