---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: 管理 [!UICONTROL 视图] 页面 [!DNL Workfront Proof]
description: 的 [!UICONTROL 视图] 页面允许您在一个位置查看和处理所有校样、文件和文件夹。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 56556d16-9aab-4b0e-b08c-ac5f1703e082
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1535'
ht-degree: 0%

---

# 管理 [!UICONTROL 视图] 页面 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

的 [!UICONTROL 视图] 页面允许您在一个位置查看和处理所有校样、文件和文件夹。

## 显示 [!UICONTROL 视图] 页面

1. 单击 **[!UICONTROL 视图]** 中。
1. 从下拉菜单(2)中，单击要查看的视图(3)。

![Views.png](assets/views-350x297.png)

## 更改 [!UICONTROL 视图] 页面布局

默认 [!UICONTROL 视图] 页面布局是缩略图列表。 在此布局中，您可以看到每个校样、文件（如果可能生成）和文件夹（如果已设置）的缩微图像，其他详细信息包含在单独的列中。

1. 单击 **[!UICONTROL 页面布局]** 图标(1)，然后选择所需的布局。

![Views_Page_Layout.png](assets/views-page-layout-350x140.png)

## 更改 [!UICONTROL 视图] 列表

要更改 [!UICONTROL 视图] 列表：

1. 单击 **[!UICONTROL 更改视图]** 按钮。\
   此按钮上显示的名称取决于您上次使用该按钮时选择的视图。\
   ![Views-Change_view_button.png](assets/views-chnge-view-button-350x205.png)

1. 在下拉菜单中单击其他视图：

   * **[!UICONTROL 所有项目]**:包括您有权查看的所有校样、文件和文件夹。 当您打开 [!UICONTROL 视图] 页面。 您可以选择在此视图中包含/排除已存档的校样。
   * **[!UICONTROL 活动项目]**:所有活动校样、文件和文件夹。
   * **[!UICONTROL 活动校样]**:您有权查看的所有活动（未存档）校样。
   * **[!UICONTROL 锁定的校样]**:仅锁定校样。
   * **[!UICONTROL 存档校样]**:仅存档校样(请参阅 [在中存档 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/archive.md))。

   * **[!UICONTROL 我的校样]**:仅显示您是其所有者且已委派给您的校样。 有关更多信息，请参阅 [在中指定临时校样所有者 [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).

   * **[!UICONTROL 等待决策的证明]**:仅显示您必须做出决策的校样
   * **[!UICONTROL 延迟校样]**:仅显示截止时间已过的校样
   * **[!UICONTROL 文件]**:仅显示文件
   在这些视图中，每个视图都包含以下列

   * **类型**:项目的图标，带有校样、文件或文件夹的图标
   * **名称**:校样、文件或文件夹的名称
   * **进度**:S=Sent， O=Opened， C=Comment， D=Decision（请参阅进度条）
   * **状态**: [!UICONTROL 待定，需要更改，已批准]
   * **决策**:作出决定的次数和所需数量
   * **所有者**:校样所有者的姓名\

      我的校样、等待决策的校样和延迟校样视图还有一个名为“我的截止日期”的列。 此列在明确添加为审核者/审批者的校样上显示您自己的截止日期。

      >[!NOTE]
      >
      >如果您从“视图”页面导航到其他位置，并在稍后的同一会话中返回到该页面，则会显示您最后选择的视图。

      您还可以创建自己的视图。 请参阅 [在中创建和管理自定义视图 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md) 以了解更多信息。




## 筛选项目

您可以过滤视图中列出的信息。

1. 单击 **显示过滤器** 图标(1)。\
   ![Filters.png](assets/filters-350x107.png)

1. 出现过滤条(2)，每个类别都有一个过滤下拉菜单(3)，用于选择您的首选值。 每个类别的默认值为“全部”。
1. 过滤器栏不会在您创建的自定义视图中显示。 对于这些视图，您可以在 [!UICONTROL 过滤器] 选项卡。 有关更多信息，请参阅 [在中创建和管理自定义视图 [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
1. 要应用所有选定的过滤器，请单击 [!UICONTROL 过滤器] 图标(4)。\
   ![Filters_2.png](assets/filters-2-350x102.png)

您选择的过滤器值在您更改之前会一直有效。 如果要再次查看并访问项目的完整列表，则必须将所有过滤器值更改回默认值，即 **[!UICONTROL 全部]**.

>[!NOTE]
>
>如果您设置了过滤选项，然后通过单击 [!UICONTROL 隐藏过滤器] 图标(5)，则当您更改视图时，该栏会再次自动显示。 如果在所有过滤器都设置为默认全部选项的情况下隐藏过滤栏，则在更改视图时，过滤栏会保持隐藏状态。

## 对项目排序

创建新校样（或版本）或上传新文件时，该校样会显示在 [!UICONTROL 所有项目] 列表。 最早的项目将显示在列表底部。

要按不同的排序顺序查看列表，请执行以下操作：

1. 执行下列操作之一：

   * 单击列表中的列标题之一：类型、名称、状态、决策或所有者。\

      例如，如果要按字母顺序查看校样/文件，请单击“名称”标题一次(1)，以按名称升序(A - Z)对列表进行排序。\
      您可以再次单击校样名称标题(2)以反转顺序并以降序(Z - A)显示校样。

   * 单击 [!UICONTROL 视图] 页面，按创建日期（最新或最旧）或类型、名称、状态、决策或所有者进行排序。\

      ![Views-Sort_down_arrow.png](assets/views-sort-down-arrow-350x124.png)\
      如果您的列按升序排序，则列标题将在列名称旁边显示一个向上箭头。 要反转顺序（降序），请单击相关列标题（这将在列名称旁边显示一个向下箭头）。

   * 仅当您保留在“所有项目”页面上时，才对项目排序顺序所做的更改才会持续。 如果您从“所有项目”页面导航离开，稍后又返回到该页面，则这些项目将再次按默认的时间顺序逆序列出。

## 查看校样摘要

要查看有关校样的更多详细信息，请执行以下操作：

1. 单击校样图像左侧的箭头。\
   箭头向下指向，校样摘要将显示在有关校样的基本信息下方。 校样摘要显示：

   * **校样摘要**:验证的总体状态
   * **阶段**:指示验证的截止时间和已做出和需要的决定的数量
   * **审阅人**:将列出每个审阅人的名称、角色和进度
   * **版本**:正在查看的校样版本和可用版本总数
   * **文件夹**:校样所在的文件夹
   * **州**:活动、锁定、草稿或已提交

1. （可选）如果您对校样具有编辑权限，并且校样具有阶段，请单击 **[!UICONTROL 更多]** （三个圆点）菜单，用于访问以下选项：

   * **[!UICONTROL 全部消息]**:向舞台上的所有审阅人发送电子邮件。
   * **[!UICONTROL 共享]**:添加新审阅人
   * **[!UICONTROL 删除阶段]**

1. （可选）单击审阅人的 **[!UICONTROL 更多]** （三个圆点）菜单，用于执行以下任一操作：

   * 向审阅人发送提醒消息。
   * 编辑审阅人对校样的设置。\

      出现的“编辑审阅人”框，您不仅可以更改角色和电子邮件警报，还可以更改审阅人的显示名称。 请注意，显示名称只能在特定校样中更改，而不能在“联系人”页面的审阅人详细信息中更改。 请参阅 [联系人](https://support.workfront.com/hc/en-us/sections/115000920808-Contacts) 以了解更多信息。

   * 选择要作为校样主要决策者的审阅人。
   * 从校样中删除审阅人。
   * 您还可以为添加到校样的审阅人更改角色和电子邮件警报。

## 包含和排除存档的校样

的 [!UICONTROL 所有项目] 默认情况下，“视图”显示所有活动和锁定的校样、文件和文件夹。 它还提供了在视图中包含或排除已存档校样的选项。\
要包含存档的校样，请执行以下操作：

1. 选择视图时，单击 **[!UICONTROL 包含存档校样]**.\
   ![Views-include_archived_proods.png](assets/views-include-archived-proofs-350x188.png)\
   存档的校样将显示一个存档图标，以便与其他校样区分开来。\
   ![Views-Archived_icon.png](assets/views-archived-icon.png)

## 从列表视图打开项目

1. 执行下列操作之一：

   * 要查看有关校样、文件或文件夹的详细信息，请单击其名称。
   * 要在校样查看器中打开校样，请单击 **[!UICONTROL 转到校样]**.\

      有关校对查看器的信息，请参阅 [查看验证](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## 对多个项目执行操作

要选择多个项目，请执行以下操作：

1. 单击列表上方的复选框。\
   ![Views-select_all_items_checkbox.png](assets/views-select-all-items-checkbox-350x193.png)

1. 在“视图”列表上方显示的额外选项中，对您选择的文件执行以下任一操作：

   * 单击 **[!UICONTROL 标记]** 向这些项目添加标记。
   * 单击 **[!UICONTROL 移动到]** 将选定项目移至其他文件夹(或者，如果选择（未选择文件夹），则将项目移出文件夹。
   * 单击 **[!UICONTROL 共享选定项目]** 与其他审阅人共享所有这些项目。

      ![Share_button-small.png](assets/share-button-small.png)

   * 单击 **[!UICONTROL 删除]** 将选定项目移到垃圾桶。\

      ![Trash_button.png](assets/trash-button.png)

   * 单击 **[!UICONTROL 更多]** 菜单，以了解其他可用操作。

   * 该操作将仅应用于具有可用特定选项的选定项目的操作。 例如，如果选择文件和校样，然后选择 [!UICONTROL 锁]，则只会锁定校样（因为您无法锁定文件）

## 将项目移到文件夹

如果您具有执行此操作的编辑权限，则可以将校样、文件和文件夹移动到 [!UICONTROL 视图] 页面。

1. 通过单击最上方文件夹左侧的箭头，在侧栏中打开文件夹树。
1. 执行下列操作之一：

   * 要移动一个项目，请单击并按住该项目，然后将其拖放到要放置该项目的文件夹中。
   * 要同时移动多个项目，您可以选中项目左侧的复选框，然后单击**[!UICONTROL 移动到]**在列表上方，选择要放置这些文件夹的文件夹，或为其创建新文件夹。
