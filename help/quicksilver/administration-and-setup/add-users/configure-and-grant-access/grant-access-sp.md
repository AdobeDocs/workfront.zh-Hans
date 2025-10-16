---
title: 授予对Scenario Planner的访问权限
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Scenario Planner的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# 授予对Scenario Planner的访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Scenario Planner的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

除了访问Scenario Planner之外，具有非系统管理员访问级别的用户还必须具有财务数据的访问权限，才能查看计划中包含的任何财务信息，如预算、成本和工作角色费率。 有关详细信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront包</p> </td> 
   <td>业务或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>浅色或更高</p>
   <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront Scenario Planner购买附加许可证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对Scenario Planner的访问权限或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> <p>查看计划的权限或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用自定义访问级别配置用户对Scenario Planner的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击要用于此访问级别的&#x200B;**Scenario Planner**&#x200B;右侧的选项。

   >[!NOTE]
   >
   >请求或外部许可证类型不允许查看或编辑对Scenario Planner的访问权限。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续执行[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)和[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

## 按许可证类型访问Scenario Planner

有关每个访问级别中的用户可以对Scenario Planner执行哪些操作的信息，请参阅[可用于每个对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario)一文中的[Scenario Planner区域](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)部分。

## 按访问级别设置显示的Scenario Planner访问权限

以下信息可帮助您了解如何使用访问级别设置控制用户对Workfront Scenario Planner中信息的访问。

* [无访问权限](#no-access)
* [查看访问权限](#view-access)
* [编辑访问权限](#edit-access)

### 无访问权限 {#no-access}

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
