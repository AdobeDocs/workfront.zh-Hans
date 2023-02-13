---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 使用自定义状态作为群组的默认状态
description: 作为组管理员，您可以将自定义状态配置为所管理的组或子组的默认状态。 当系统需要为项目、任务或问题自动分配Workfront状态时，此功能非常有用。 项目、任务或问题始终显示您设置为默认状态的自定义状态，而不是显示它等同于的Workfront状态。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 使用自定义状态作为群组的默认状态

作为组管理员，您可以将自定义状态配置为所管理的组或子组的默认状态。 当系统需要为项目、任务或问题自动分配Workfront状态时，此功能非常有用。 项目、任务或问题始终显示您设置为默认状态的自定义状态，而不是显示它等同于的Workfront状态。

您配置的状态可以是为群组创建、从群组上方的群组继承或从系统级别继承的任何自定义状态。

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!INFO]
>
>**示例：** 您可以创建一个名为“已完成”的自定义状态，并将其设置为与Workfront状态“完成”等同的默认状态。
>
>然后，对于设置为在任务达到100%时更改为“完成”状态的任务，状态显示为“已完成”而不是“完成”。

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

## 问题状态

如果自定义状态为“问题”状态，则必须为其启用所有四种问题类型（错误报告、更改顺序、问题和请求）。 例如，在下面显示的问题状态中，由于未选中“更改订单”问题类型，因此无法将“重新打开”状态用作默认状态：

![](assets/all-4-issue-types-enabled.png)

## 将自定义状态设置为群组的默认状态

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).
1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png)，然后单击要创建或自定义状态的组名称。
1. 在左侧面板中，单击 **状态** ![](assets/gear-icon-settings.png).
1. 打开 **项目**, **任务**&#x200B;或 **问题** 选项卡，具体取决于要设置为默认状态的状态类型。
1. 单击 **设置默认状态** 在右上角附近。
1. 在显示的下拉区域中，在要设置默认状态的状态旁边，选择要设置的默认状态。
1. 单击&#x200B;**保存**。

   现在，状态可用作与群组关联的项目使用的默认状态。

1. 将自定义状态与您要在其中使用它的项目关联。

   通过将状态所在的组与项目关联，可将状态与项目关联。 仅当状态所在的组与项目关联时，用户才能使用自定义状态。

   >[!NOTE]
   >
   >如果将项目分配给其他组，则项目状态将重新加载，并可能发生更改。

   1. 转到要使用自定义状态的项目。
   1. 单击“更多”菜单 ![](assets/more-icon.png)，然后单击 **编辑**.
   1. 在 **编辑项目** 框中显示 **组** 字段 **项目关联**，选择与自定义状态关联的组。

   1. 单击 **保存更改**.

## 组将继承默认状态配置

在Workfront管理员将自定义状态配置为默认状态后，创建的新组将继承该配置。

同样，在群组管理员将自定义状态设置为默认状态后，群组正下方创建的新子组将继承该配置。

有关更多信息，请参阅 [组如何继承状态](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## 隐藏默认状态时

如果隐藏默认状态（通过为其启用“隐藏状态”选项），系统将尝试将其他等效类型的状态设置为默认状态。

如果没有对等类型的可用状态，则状态类型显示为 **隐藏** 和不适用于工作项。

![](assets/when-hide-default-status-no-equivalent.png)
