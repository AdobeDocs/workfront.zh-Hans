---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 提供对请求队列的访问权限
description: 提供对请求队列的访问权限时，您可以确定组织中的哪些人可以在Adobe Workfront的请求区域查看请求队列。
author: Becky
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 1%

---

# 提供对请求队列的访问权限

<!-- Audited: 6/2025 -->

提供对请求队列的访问权限时，您可以确定组织中的哪些人可以在Adobe Workfront的请求区域查看请求队列。

您可以根据请求队列中的不同用户是项目团队、项目组或项目公司的一员，为他们提供不同的访问权限。 您还可以向系统中的每个人提供请求队列访问权限。

这在邀请外部利益相关者进入Workfront并希望限制用户对特定区域的访问权限的组织中很有用。 在这种情况下，仅对与项目公司或组关联的用户打开的请求队列限制了外部利益相关者可见。 将访问权限授予任何人都可以让内部和外部利益相关者看到该请求。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准 </p>
   <p>规划 </p> </td> 
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

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在请求队列可供请求区域中的用户使用之前，您必须创建具有以下设置的项目：

* 将其指定为请求队列。 有关详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
* 将项目的状态更新为当前。

## 提供对请求队列的访问权限

1. 转到要提供请求队列访问权限的项目。

   >[!NOTE]
   >
   >只有状态为“当前”的项目才会显示在“请求”区域中。

1. 单击左侧面板中的&#x200B;**队列详细信息**。
1. 选择&#x200B;**发布为帮助请求队列**&#x200B;以将项目指定为请求队列。
1. 从显示的以下选项中进行选择：

   * **任何人**：任何用户都可以查看请求并将其添加到请求队列。
   * **拥有查看此项目访问权限的用户**：拥有项目查看权限的用户可以查看请求并将其添加到请求队列。
   * **此项目公司中的人员**：与项目公司关联的用户可以查看和添加请求。 与该项目关联的公司列在该选项旁边的括号中。
   * **此项目组的人员**：与项目组关联的用户可以查看和添加请求。 此选项旁边的括号中列出了与项目关联的组。

     当多个部门共享一个Workfront帐户以实现独特的组织目标时，组队列非常有用。 每个部门可能有自己的队列，其他组的成员应该看不到这些队列。

     有关谁拥有项目权限的信息，请参阅[在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

     编辑项目时，组和公司可以与项目相关联。 有关详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. 单击&#x200B;**保存**。
