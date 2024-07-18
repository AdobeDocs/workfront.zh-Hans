---
title: 授予对Scenario Planner的访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Scenario Planner的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 授予对Scenario Planner的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Scenario Planner的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

除了访问Scenario Planner之外，具有非系统管理员访问级别的用户还必须具有财务数据的访问权限，才能查看计划中包含的任何财务信息，如预算、成本和工作角色费率。 有关详细信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>业务或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>查看或更高版本。 有关详细信息，请参阅<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">许可证概述</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront Scenario Planner购买附加许可证，才能访问本文中描述的功能。</p> <p>有关获取Workfront Scenario Planner的信息，请参阅<a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">使用Scenario Planner所需的访问权限</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看对Scenario Planner的访问权限或更高</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> <p>查看计划的权限或更高</p> <p>有关请求对计划的附加访问权限的信息，请参阅<a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">在方案规划者中请求对计划的访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 使用自定义访问级别配置用户对Scenario Planner的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击要用于此访问级别的&#x200B;**Scenario Planner**&#x200B;右侧的选项。

   >[!NOTE]
   >
   >请求或外部许可证类型不允许查看或编辑对Scenario Planner的访问权限。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

## 按许可证类型访问Scenario Planner

有关每个访问级别中的用户可以对Scenario Planner执行哪些操作的信息，请参阅[可用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)一文中的[Scenario Planner区域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario)部分。

## 按访问级别设置显示的Scenario Planner访问权限

以下信息可帮助您了解如何使用访问级别设置控制用户对Workfront Scenario Planner中信息的访问。

* [无访问权限](#no-access)
* [查看访问权限](#view-access)
* [编辑访问权限](#edit-access)

### 无权访问 {#no-access}

无权访问Scenario Planner的用户既无法在主菜单中看到添加到其布局模板的“方案”图标，也无法查看与其共享的计划和计划。 如果与无权访问Scenario Planner的用户共享指向计划的链接，则用户无法查看或编辑计划。

### 查看访问权限 {#view-access}

对Scenario Planner具有“查看”权限的用户可以执行以下操作：

* 查看主菜单![](assets/esp-icon-in-main-menu.png)中的“方案”图标，但“计划”区域为空，除非用户单击由其他用户共享的计划链接。
* 当另一用户共享指向计划的链接时，查看计划。

  这包括计划中的任何工作角色信息。

  如果接收用户还有权访问财务数据，它还包括工作角色费率和计划的成本信息。 有关详细信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

### 编辑访问权限 {#edit-access}

对Scenario Planner具有“编辑”权限的用户可以执行以下操作：

* 查看主菜单![](assets/esp-icon-in-main-menu.png)中的方案图标，并使用它访问计划数据。
* 创建计划。
* 查看、编辑和删除他们创建的计划。
* 查看、编辑和删除其他用户使用共享链接访问的计划。

  这包括计划中的任何工作角色信息。

  如果接收用户有权访问财务数据，它还包括工作角色费率和计划的成本信息。 有关详细信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
