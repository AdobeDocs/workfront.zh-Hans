---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 删除组状态
description: 作为组管理员，您可以删除您管理的组的状态（如果该组未在系统级别配置为必需或已锁定状态），或者删除层次结构中较高组的状态。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 删除组状态

作为组管理员，您可以删除您管理的组的状态（如果该组未在系统级别配置为必需或已锁定状态），或者删除层次结构中较高组的状态。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!NOTE]
>
>您无法删除以下项：
>
>* 内置状态为“计划”、“当前”和“完成”。 您可以更新他们的姓名、编辑他们的颜色、锁定或解锁他们，但无法删除他们。
>* 与组或其子组相关联的至少一个对象处于待审批状态。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

## 删除组状态

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**组**。
1. 单击顶级组的名称。
1. 在左侧面板中，单击&#x200B;**状态**。
1. 在显示的状态列表中，将鼠标悬停在要删除的状态上，然后在最右边显示&#x200B;**删除**&#x200B;时单击该状态。

   ![](assets/hover-click-delete.jpg)

1. 在显示的框中，选择一个状态，为正在使用要删除状态的对象（项目、任务、问题和审批流程）指定替换状态。

   只有与您正在删除的状态等同的状态才可用。 例如，如果要删除与“当前”相等的状态，则只能看到与“当前”相等的状态。

   此外，显示的状态取决于您要删除的状态是“已解锁”还是“已锁定”：

   * **如果已解锁**：非隐藏锁定和未锁定状态可用。

     除了为子组创建的状态外，还包括从系统级别和高级别组继承的状态。

   * **如果锁定**：以下项之一为true：

      * 如果有其他锁定、非隐藏状态，则只有这些状态可用。
      * 如果没有锁定的非隐藏状态，则默认的Workfront状态将可用，即使处于隐藏或未锁定状态也是如此。

        有关默认Workfront状态的信息，请参阅[访问系统项目状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)，[访问系统任务状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)，以及[中有关4个必需问题状态的信息。访问系统问题状态列表](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)。

1. 单击&#x200B;**删除状态**。

   如果删除的状态是组中该类型的默认状态，则替换状态将取代该状态。

   如果在项目首选项中将已删除状态设置为默认项目状态，则首选项现在设置为替换状态。

## 删除组时

当删除组并将其替换为另一个组时，已删除组具有的任何唯一状态都将添加到替换组的状态。 有关详细信息，请参阅[移动或删除的组中的自定义状态](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md)。
