---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 使用自定义状态作为组的默认状态
description: 作为组管理员，您可以将自定义状态配置为您管理的组或子组的默认状态。 当系统需要自动将Workfront状态分配给项目、任务或问题时，这将很有用。 项目、任务或问题始终显示您设置为默认状态的自定义状态，而不是显示它相当于的Workfront状态。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 0%

---

# 使用自定义状态作为组的默认状态

作为组管理员，您可以将自定义状态配置为您管理的组或子组的默认状态。 当系统需要自动将Workfront状态分配给项目、任务或问题时，这将很有用。 项目、任务或问题始终显示您设置为默认状态的自定义状态，而不是显示它相当于的Workfront状态。

您配置的状态可以是为该组创建的任何自定义状态，继承自该组上方的组，或从系统级别继承。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!INFO]
>
>**示例：**&#x200B;您可以创建一个名为“已完成”的自定义状态，并将其设置为等同于Workfront状态“已完成”的默认状态。
>
>然后，对于设置为在任务达到100%时更改为完成状态的任务，状态将显示为已完成，而不是完成。

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

## 问题状态

如果自定义状态是问题状态，则必须为其启用所有四种问题类型（错误报告、更改顺序、问题和请求）。 例如，在下面显示的问题状态中，由于未选择“更改单”问题类型，因此不能将“重新打开”状态用作默认状态：

![](assets/all-4-issue-types-enabled.png)

## 将自定义状态设置为组的默认状态

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。
1. 在左侧面板中，单击&#x200B;**组** ![](assets/groups-icon.png)，然后单击要创建或自定义状态的组的名称。
1. 在左侧面板中，单击&#x200B;**状态** ![](assets/gear-icon-settings.png)。
1. 打开&#x200B;**项目**、**任务**&#x200B;或&#x200B;**问题**&#x200B;选项卡，具体取决于要设置为默认状态的状态类型。
1. 单击右上角附近的&#x200B;**设置默认状态**。
1. 在显示的下拉区域中，在要设置默认状态的状态旁边选择要设置的默认状态。
1. 单击&#x200B;**保存**。

   该状态现在可作为默认状态用于与组关联的项目。

1. 将自定义状态与要使用该状态的项目关联。

   通过将状态所在的组与项目相关联，可将状态与项目相关联。 仅当状态所在的组与项目相关联时，用户才能使用自定义状态。

   >[!NOTE]
   >
   >如果将项目分配给其他组，则项目状态将重新加载并可能发生变化。

   1. 转到要在其中使用自定义状态的项目。
   1. 单击“更多”菜单![](assets/more-icon.png)，然后单击&#x200B;**编辑**。
   1. 在显示的&#x200B;**编辑项目**&#x200B;框中，在&#x200B;**项目关联**&#x200B;下的&#x200B;**组**&#x200B;字段中，选择与自定义状态关联的组。

   1. 单击&#x200B;**保存更改**。

## 组继承默认状态配置

Workfront管理员将自定义状态配置为默认状态后，创建的新组将继承该配置。

同样，组管理员将自定义状态设置为默认状态后，直接在组下创建的新子组将继承该配置。

有关详细信息，请参阅[组如何继承状态](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md)。

## 默认状态为隐藏时

如果隐藏默认状态（通过为其启用“隐藏状态”选项），则系统会尝试将另一个等效类型的状态设置为默认状态。

如果没有对等类型的可用状态，则状态类型显示为&#x200B;**隐藏**，且不可用于工作项。

![](assets/when-hide-default-status-no-equivalent.png)
