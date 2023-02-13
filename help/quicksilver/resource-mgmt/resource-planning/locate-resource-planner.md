---
product-area: resource-management
navigation-topic: resource-planning
title: 查找资源计划员
description: “(这源于本文：当该内容正式发布时，在文章中起草该内容：/Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)`
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# 查找资源计划员

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

您可以使用资源计划器来管理资源到项目的分配。 您可以同时访问多个项目的资源计划员，也可以从项目的“业务案例”区域访问一个项目的资源计划员。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>在全局区域中计划或更高版本以定位资源计划员</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对资源管理的访问权限或更高权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目和用户的权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始使用资源计划器之前，请确保满足访问和使用资源计划器的所有先决条件。 这样，在开始对资源进行预算编制之前，您就可以确保资源计划员显示正确的信息。

有关资源计划员先决条件的信息，请参阅 [资源规划入门](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## 查找资源计划员

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

您可以在Workfront的两个区域中找到资源计划器，具体取决于您是要为多个项目预算资源，还是只为一个项目预算资源。

* [对多个项目使用资源计划器](#use-the-resource-planner-for-multiple-projects)
* [将资源计划器用于一个项目](#use-the-resource-planner-for-one-project)

### 对多个项目使用资源计划器 {#use-the-resource-planner-for-multiple-projects}

在将资源计划器用于多个项目时，资源的分配编号表示跨多个项目的编号。

要在“资源”区域访问“计划员”部分，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **资源化**. 默认情况下，计划员会显示。  有关资源计划员中预算资源的信息，请参阅文章 [使用“项目”和“职责”视图在资源计划员中预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 将鼠标悬停在左侧面板上，然后单击 **资源池**.\
   有关创建资源池的信息，请参阅 [创建资源池](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### 将资源计划器用于一个项目 {#use-the-resource-planner-for-one-project}

在将资源计划器用于一个项目时，资源的分配编号表示选定项目的编号。

1. 转到要对资源进行预算的项目。
1. 单击 **商业案例** 中。
1. 滚动到 **资源预算编制** 部分。
1. 单击 **编辑资源预算** 向项目添加资源池并开始对资源进行预算。

   >[!TIP]
   >
   >只有当项目没有与其关联的资源池时，才能在“业务案例”的“资源预算”区域中添加资源池。 当项目已具有资源池时，默认情况下，池中的用户及其作业角色将显示在“资源预算”区域中。

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   有关一个项目的预算编制资源的信息，请参阅文章 [业务案例中的预算资源](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
