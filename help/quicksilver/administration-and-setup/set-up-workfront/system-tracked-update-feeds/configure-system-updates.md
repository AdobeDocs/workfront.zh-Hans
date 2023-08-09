---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置系统更新
description: Workfront在对象的 [!UICONTROL 更新] 区域来记录用户对对象执行的更改。 作为 [!DNL Workfront] 管理员，您可以配置哪些对象字段和操作 [!DNL Workfront] 用于记录系统更新的轨道。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 7%

---

# 配置系统更新

[!DNL Adobe Workfront] 在对象的 [!UICONTROL 更新] 区域以记录以下事件：

* 用户在对象字段中进行的更改
* 用户对对象执行的操作

这些系统更新包括已进行的更改、进行更改的用户名称以及更改的时间和日期。

有关系统更新的详细信息，请参阅 [系统跟踪更新](../system-tracked-update-feeds/system-tracked-update-feeds.md).

作为 [!DNL Workfront] 管理员，您可以配置哪些对象字段和操作 [!DNL Workfront] 用于记录系统更新的轨道。

例如，您可以 [!DNL Workfront] 跟踪用户对整个系统中的问题名称所做的所有更改。 然后，任何问题名称更改将作为系统更新出现在问题的 [!UICONTROL 更新] 区域。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 确定哪些字段 [!DNL Workfront] 跟踪对象类型

您可以确定哪些信息 [!DNL Workfront] 跟踪用户在整个过程中更改与特定对象类型关联的信息的情况 [!DNL Workfront] 界面。 您可以通过添加或删除所需字段来实现这一点 [!DNL Workfront] 以跟踪该对象类型。

>[!NOTE]
>
>* [!DNL Workfront] 无法跟踪和记录有关计算的自定义字段的更新。
>* 您可以为项目、任务、问题、项目组合、项目和用户自定义系统更新。 您无法自定义模板、文档或工时表的系统更新，但是 [!DNL Workfront] 会记录这些对象的系统更新。
>



* [添加所需字段 [!DNL Workfront] 要跟踪的](#add-fields-you-want-workfront-to-track)
* [删除您不希望跟踪的字段](#remove-fields-that-you-don-t-want-tracked)

### 添加所需字段 [!DNL Workfront] 要跟踪的 {#add-fields-you-want-workfront-to-track}

您可以添加所需的字段 [!DNL Workfront] 在整个中跟踪特定类型的对象 [!DNL Workfront] 界面。 当用户更改该字段中的信息时， [!DNL Workfront] 将有关更改的信息作为系统更新记录在 [!UICONTROL 更新] 对象的区域。

>[!NOTE]
>
>您最多可以在更新源中跟踪300个内置和自定义字段。 如果您要跟踪最大字段数，并且希望跟踪未在 [!UICONTROL 所有字段] 子选项卡，您必须首先删除一些跟踪的字段才能跟踪新字段。 有关从更新字段中移除字段的更多信息，请参阅 [删除您不希望跟踪的字段](#remove-fields-that-you-don-t-want-tracked).

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧的面板中，单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. 单&#x200B;击 **[!UICONTROL 添加字段]**，然后单击要跟踪的对象。

1. 在&#x200B; **[!UICONTROL 更新信息源]** 框，开始键入对象的内置（标准）字段或自定义字段，然后单击以在对象出现在列表中时将其选中。

   如果 [!DNL Workfront] 已在跟踪该字段，您无法再次从列表中添加该字段。

1. 添加所需的所有字段后 [!DNL Workfront] 要跟踪，请单击 **[!UICONTROL 添加字段]**.

   您添加的内置字段显示在 **[!UICONTROL 内置字段]** 子选项卡。

   您添加的自定义字段显示在 **[!UICONTROL 自定义字段]** 子选项卡。

   此 **[!UICONTROL 所有字段]** 子选项卡同时显示内置字段和正在跟踪的自定义字段。

### 删除您不希望跟踪的字段 {#remove-fields-that-you-don-t-want-tracked}

您可以删除不希望系统跟踪特定类型对象的字段，在 [!DNL Workfront] 界面。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. 在 **[!UICONTROL 跟踪的字段]** 选项卡，选择 **[!UICONTROL 所有字段]** 子选项卡。

   这会显示当前跟踪的内置和自定义字段。

1. 选择要停止跟踪的字段，然后单击 **[!UICONTROL 移除]**.

1. 在 **[!UICONTROL 删除字段]** 框中，单击 **[!UICONTROL 是的，删除它]** 以确认。

有关以前跟踪的字段的任何更新将保留在 [!UICONTROL 更新] 被记录的区域。

## 确定哪些操作 [!DNL Workfront] 跟踪对象类型

您可以 [!DNL Workfront] 在整个过程中跟踪用户可以对对象执行的以下操作 [!DNL Workfront] 界面。

例如，您可以 [!DNL Workfront] 每次用户将分配更改为任务或问题时记录更新。 然后，此更改将作为系统更新显示在 [!UICONTROL 更新] 任务或问题的区域。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong> </th> 
   <th><strong>对象</strong> </th> 
   <th><strong>默认状态</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>分配已更改</td> 
   <td>任务，问题</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>基线已删除</td> 
   <td>项目</td> 
   <td> <p>已禁用</p> </td> 
  </tr> 
  <tr> 
   <td>开票记录已创建或删除</td> 
   <td>项目</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>文档已创建或删除</td> 
   <td>项目、任务、问题、投资组合和计划</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>费用已创建或删除</td> 
   <td>项目、任务</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>小时已记录或删除</td> 
   <td>项目、任务、问题</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>问题已删除</td> 
   <td>项目</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>任务已删除</td> 
   <td>项目</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>默认的访问权限已被更改</td> 
   <td>项目、任务、问题、文档、项目组合、程序</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
  <tr> 
   <td>订阅评论对象</td> 
   <td>项目、任务、问题</td> 
   <td> <p>已启用</p> </td> 
  </tr> 
 </tbody> 
</table>

配置要执行的操作 [!DNL Workfront] 要跟踪：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. 单击 **[!UICONTROL 操作]** 选项卡。

1. 选择操作以启用它，或取消选择操作以禁用它。
1. 单击&#x200B;**[!UICONTROL 保存]**。

禁用某个操作时，之前记录的有关该操作的任何更新都会保留在 [!UICONTROL 更新] 记录区域。
