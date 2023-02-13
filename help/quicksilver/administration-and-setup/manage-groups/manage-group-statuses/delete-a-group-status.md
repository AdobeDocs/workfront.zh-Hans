---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 删除群组状态
description: 作为组管理员，如果组未在系统级别上配置为必需或锁定状态，或者在层次结构中为较高组配置，则可以删除所管理组的状态。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 删除群组状态

作为组管理员，如果组未在系统级别上配置为必需或锁定状态，或者在层次结构中为较高组配置，则可以删除所管理组的状态。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!NOTE]
>
>您无法删除以下项：
>
>* 内置状态：规划、当前和结束。 您可以更新其名称、编辑其颜色、锁定或解锁它们，但无法删除它们。
>* 至少一个与组或其子组关联的对象处于待批准状态的状态。


## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 删除群组状态

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组**.
1. 单击顶级群组的名称。
1. 在左侧面板中，单击 **状态**.
1. 在显示的状态列表中，将鼠标悬停在要删除的状态上，然后单击 **删除** 在最右边。

   ![](assets/hover-click-delete.jpg)

1. 在显示的框中，选择一个状态，以指定正在使用您正在删除的状态的对象（项目、任务、问题和审批流程）的替换状态。

   只有与您删除的状态等同的状态才可用。 例如，如果您删除的状态等于“当前”，则只能看到等同于“当前”的状态。

   此外，显示的状态取决于您删除的状态是已解锁还是已锁定：

   * **如果它没锁**:可以使用非隐藏的锁定状态和已解锁状态。

      除了为子组创建的状态之外，还包含从系统级别和上级别组继承的状态。

   * **如果它被锁定**:以下情况之一是真的：

      * 如果存在其他锁定状态和非隐藏状态，则只有这些状态可用。
      * 如果没有锁定的非隐藏状态，则默认的Workfront状态将可用，即使它处于隐藏或解锁状态也是如此。

         有关默认Workfront状态的信息，请参阅 [访问系统项目状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md), [访问系统任务状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)，以及有关 [访问系统问题状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md).

1. 单击 **删除状态**.

   如果删除状态是组中该类型的默认状态，则替换状态将替换。

   如果删除状态在项目首选项中设置为默认项目状态，则首选项现在将设置为替换状态。

## 删除群组时

删除某个组并替换为另一个组后，已删除的组所具有的任何唯一状态都会添加到替换组的状态中。 有关更多信息，请参阅 [移动或删除的群组中的自定义状态](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md).
