---
user-type: administrator
product-area: system-administration;setup
title: 配置要在变更历史记录中跟踪的字段
description: 作为Workfront管理员，您可以配置Workfront跟踪哪些对象字段和操作。
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 6%

---

# 配置要在变更历史记录中跟踪的字段

{{highlighted-preview-article-level}}

Adobe Workfront会生成自动系统更新以记录以下事件：

* 用户在对象字段中进行的更改
* 用户对对象执行的操作

这些系统更新包括以下类型的信息：

* 所做的更改
* 进行更改的用户的名称
* 更改的时间和日期

作为Workfront管理员，您可以配置Workfront跟踪哪些对象字段和操作。

例如，您可以让Workfront跟踪用户对整个系统内的问题名称所做的所有更改。 然后，任何问题名称更改将作为条目显示在更改历史记录日志中。 有关详细信息，请参阅[查看和管理更改历史记录](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL 标准版]</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 字段跟踪限制

可跟踪的字段数限制由Workfront包定义。

| Workfront包 | 跟踪的最大字段数 |
|---------|----------|
| 选择 | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| 工作流选择 | 1000 |
| 工作流 Prime | 5000 |
| 工作流 Ultimate | 无限制 |

## 添加要跟踪的字段

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪>配置**。
1. 在配置屏幕上，单击&#x200B;**添加字段**。
1. 在&#x200B;**添加字段**&#x200B;框中，选择一个对象。 您可以开始键入对象名称，然后当它出现在列表中时将其选定。
1. 接下来，选择要跟踪该对象的字段名称。 您可以开始键入字段名称，然后当该字段显示在列表中时将其选定。

   自定义字段和本机字段均可用于该对象。
   已跟踪的字段将显示为列表中的选定字段。

   ![添加用于更改跟踪的字段](assets/change-history-config-add-fields.png)

1. 选择所有要跟踪的字段后，单击&#x200B;**添加**。

   这些字段将添加到“跟踪的字段”列表中。

## 删除您不再想要跟踪的字段

您可以删除不希望系统在整个Workfront界面中跟踪特定类型对象的字段。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**更改跟踪>配置**。
1. 在配置屏幕上，选择要停止跟踪的一个或多个字段。

   您可能会多次看到相同的字段名称。 这些字段按对象分组，以便您可以找到正确的字段。 您还可以使用屏幕顶部的搜索框。

1. 在屏幕底部的操作栏中选择&#x200B;**删除**。
1. 单击确认消息上的&#x200B;**删除**。

   这些字段会从跟踪的字段列表中删除。


