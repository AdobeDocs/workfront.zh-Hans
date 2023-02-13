---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 使用校样批准报表
description: 您可以使用校样批准报表查看环境中有关校样的信息。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# 使用校样批准报表

您可以使用校样批准报表查看环境中有关校样的信息。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证概述*</p> </td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别*</strong> </td> 
   <td> <p>编辑对以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报表、功能板和日历</p> </li> 
     <li> <p>创建过滤器、视图和分组</p> </li> 
    </ul> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用校样批准报表

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **报表**.
1. 单击 **新建报表**，然后滚动以选择 **校样批准**.

   ![](assets/proof-approval-report.png)

1. （可选）添加任何其他字段。
1. 单击 **保存并关闭**.

## 其他字段

您可以向校样批准报表中添加以下字段：

* **决策日期**:显示审批者对校样作出决定的日期。 您还可以在校样的“打印摘要”中找到此日期。
* **审批者阶段**:显示当前阶段信息。
* **工作流模板**:显示附加到校样的任何工作流模板。 如果没有附加模板，则列为空。
* **等待决定**:显示true，表示在以下情况下，在最新版本上未满足决策：

   * 校样尚未存档
   * 审批者所处的阶段处于活动状态
   * 校样待批

* **校样截止时间**:显示校样的截止时间。 每个阶段都必须指定一个截止日期，才能填充此字段。 字段显示最近激活的阶段的截止时间。

 
