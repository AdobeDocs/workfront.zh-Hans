---
title: 删除自定义条件
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: 您可以删除自定义条件。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 删除自定义条件

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 删除自定义条件

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **条件**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. 选择对象类型的选项卡(**项目**, **任务**&#x200B;或 **问题**)要删除的条件所在的位置。

1. 将鼠标悬停在要删除的条件上，然后单击 **删除** 图标 ![](assets/delete.png) 在最右边。
1. 在显示的确认消息中，单击 **删除条件**.

1. 在 **删除条件** 框中，为使用您删除的条件的所有项目在下拉列表中选择新条件。

   仅当自定义条件与您删除的内置条件等同时，它们才会在下拉列表中可用。 例如，如果您删除的条件等于“处于风险”，则只能选择同样等同于“处于风险”的自定义条件。

1. 单击 **删除条件**.

>[!NOTE]
>
>您无法删除内置条件，这些条件位于Target上、面临风险和有问题。 但是，您可以更改其名称和颜色。

有关自定义条件的信息，请参阅 [自定义条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
