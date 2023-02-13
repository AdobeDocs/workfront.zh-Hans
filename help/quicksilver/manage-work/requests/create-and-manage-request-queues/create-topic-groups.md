---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建主题组
description: 主题组与请求队列关联。 它们允许您根据请求的性质将请求队列分层为多个类别。
author: Alina
feature: Work Management
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 创建主题组

主题组与请求队列关联。 它们允许您根据请求的性质将请求队列分层为多个类别。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员

## 主题组概述

例如，如果您有营销请求的请求队列，则可以拥有“母亲日营销活动”的主题组、“数字媒体”的第二级主题组，以及“打印媒体”的第二级主题组。 然后，每个主题组中可以有多个队列主题。 例如，“横幅广告”和“博客”可以是“数字媒体”主题组的队列主题。

有关如何创建请求队列的详细信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!TIP]
>
>* 在请求队列中，最多可以创建10层主题组。
>* 可以与主题组关联的队列主题的数量没有限制。
>* 主题组是可报告的对象。
>


## 创建主题组

我们建议您在创建队列主题之前先创建主题组。 但是，可以在队列主题生成器中创建主题组。 有关创建队列主题的更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

要创建主题组，请执行以下操作：

1. 转到作为帮助请求队列发布的项目。\
   有关将项目作为帮助请求队列发布的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 单击 **主题组** 中。 您可能需要单击 **显示更多**，则 **主题组**.
1. 单击 **新建主题组**.

   ![](assets/new-topic-group-box-nwe-350x306.png)

1. 指定以下信息：

   * **名称**:向此请求队列提交请求的用户可以看到该名称。
   * **描述**:当用户在提交新请求的过程中选择主题组时，将显示描述。
   * **添加到主题组**:您可以将新的主题组添加到现有的主题组，也可以直接将其添加到作为帮助请求队列发布的项目中。

1. 单击&#x200B;**保存**。\
   这会在请求队列中创建新的主题组。 您现在可以从请求队列下的第一个下拉菜单中选择其他类别。\
   有关提交请求的更多信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).
