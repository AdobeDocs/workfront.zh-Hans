---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置系统更新
description: Workfront在对象的[!UICONTROL 更新]区域生成自动系统更新，以记录用户对该对象执行的更改。 作为 [!DNL Workfront] 管理员，您可以配置哪些对象字段和操作 [!DNL Workfront] 跟踪以记录系统更新。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 52ba2457ac2870d23e325f64163b683756f88ad4
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 8%

---

# 配置系统更新

<!-- Audited: 5/2025 -->

[!DNL Adobe Workfront]在对象的[!UICONTROL 更新]区域生成自动系统更新以记录以下事件：

* 用户在对象字段中进行的更改
* 用户对对象执行的操作

这些系统更新包括以下类型的信息：

* 所做的更改
* 进行更改的用户的名称
* 更改的时间和日期

有关系统更新的详细信息，请参阅[系统跟踪的更新](../system-tracked-update-feeds/system-tracked-update-feeds.md)。

作为[!DNL Workfront]管理员，您可以配置[!DNL Workfront]跟踪哪些对象字段和操作来记录系统更新。

例如，您可以让[!DNL Workfront]跟踪用户对整个系统内的问题名称所做的所有更改。 然后，任何问题名称更改将作为系统更新显示在问题的[!UICONTROL 更新]区域。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td><p>新文档： [!UICONTROL Standard]</p>
   或
   <p>当前： [!UICONTROL 计划]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 确定对象类型的[!DNL Workfront]跟踪哪些字段

您可以确定用户在整个[!DNL Workfront]界面中更改与特定对象类型关联的信息时，[!DNL Workfront]跟踪哪些信息。 您可通过添加或删除希望[!DNL Workfront]跟踪该对象类型的字段来执行此操作。

>[!NOTE]
>
>* [!DNL Workfront]无法跟踪和记录有关已计算自定义字段的更新。
>* 您可以为项目、任务、问题、项目组合、项目和用户自定义系统更新。 您无法自定义模板、文档或时间表的系统更新，但[!DNL Workfront]确实记录了这些对象的系统更新。
>



* [添加您希望 [!DNL Workfront] 跟踪的字段](#add-fields-you-want-workfront-to-track)
* [删除您不希望跟踪的字段](#remove-fields-you-don-t-want-tracked)

### 添加您希望[!DNL Workfront]跟踪的字段 {#add-fields-you-want-workfront-to-track}

您可以添加希望[!DNL Workfront]在整个[!DNL Workfront]界面中跟踪特定对象类型的字段。 当用户更改该字段中的信息时，[!DNL Workfront]将有关更改的信息记录为对象的[!UICONTROL 更新]区域中的系统更新。

>[!NOTE]
>
>您最多可以在更新源中跟踪300个内置和自定义字段。 如果您要跟踪最大字段数，并且希望跟踪[!UICONTROL 所有字段]子选项卡中未显示的其他字段，则必须首先删除一些跟踪的字段，才能跟踪新字段。 有关从更新字段中删除字段的更多信息，请参阅[删除不想跟踪的字段](#remove-fields-you-don-t-want-tracked)。

{{step-1-to-setup}}

1. 在左侧的面板中，单击&#x200B;**[!UICONTROL 界面]**，然后单击&#x200B;**[!UICONTROL 更新馈送]**。

1. 单&#x200B;击&#x200B;**[!UICONTROL 添加字段]**，然后从下拉列表中选择要跟踪的对象。

1. 在出现的框中，开始键入对象的内置（标准）字段或自定义字段，然后当该对象出现在列表中时将其选定。

   >[!NOTE]
   >
   >如果[!DNL Workfront]已在跟踪该字段，则不能从列表中再次添加该字段。

1. 添加所有要[!DNL Workfront]跟踪的字段后，单击&#x200B;**[!UICONTROL 添加字段]**。 您添加的内置字段显示在&#x200B;**[!UICONTROL 内置字段]**&#x200B;子选项卡下，自定义字段显示在&#x200B;**[!UICONTROL 自定义字段]**&#x200B;子选项卡下。

   **[!UICONTROL All Fields]**&#x200B;子选项卡显示正在跟踪的内置和自定义字段。

### 删除您不希望跟踪的字段 {#remove-fields-you-don-t-want-tracked}

您可以删除不希望系统在[!DNL Workfront]界面中跟踪特定对象类型的字段。

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 界面]**，然后单击&#x200B;**[!UICONTROL 更新馈送]**。

1. 在&#x200B;**[!UICONTROL 跟踪的字段]**&#x200B;选项卡上，选择&#x200B;**[!UICONTROL 所有字段]**&#x200B;子选项卡。 当前被跟踪的内置和自定义字段都会显示。

1. 选择要停止跟踪的字段，然后单击&#x200B;**[!UICONTROL 删除]**。

1. 在出现的&#x200B;**[!UICONTROL 删除字段]**&#x200B;框中，单击&#x200B;**[!UICONTROL 是，删除它]**&#x200B;以进行确认。

有关以前跟踪的字段的任何更新将保留在记录这些字段的[!UICONTROL 更新]区域中。

## 确定对象类型跟踪的操作[!DNL Workfront]

您可以让[!DNL Workfront]在整个[!DNL Workfront]界面中跟踪用户可以对对象执行的以下操作。

例如，每次用户将分配更改为任务或问题时，您都可以让[!DNL Workfront]记录更新。 然后，该更改将作为系统更新显示在任务或问题的[!UICONTROL 更新]区域中。

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

要配置您希望[!DNL Workfront]跟踪哪些操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 界面]**，然后单击&#x200B;**[!UICONTROL 更新馈送]**。

1. 单击&#x200B;**[!UICONTROL 操作]**&#x200B;选项卡。

1. 选中某个操作的复选框可启用该操作，取消选中该复选框可禁用该操作。
1. 单击&#x200B;**[!UICONTROL 保存]**。

禁用某个操作时，先前记录的有关该操作的任何更新将保留在记录该操作的[!UICONTROL 更新]区域中。
