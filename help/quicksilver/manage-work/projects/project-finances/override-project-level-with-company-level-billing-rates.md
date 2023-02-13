---
product-area: projects
navigation-topic: financials
title: 使用公司层开单费率改写项目层开单费率
description: 使用公司层开单费率改写项目层开单费率
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 使用公司层开单费率改写项目层开单费率

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

您可以将项目配置为使用公司级别的开单费率，而不是项目级别的开单费率。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目和财务数据的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限，并具有管理财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 启用公司层开单费率改写选项

当公司与某个项目关联并且启用此选项时，对公司层开单费率所做的更改将覆盖该项目中设置的开单费率。

当用户手动重新计算项目的财务时，将应用对公司级开单费率的任何更改。 历史收入计算也会被覆盖，除非它们被标记为已开单。

1. 转到项目。
1. 单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png) 在标题中项目名称旁边，然后单击 **编辑**.
1. 在 **金融** 部分，启用 **允许公司级开单费率改写项目级开单费率**.

   >[!CAUTION]
   >
   >启用此选项将覆盖历史收入计算，除非它们被标记为已开单。 您可以通过创建开单记录来保留历史收入计算。 有关更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md)

1. 单击 **保存更改**.

## 更新公司层开单费率，并将其应用于项目

在项目中启用公司层开单费率改写选项后，在重新计算财务后，对公司开单费率所做的更改将应用于项目。

>[!NOTE]
>
>用户必须在其访问级别拥有对公司的访问权限，才能更新公司级别的账单费率。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置**.
1. 单击 **公司**.
1. 单击与您为其启用公司层开单费率覆盖的项目关联的公司名称。
1. 单击 **计费费率** 中。
1. 在 **公司账单费率** 字段，然后按Enter。
1. 要更新一个或多个项目的公司费率，请执行以下操作之一：

   * 多个项目：
   1. 转到项目列表。
   1. 选中与要更新的项目对应的复选框。
   1. 单击 **编辑**.
   1. 在设置部分中，启用 **重新计算成本和收入** 选项。
   1. 单击 **保存更改**.
   * 单个项目：

      1. 转到您为其启用公司层开单费率改写的项目。
      1. 单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png) 在标题中项目名称旁边，然后单击 **重新计算财务**.
