---
title: 删除自定义完成情况
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 您可以删除自定义完成情况。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 删除自定义完成情况

如果不再需要某个自定义条件，您可以删除该条件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除自定义完成情况

{{step-1-to-setup}}

1. 单击&#x200B;**项目首选项** > **条件**。

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. 选择要删除的条件所在的对象类型（**项目**、**任务**&#x200B;或&#x200B;**问题**）的选项卡。

1. 将鼠标悬停在要删除的条件上，然后单击最右侧显示的&#x200B;**删除**&#x200B;图标![删除](assets/delete.png)。
1. 在显示的确认消息中，单击&#x200B;**删除条件**。

1. 在出现的&#x200B;**删除条件**&#x200B;框中，在下拉列表中选择一个新条件，以用于使用要删除的条件的所有项目。

   仅当自定义条件与您要删除的内置条件相等时，它们才在下拉列表中可用。 例如，如果要删除与“处于风险中”相等的条件，则只能选择与“处于风险中”相等的自定义条件。

1. 单击&#x200B;**删除条件**。

>[!NOTE]
>
>您无法删除内置完成情况，这些完成情况符合目标、存在风险和存在问题。 但是，您可以更改它们的名称和颜色。

有关自定义条件的信息，请参阅[自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)。
