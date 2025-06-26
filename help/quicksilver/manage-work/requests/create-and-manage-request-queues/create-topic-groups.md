---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建主题组
description: 主题组与请求队列相关联。 它们允许您根据请求的性质将请求队列分为多个类别。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 7c5959f4-f33f-4f5e-b031-748dbe1a24a5
source-git-commit: 0da05d048d0dab1c2f06870e589c1349c48ccc58
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 创建主题组

<!-- Audited: 2/2024 -->

主题组与请求队列相关联。 您可以使用主题组，根据请求的性质将请求队列分为多个类别。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront许可证</p> </td> 
   <td>   
      <p>新增：标准</p>
      <p>或</p> 
      <p>当前：计划</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 主题组概述

例如，如果您有一个营销请求的请求队列，则可以有一个主题组“母亲节促销活动”、一个二级主题组“数字媒体”和一个额外的二级主题组“印刷媒体”。 然后，可以在每个主题组内有多个队列主题。 例如，“横幅广告”和“博客”可以是“数字媒体”主题组的队列主题。

有关如何创建请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

使用主题组时，请考虑以下事项：

* 在一个请求队列中最多可创建10层主题组。
* 可与主题组关联的队列主题的数量没有限制。
* 主题组是可报告的对象。
* 您无法将主题组从一个项目移动到另一个项目。

## 创建主题组

我们建议您在创建队列主题之前创建主题组。 但是，可以在队列主题生成器中创建主题组。 有关创建队列主题的详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

创建主题组：

1. 转到您作为帮助请求队列发布的项目。\
   有关将项目发布为帮助请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

1. 单击左侧面板中的&#x200B;**主题组**。
1. 单击&#x200B;**新建主题组**。

   <!--   ![](assets/new-topic-group-box-nwe-350x306.png) -->

1. 指定以下信息：

   * **名称**：向此请求队列提交请求的用户可以看到该名称。
   * **描述**：在提交新请求的过程中，当用户选择主题组时，将显示描述。
   * **添加到主题组**：您可以将新的主题组添加到现有主题组，也可以直接将其添加到作为帮助请求队列发布的项目。

1. 单击&#x200B;**保存**。\
   这将在您的请求队列中创建一个新的主题组。 现在，您可以从请求队列下的第一个下拉菜单中选择其他类别。\
   有关提交请求的更多信息，请参阅[创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。
1. 要编辑现有的主题组，请从“主题组”列表中选择主题组，然后在打开的窗口中编辑详细信息。 单击&#x200B;**保存**&#x200B;以保存更改。
