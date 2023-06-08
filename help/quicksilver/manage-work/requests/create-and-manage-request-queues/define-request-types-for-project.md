---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定义项目的请求类型
description: 您可以按请求类型整理在Adobe Workfront中记录的问题或请求类型。
author: Alina
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9b6552fe496a1602786cdc6b6050d02cd367a531
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 2%

---

# 定义项目的请求类型

您可以按请求类型整理在Adobe Workfront中记录的问题或请求类型。

此组织非常有用，可用于生成报表，以及帮助用户了解在项目存留期内可能会发生什么类型的意外工作。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront计划</a>*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">许可证概述</a>*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须执行以下操作：

* 拥有或创建项目

  有关创建项目的信息，请参阅 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

## 有关请求类型的注意事项

* 在配置时，您可以指定可在项目上记录的问题或请求类型。 **队列详细信息** 项目区域。
* 您无需使项目成为请求队列即可为项目定义请求类型。 为项目记录的任何问题都可以使用不同的请求类型进行标记。
* 如果将“队列主题”添加到项目中，则必须在每个队列主题上定义“请求类型”，以便在添加新问题或请求时显示该队列主题。 有关更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

## 定义项目的问题或请求类型

1. 单击 **项目** 在主菜单中。 ![](assets/main-menu-icon.png)

1. 单击项目名称以将其打开。
1. 在左侧面板中，单击 **队列详细信息**.
1. 在 **队列属性** 部分，选择 **请求类型** 您想要的项目。

   >[!NOTE]
   >
   >您必须至少选择一个请求类型。 您可以选择多个请求类型。

   从以下类型中选择：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求

   >[!TIP]
   >
   >您的Workfront管理员可能已重命名其中的一些选项。 有关信息，请参阅 [配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. 单击&#x200B;**保存**。

   在任务或项目上输入新问题时，或者在向项目提交新请求时（如果项目已作为请求队列启用），您指定的请求类型将可供选择。
