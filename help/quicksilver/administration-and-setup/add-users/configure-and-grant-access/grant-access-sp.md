---
title: 授予对方案计划员的访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对方案计划员的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 授予对方案计划员的访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对方案计划员的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

除了对方案计划员的访问权限之外，具有非系统管理员访问权限级别的用户还必须具有财务数据的访问权限，才能查看计划中包含的任何财务信息，如预算、成本和职务角色费率。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>业务或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本。 有关更多信息，请参阅 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront方案规划器购买额外的许可证才能访问本文中所述的功能。</p> <p>有关获取Workfront方案计划员的信息，请参阅 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">使用方案计划员所需的访问权限</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看方案计划员的访问权限或更高权限</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> <p>查看计划的权限或更高权限</p> <p>有关请求对计划进行额外访问的信息，请参阅 <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">请求对方案计划员中计划的访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用自定义访问级别配置用户对方案规划器的访问权限

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击右侧的选项 **方案规划器** 用于此访问级别。

   >[!NOTE]
   >
   >“请求”或“外部”许可证类型不允许“查看”或“编辑”访问方案计划员。

1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

## 按许可证类型访问方案计划员

有关每个访问级别中的用户可以使用方案计划员执行的操作的信息，请参阅部分 [方案计划员区域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 按访问级别设置的方案计划员访问

以下信息可帮助您了解如何使用访问级别设置控制用户对Workfront方案计划员中信息的访问。

* [无权访问](#no-access)
* [查看访问](#view-access)
* [编辑访问权限](#edit-access)

### 无权访问 {#no-access}

无权访问方案计划员的用户在将其添加到其布局模板时，既无法在主菜单中看到方案图标，也无法查看与他们共享的计划和方案。 如果与无权访问方案计划员的用户共享指向计划的链接，则用户将无法查看或编辑计划。

### 查看访问 {#view-access}

具有方案计划员查看权限的用户可以执行以下操作：

* 请参阅主菜单中的方案图标 ![](assets/esp-icon-in-main-menu.png)，但“计划”区域为空，除非用户单击其他用户共享的计划链接。
* 当其他用户共享指向该计划的链接时，查看计划。

   这包括计划中的任何职务职责信息。

   此外，如果收件人用户也有权访问财务数据，则还包括有关计划的职务角色费率和成本信息。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### 编辑访问权限 {#edit-access}

具有方案计划员编辑访问权限的用户可以执行以下操作：

* 请参阅主菜单中的方案图标 ![](assets/esp-icon-in-main-menu.png) 并使用它访问计划数据。
* 创建计划。
* 查看、编辑和删除他们创建的计划。
* 查看、编辑和删除其他用户通过共享链接访问的计划。

   这包括计划中的任何职务角色信息。

   此外，如果收件人用户有权访问财务数据，则还包括有关计划的工作角色费率和成本信息。 有关更多信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
