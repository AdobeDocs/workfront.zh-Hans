---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: 删除自定义状态
description: 如果自定义系统状态对您的组织不再有用，您可以删除该状态。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---

# 删除自定义状态

如果自定义系统状态对您的组织不再有用，您可以删除该状态。

状态是锁定还是解除锁定决定着系统中所有组的状态是否被删除：

* 删除当前锁定的系统状态时，系统会删除系统中所有组的状态，无论组是否已重命名它。
* 相反，当您删除当前已解锁的系统状态时，系统中所有组的状态都将保持不变。


>[!NOTE]
>
>您无法删除以下项：
>
>* 在系统审批流程中使用的锁定或解锁系统状态，当前正等待审批系统中的至少一个对象。
>
>  但是，您可以删除在一次性使用或当前未决批准的组级别批准流程中使用的未锁定系统状态。
>
>  您可以运行报告以查找对象并解决待审批问题，然后再次尝试删除状态。 有关说明，请参阅[使用特定状态列出具有未决批准流程的对象](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md)。
>
>* 审批流程中使用的状态，当前为系统中至少一个对象的未决审批。

有关删除组状态的说明，请参阅[删除组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md)。

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
     <p>新增：标准</p>
     <p>或</p>
     <p>当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除自定义系统状态

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项** > **状态**。

1. 要删除整个系统（包括单个组）的状态，请将鼠标悬停在该状态上，单击&#x200B;**编辑**，然后确保已选择&#x200B;**锁定所有组**。 单击&#x200B;**保存**。

   或

   要删除系统状态但保留单个组的状态，请将鼠标悬停在该状态上，单击&#x200B;**编辑**，然后确保取消选择所有组的&#x200B;**锁定**。 单击&#x200B;**保存**。

1. 将鼠标悬停在要删除的状态上，然后单击&#x200B;**删除**。
1. 在显示的消息中，单击&#x200B;**删除状态**。
1. 在显示的&#x200B;**删除状态**&#x200B;框中，在标记为&#x200B;**将当前具有此状态的所有项目设置为**&#x200B;的字段中选择一个状态。

   使用您要删除的状态的项目将被设置为您选择的状态。

   仅当状态与您正在删除的状态相等时，下拉列表中的状态才可用。

   例如，如果要删除与“当前”相等的状态，则只能选择与“当前”相等的状态。

1. 单击&#x200B;**删除状态**。
