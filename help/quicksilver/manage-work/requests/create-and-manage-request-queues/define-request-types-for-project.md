---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 为项目定义请求类型
description: 您可以按请求类型组织登录Adobe Workfront的问题或请求类型。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# 为项目定义请求类型

您可以按请求类型组织登录Adobe Workfront的问题或请求类型。

此组织有助于报告原因，并帮助用户了解在项目的生命周期中可能会发生哪种类型的意外工作。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfront许可证</a>*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须

* 拥有或创建项目

   有关创建项目的信息，请参阅 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

## 有关请求类型的注意事项

* 您可以指定在配置 **队列详细信息** 的双曲余切值。
* 您不必使项目成为请求队列，即可为项目定义请求类型。 为项目记录的任何问题都可以使用其他请求类型进行标记。
* 如果向项目添加队列主题，则必须在每个队列主题上定义请求类型，以在添加新问题或请求时显示该类型。 有关更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## 为项目定义问题或请求类型

1. 单击 **项目** 中。 ![](assets/main-menu-icon.png)

1. 单击项目的名称以将其打开。
1. 在左侧面板中，单击 **队列详细信息**.
1. 在 **队列属性** 选择 **请求类型** 您希望获得项目。

   >[!NOTE]
   >
   >您必须至少选择了一种请求类型。 您可以选择多个请求类型。

   从以下类型中进行选择：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求

   >[!TIP]
   >
   >您的Workfront管理员可能已重命名其中一些选项。 有关信息，请参阅 [配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. 单击&#x200B;**保存**。

   当您在任务或项目上输入新问题时，或者当您向项目提交新请求时（如果项目被启用为请求队列），您可以选择指定的请求类型。
