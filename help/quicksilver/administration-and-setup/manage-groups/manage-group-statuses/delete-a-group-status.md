---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 删除组状态
description: 作为组管理员，您可以删除您管理的组的状态（如果该组未在系统级别配置为必需或已锁定状态），或者删除层次结构中较高组的状态。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: 1554c067afcc548c7f7abd03dbc3a49404e3c89c
workflow-type: tm+mt
source-wordcount: '541'
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

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除组状态

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组**。
1. 单击顶级组的名称。
1. 在左侧面板中，单击&#x200B;**状态**。
1. 在显示的状态列表中，将鼠标悬停在要删除的状态上，然后在最右边显示&#x200B;**删除**&#x200B;时单击该状态。

   ![删除](assets/hover-click-delete.jpg)

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
