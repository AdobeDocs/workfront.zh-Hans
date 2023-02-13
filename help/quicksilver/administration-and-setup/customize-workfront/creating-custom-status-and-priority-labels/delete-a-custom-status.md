---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 删除自定义状态
description: 如果自定义系统状态对您的组织不再有用，您可以将其删除。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 删除自定义状态

如果自定义系统状态对您的组织不再有用，您可以将其删除。

状态是锁定状态还是解锁状态决定了系统中所有组的状态是否被删除：

* 删除当前锁定的系统状态时，系统中所有组的状态都会被删除，无论该组是否对其进行了重命名。
* 相反，如果删除当前已解锁的系统状态，则系统中所有组的状态都将保持不变。


>[!NOTE]
>
>您无法删除以下项：
>
>* 在系统批准流程中使用的锁定或解锁系统状态，当前正在等待系统中至少一个对象的批准。
>
>  但是，您可以删除在单次使用或组级别审批流程中使用的已解锁系统状态，该流程当前正在等待审批。
>
>  您可以运行报告以查找对象并解析待处理的批准，然后重试删除状态。 有关说明，请参阅 [使用特定状态列出具有待批准流程的对象](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* 在审批流程中使用的状态，这些流程当前正在等待系统中至少一个对象的审批。


有关删除组状态的说明，请参阅 [删除群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## 删除自定义系统状态

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **项目首选项** > **状态**.

1. 要删除整个系统中的状态（包括各个组的状态），请将鼠标悬停在状态上，单击 **编辑**，然后确保 **锁定所有组** 中。 单击&#x200B;**保存**。

   或

   要删除系统状态，但将其保留给各个组，请将鼠标悬停在状态上，单击 **编辑**，然后确保 **锁定所有组** 中。 单击&#x200B;**保存**。

1. 将鼠标悬停在要删除的状态上，然后单击 **删除**.
1. 在显示的消息中，单击 **删除状态**.
1. 在 **删除状态** 框中，在标记为 **将当前具有此状态的所有项目设置为**.

   使用您正在删除的状态的项目将设置为您选择的状态。

   仅当状态与您删除的状态相同时，才会在下拉列表中提供状态。

   例如，如果您删除的状态等于“当前”，则只能选择同样等同于“当前”的状态。

1. 单击 **删除状态**.
