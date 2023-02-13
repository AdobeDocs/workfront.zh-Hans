---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: 配置系统更新
description: Workfront在对象中生成自动系统更新 [!UICONTROL 更新] 区域，以记录用户对对象执行的更改。 As a [!DNL Workfront] 管理员，可以配置哪些对象字段和操作 [!DNL Workfront] 跟踪以记录系统更新。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# 配置系统更新

[!DNL Adobe Workfront] 在对象中生成自动系统更新 [!UICONTROL 更新] 区域来记录以下事件：

* 用户在对象字段中所做的更改
* 用户对对象执行的操作

这些系统更新包括所做的更改、进行更改的用户名称以及更改的时间和日期。

As a [!DNL Workfront] 管理员，可以配置哪些对象字段和操作 [!DNL Workfront] 跟踪以记录系统更新。

例如，您可以 [!DNL Workfront] 跟踪用户对整个系统中问题名称所做的所有更改。 任何问题名称更改随后都会显示为问题的系统更新 [!UICONTROL 更新] 的上界。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 确定哪些字段 [!DNL Workfront] 对象类型的跟踪

您可以确定哪些信息 [!DNL Workfront] 跟踪用户在整个过程中更改与特定对象类型关联的信息的时间 [!DNL Workfront] 界面。 要执行此操作，请添加或删除所需的字段 [!DNL Workfront] 以跟踪该对象类型。

>[!NOTE]
>
>* [!DNL Workfront] 无法跟踪和记录有关计算自定义字段的更新。
>* 您可以为项目、任务、问题、项目组合、项目和用户自定义系统更新。 不能为模板、文档或工时单自定义系统更新，但 [!DNL Workfront] 会记录这些对象的系统更新。
>




* [添加所需字段 [!DNL Workfront] 跟踪](#add-fields-you-want-workfront-to-track)
* [删除您不希望跟踪的字段](#remove-fields-that-you-don-t-want-tracked)

### 添加所需字段 [!DNL Workfront] 跟踪 {#add-fields-you-want-workfront-to-track}

您可以添加所需的字段 [!DNL Workfront] 在 [!DNL Workfront] 界面。 当用户更改该字段中的信息时， [!DNL Workfront] 在 [!UICONTROL 更新] 对象的区域。

>[!NOTE]
>
>您最多可以跟踪更新馈送中300个内置和自定义字段。 如果要跟踪最大字段数，并且希望跟踪未在 [!UICONTROL 所有字段] 子选项卡中，您必须先删除一些跟踪的字段，才能跟踪新字段。 有关从更新字段中删除字段的详细信息，请参阅 [删除您不希望跟踪的字段](#remove-fields-that-you-don-t-want-tracked).

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧的面板中，单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. &#x200B;单击 **[!UICONTROL 添加字段]**，然后单击要跟踪的对象。

1. 在&#x200B; **[!UICONTROL 更新信息源]** 框中，开始键入对象的内置（标准）字段或自定义字段，然后单击以在列表中显示该字段时将其选中。

   如果 [!DNL Workfront] 已在跟踪该字段，则无法再从列表中添加一次。

1. 添加所有所需字段后 [!DNL Workfront] 要跟踪，请单击 **[!UICONTROL 添加字段]**.

   您添加的内置字段显示在 **[!UICONTROL 内置字段]** 子选项卡。

   您添加的自定义字段显示在 **[!UICONTROL 自定义字段]** 子选项卡。

   的 **[!UICONTROL 所有字段]** 子选项卡显示被跟踪的内置字段和自定义字段。

### 删除您不希望跟踪的字段 {#remove-fields-that-you-don-t-want-tracked}

您可以删除不希望系统在 [!DNL Workfront] 界面。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. 在 **[!UICONTROL 跟踪的字段]** 选项卡，选择 **[!UICONTROL 所有字段]** 子选项卡。

   这会显示当前正在跟踪的内置字段和自定义字段。

1. 选择要停止跟踪的字段，然后单击 **[!UICONTROL 删除]**.

1. 在 **[!UICONTROL 删除字段]** 框，单击 **[!UICONTROL 是，删除它]** 确认。

有关之前跟踪的字段的任何更新将保留在 [!UICONTROL 更新] 的区域。

## 确定哪些操作 [!DNL Workfront] 对象类型的跟踪

您可以 [!DNL Workfront] 跟踪用户可以在 [!DNL Workfront] 界面。

例如，您可以 [!DNL Workfront] 每次用户更改任务或问题的分配时记录更新。 然后，该更改将在 [!UICONTROL 更新] 中。

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
   <td>已创建或删除帐单记录</td> 
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

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 界面]** > **[!UICONTROL 更新信息源]**.

1. 单击 **[!UICONTROL 操作]** 选项卡。

1. 选择要启用的操作，或取消选择要禁用的操作。
1. 单击&#x200B;**[!UICONTROL 保存]**。

禁用某个操作时，之前记录的有关该操作的任何更新将保留在 [!UICONTROL 更新] 的区域。
