---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: 在 [!DNL Workfront Proof]中管理使用自动化工作流配置的校对
description: 您可以方便地在验证详细信息页面的工作流部分跟踪自动工作流验证的进度。 您可以查看在每个阶段上完成的工作，并修改、添加、启动和锁定验证上的阶段。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1d0ad905-f3fb-471a-8766-096b978cdf4e
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 在[!DNL Workfront Proof]中管理使用自动化工作流配置的校对

>[!IMPORTANT]
>
>本文提及独立产品[!DNL Workfront Proof]中的功能。 有关[!DNL Adobe Workfront]内部校对的信息，请参阅[校对](../../../review-and-approve-work/proofing/proofing.md)。

您可以在[!UICONTROL 验证详细信息]页面的“工作流”部分方便地跟踪自动工作流验证的进度。 您可以查看在每个阶段上完成的工作，并修改、添加、启动和锁定验证上的阶段。

## 查看自动工作流

您可以通过三种主要方式查看您的自动工作流：

* [详细查看阶段](#view-a-stage-in-detail)
* [查看所有阶段](#view-all-stages)
* [详细查看所有阶段](#view-all-stages-in-detail)

### 详细查看阶段 {#view-a-stage-in-detail}

1. 单击部分(1)顶部的按钮。

   您可以使用图表在阶段之间切换。 您正在查看的舞台以灰色(2)突出显示。

1. 要查看其他阶段，请在图中选择该阶段。

![View_a_stage_in_detail.png](assets/view-a-stage-in-detail-350x249.png)

### 查看所有阶段 {#view-all-stages}

要查看自动工作流中的所有阶段，请执行以下操作：

1. 单击页面(3)顶部的按钮。

   自动工作流的所有阶段都列在部分中，但详细信息隐藏。

1. 要查看阶段的详细信息，请单击每个阶段(4)的名称旁边的加号图标。

![View_all_stages.png](assets/view-all-stages-350x212.png)

### 详细查看所有阶段 {#view-all-stages-in-detail}

要详细查看自动工作流的所有阶段，请执行以下操作：

1. 单击页面顶部的按钮(5)。

   这将向您显示自动工作流的所有阶段，并展开每个阶段的详细信息。

   您可以通过单击减号图标(6)来隐藏每个阶段的详细信息。

![View_all_stages_in_detail.png](assets/view-all-stages-in-detail-350x370.png)

## 使用自动工作流程图

自动化[!UICONTROL 工作流]的图表显示在工作流部分的顶部。

隐藏图表

1. 单击&#x200B;**[!UICONTROL 隐藏]**&#x200B;按钮(1)。

![图__1_.png](assets/diagram--1--350x217.png)

图中的各个阶段标记如下：

![dot.png](assets/dot.png) — 活动阶段

![gray_dot.png](assets/grey-dot.png) — 非活动阶段\
![sbw-key-icon.png](assets/sbw-key-icon.png)   — 私人舞台

![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)   — 锁定的阶段

阶段之间的行描述阶段之间的依赖关系。 指向非活动阶段的行将虚线，直到激活阶段。

将鼠标悬停在图中的某个阶段上会显示该阶段的进度。 如果舞台处于非活动状态，并且您具有在舞台上的编辑权限，则可使用[!UICONTROL 开始舞台]按钮从弹出窗口中开始舞台。 同样，将显示“锁定活动阶段”选项。

要了解有关“进度”栏的更多信息，请参阅  [在 [!DNL Workfront] Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md)中查看校对的进度和状态。

![Diagram_-_stage_summary.png](assets/diagram---stage-summary-350x214.png)

## 添加新阶段

您可以从[!UICONTROL 验证详细信息]页面向自动工作流添加新阶段。

1. 单击&#x200B;**[!UICONTROL 新建阶段]**&#x200B;按钮(1)。

![Adding_a_new_stage_1.png](assets/adding-a-new-stage-1-350x218.png)

在出现的&#x200B;**新阶段**&#x200B;框中，您可以填充阶段的详细信息和设置。

![Adding_a_new_stage_2.png](assets/adding-a-new-stage-2-350x332.png)

## 管理阶段设置

在页面详细信息中，您可以修改每个阶段的设置（如果您具有编辑权限）：

* 更改、添加或删除阶段(1)的截止日期
* 锁定阶段(2) — 如果阶段处于活动状态，则此选项将启动；对于非活动阶段，您将看到启动阶段的选项
* 通过内联编辑修改设置(3)
* 仅启用或禁用阶段(4)上需要一个决策
* 更改阶段(5)的隐私

![Managing_stage_settings.png](assets/managing-stage-settings-350x93.png)

也可以通过将审阅人从一个阶段拖放到另一个阶段来在阶段之间移动审阅人。 可用阶段将以蓝色突出显示，并清楚地标记每个阶段的放置区域。

![Moving_reviewers_between_stages.png](assets/moving-reviewers-between-stages-350x254.png)

## 暂存选项

每个阶段的[!UICONTROL 操作]菜单(1)具有以下选项：

* 全部发送消息(2) — 您可以向舞台上的所有审阅人发送提醒电子邮件
* 共享(3) — 可以向舞台添加新审阅者
* 删除阶段(4) — 如果验证所有者在该阶段中，系统将要求您为其选择新阶段
