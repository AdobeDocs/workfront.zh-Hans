---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 定义项目的请求类型
description: 您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。
author: Becky
feature: Work Management
exl-id: 627749bb-a8d7-4cc2-9d11-237811f82eb8
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 3%

---

# 定义项目的请求类型

<!-- Audited: 6/2025 -->

您可以按“请求类型”来整理Adobe Workfront中登录的问题或请求类型。 这对于报告相关原因以及帮助用户了解在项目存留期内可能会发生何种意外工作非常有用。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
    <p>标准</p>
    <p>规划</p></td>  
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

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，必须执行以下操作：

* 拥有或创建项目。

  有关创建项目的信息，请参阅[创建项目](../../../manage-work/projects/create-projects/create-project.md)。

## 有关请求类型的注意事项

* 在为项目配置队列详细信息区域时，您可以指定可在项目中记录的问题或请求类型。
* 您无需使项目成为请求队列即可为项目定义请求类型。 为项目记录的任何问题都可以标记为不同的请求类型。
* 如果您将队列主题添加到项目中，则必须在每个队列主题上定义请求类型，以便在添加新问题或请求时显示它。 有关详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

## 定义项目的问题或请求类型

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。
1. 在左侧面板中，单击&#x200B;**队列详细信息**。
1. 在&#x200B;**队列属性**&#x200B;部分中，为项目选择所需的&#x200B;**请求类型**：
   * 错误报告
   * 更改顺序
   * 问题
   * 请求

   >[!NOTE]
   >
   >* 您必须至少选择一个请求类型。 您可以选择多种类型。
   >* 您的Workfront管理员可能已重命名其中一些选项。 有关信息，请参阅[配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 单击 **Save**。在任务或项目上输入新问题时，或在向项目提交新请求时（如果项目已作为请求队列启用），您指定的请求类型将可供选择。
