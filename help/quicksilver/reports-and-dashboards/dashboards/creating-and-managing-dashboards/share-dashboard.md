---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 共享功能板
description: 您的Adobe Workfront管理员在用户分配访问级别时，会授予用户查看或编辑功能板的访问权限。 除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定功能板的权限。
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# 共享功能板

您的Adobe Workfront管理员在用户分配访问级别时，会授予用户查看或编辑功能板的访问权限。 有关授予对问题的访问权限的更多信息，请参阅 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定功能板的权限。 有关访问级别和权限的更多信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

权限特定于Workfront中的一个项目，并定义可以对该项目执行哪些操作。

>[!NOTE]
>
>Workfront管理员可以添加或删除系统中所有用户的任何项目的权限，而不是这些项目的所有者。

## 访问要求

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>查看对报表、功能板、日历的访问权限或更高权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>查看功能板权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建功能板，然后才能共享该功能板。

有关创建功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## 有关共享功能板的注意事项

除了以下注意事项外，另请参阅 [共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 默认情况下，功能板的创建者具有其“管理”权限。

* 您可以与其他个人、团队、组、工作角色或公司共享您创建的功能板。 您还可以共享其他已创建并与您共享的功能板。
* 您还可以通过在整个系统范围内显示这些组件来与整个组织共享它们。
* 您可以共享单个功能板，也可以从列表共享多个功能板。
* 在您共享功能板时，默认情况下，用户将继承功能板上所有报表对象的查看权限。

   有关Workfront中对象层次结构的更多信息，请参阅 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   有关查看继承权限的信息，请参阅 [查看对象的继承权限](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 共享功能板

从列表中共享一个功能板或多个功能板是相同的。

1. 转到功能板列表，选择一个或多个功能板，然后单击 **共享** ![](assets/share-icon.png).

   或

   单击一个功能板的名称，然后单击**功能板操作>****共享**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

1. 在 **添加人员、团队、角色、组或公司……** 字段中，开始键入要与其共享功能板的用户、团队、角色、群组或公司的名称，然后在下拉列表中显示该名称时单击该名称。
1. （可选）要使功能板对系统中的所有用户都可访问，请单击 **设置** 图标，然后选择 **在系统范围内使此可见**.

1. 单击&#x200B;**保存**。
