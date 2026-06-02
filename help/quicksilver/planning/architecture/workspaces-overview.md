---
title: 工作区概述
description: 工作区是团队使用的记录类型的集合，表示团队的工作生命周期。 您可以在Adobe Workfront Planning中完全自定义工作区，以匹配组织单位的工作流。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 0%

---

# 工作区概述

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

工作区是组织单位使用的记录类型的集合，它表示该单位的工作生命周期和流程。 您可以在Adobe Workfront Planning中完全自定义工作区。

<!--update screenshot with production, it was broken at Preview-->

![工作区登陆页面管理员帐户](assets/workspaces-landing-page-admin-account.png)

## 有关工作区的注意事项

* 您可以为组织内的特定组织单位创建工作区，以匹配每个单位独特的工作方式。
* Workfront Planning不附带任何预配置的工作区。 您必须根据组织的需求创建它们。
* 您可以通过以下方式创建工作区：

   * 从头开始
   * 使用模板。 模板包含预配置的记录类型及其字段。
   * 使用AI支持的规划Designer。 此功能当前位于Beta中。
   * 使用多工作区模板捆绑包。

  有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

* 工作区是组织单位（团队、组、部门或分部）工作所在的框架。 它们不能与字段相关联。 只有工作区中的记录类型可以与字段相关联。

  有关信息，请参阅[记录类型概述](/help/quicksilver/planning/architecture/overview-of-record-types.md)。
* 工作区显示在Planning区域的以下选项卡中：

   * **我所在的工作区**：显示您创建的工作区或与您共享的工作区。
   * **其他工作区**：显示系统中的所有其他工作区。 这仅适用于系统管理员。
   * <span class="preview">**示例工作区**：显示最佳实践工作区的内置示例。 您无法编辑工作区、记录类型或添加记录或字段，但可以添加、编辑视图并与他人共享视图。</span>

  >[!NOTE]
  >
  ><span class="preview">我们建议不要编辑示例工作区，而是将其用作创建您自己的工作区的引用。 使用多工作区模板包创建与“示例工作区”选项卡中列出的工作区相同的工作区。 有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)一文中的“使用最佳实践多工作区模板包创建多个工作区”部分。</span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* 工作区包含的记录类型应反映工作生命周期和组织单位的概念。

  例如，如果单位的工作对象是促销活动、产品和区域，则该单位的工作区应包含促销活动、产品和区域的记录类型。
* 在创建工作区时，只有您才有权访问和管理工作区。 您必须与其他用户共享，他们才能在同一空间与您协作。

  有关信息，请参阅[共享工作区](/help/quicksilver/planning/access/share-workspaces.md)。

  系统管理员可以管理所有工作区，甚至可以管理他们未创建的工作区。

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* 在Workfront Planning的实例中，您可以创建的工作区对象数量存在限制。 有关信息，请参阅[Adobe Workfront Planning对象限制概述](/help/quicksilver/planning/general/limitations-overview.md)。
