---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: 系统跟踪更新
description: Adobe Workfront通过将状态信息记录在对象的 [!UICONTROL 更新] 区域。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: d76ab0e165d280f84718b52cc72a9b4c152a0897
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# 系统跟踪更新

{{highlighted-preview}}

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] 通过在对象的 [!UICONTROL 更新] 区域。

此 [!UICONTROL 更新] 区域包含以下类型的更新：

* **用户更新：** 由用户手动输入。 也称为评论、回复和注释。

  有关配置用户更新的更多信息，请参阅 [配置用户更新的首选项](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **系统更新：** 由系统自动生成。 系统更新包括一个简要注释，描述该项发生了什么类型的更改。

  有关系统更新源以及如何启用它们的详细信息，请参阅 [配置系统更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## 有关系统跟踪更新的注意事项

系统跟踪更新不适用于具有“更新”区域的所有对象。

* 此 [!UICONTROL 更新] 区域可用于以下对象：

   * [!UICONTROL 项目]
   * [!UICONTROL 任务]
   * [!UICONTROL 问题]
   * [!UICONTROL Portfolio]
   * [!UICONTROL 项目]
   * [!UICONTROL 用户]
   * [!UICONTROL 模板]
   * [!UICONTROL 模板任务]
   * [!UICONTROL 团队]
   * [!UICONTROL 文档]
   * [!UICONTROL 工时表]
   * [!UICONTROL Story]

     在 [!DNL Workfront]，故事是任务。
   * [!UICONTROL 迭代]
   * [!UICONTROL 目标]

     您必须拥有额外的许可证才能访问 [!UICONTROL 目标] 区域。 有关信息，请参阅 [使用Workfront Goals的要求](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL 卡片] 在展示板上

     有关信息卡更新的更多信息，请参阅 [在展示板上使用连接的信息卡](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] 不跟踪以下对象的系统更新：

   * [!UICONTROL 团队]
   * [!UICONTROL 模板]
   * [!UICONTROL 模板任务]
   * 临时 [!UICONTROL 卡片]
   * [!UICONTROL 迭代]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* 以下是新评论体验和旧评论体验之间的差异：

   * 使用新的备注体验时，用户更新显示在“备注”选项卡中，系统更新显示在“系统活动”选项卡中。

     有关新评论体验的更多信息，请参阅 [新的评论体验](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">使用新的评论体验时，用户无法将评论添加到系统更新。 但是，对旧版注释体验中的系统活动记录所做的任何回复，都会在新版注释体验中的“系统活动”选项卡中以只读形式填充。</span>
   * 使用旧版评论体验时，系统和用户更新显示在一个连续馈送中。

   * 使用旧版评论体验时，用户可以默认查看系统更新，也可以选择不显示这些更新。 使用新的注释体验时，无法禁用系统更新。

     有关禁用系统更新显示的信息，请参阅部分 [启用或禁用系统更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) 在文章中 [更新工作](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront记录以下对象的系统跟踪更新，但没有选项可禁用显示这些对象：

   * [!UICONTROL Portfolio]
   * [!UICONTROL 项目]
   * [!UICONTROL 迭代]

* [!DNL Workfront] 管理员可以定义系统应跟踪的更改类型 [!UICONTROL 更新] 区域。 并非所有具有 [!UICONTROL 更新] 区域也可供配置 [!UICONTROL 更新] 信息源。 以下对象具有 [!UICONTROL 更新] 捕获系统跟踪的更新馈送，但没有可配置的更新馈送的区域：

   * [!UICONTROL 文档]
   * [!UICONTROL 工时表]
   * [!UICONTROL 迭代]
   * [!UICONTROL 目标]


