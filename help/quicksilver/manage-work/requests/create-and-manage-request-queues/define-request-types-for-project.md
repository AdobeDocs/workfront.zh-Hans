---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定义项目的请求类型
description: 您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。
author: Lisa
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 6d9583f8a0e1e0c3712c8a47d68c5d5d321679f9
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 2%

---

# 定义项目的请求类型

您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。

此组织非常有用，可用于生成报表，以及帮助用户了解在项目存留期内可能会发生什么类型的意外工作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
    <p>新增：标准</p>
    <p>或</p>
    <p>当前：计划</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，必须执行以下操作：

* 拥有或创建项目

  有关创建项目的信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

## 有关请求类型的注意事项

* 在为项目配置&#x200B;**队列详细信息**&#x200B;区域时，您可以指定可在项目中记录的问题或请求的类型。
* 您无需使项目成为请求队列即可为项目定义请求类型。 为项目记录的任何问题都可以标记为不同的请求类型。
* 如果您将队列主题添加到项目中，则必须在每个队列主题上定义请求类型，以便在添加新问题或请求时显示它。 有关详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

## 定义项目的问题或请求类型

{{step1-to-projects}}

1. 单击项目名称以将其打开。
1. 在左侧面板中，单击&#x200B;**队列详细信息**。
1. 在&#x200B;**队列属性**&#x200B;部分中，为项目选择所需的&#x200B;**请求类型**。

   >[!NOTE]
   >
   >您必须至少选择一个请求类型。 您可以选择多种请求类型。

   从以下类型中选择：

   * 错误报告
   * 更改顺序
   * 问题
   * 请求

   >[!TIP]
   >
   >您的Workfront管理员可能已重命名其中一些选项。 有关信息，请参阅[配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 单击&#x200B;**保存**。

   在任务或项目上输入新问题时，或者在向项目提交新请求时（如果项目已作为请求队列启用），您指定的请求类型将可供选择。
